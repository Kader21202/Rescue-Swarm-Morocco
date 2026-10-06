\# Rescue Swarm Morocco — System Architecture



\## 1. Architecture Overview



Rescue Swarm Morocco is conceived as a modular maritime rescue system in which specialized unmanned units cooperate during a multi-victim rescue mission.



The target operational chain is:



\*\*Rescue Station → Rescue Carrier → ScoutPods / RescuePods → Rescue Islands → Rescue Carrier → Shore\*\*



The Rescue Carrier remains the principal evacuation vehicle between the accident area and the shore.



\## 2. Rescue Station



The Rescue Station represents the mission supervision and human oversight level.



Its intended functions include:



\- receiving and consolidating distress information;

\- mission initialization;

\- monitoring robotic units;

\- human supervision of autonomous operations;

\- visualization of victim and vehicle states;

\- emergency intervention and mission termination.



\## 3. Rescue Carrier



The Rescue Carrier is an unmanned maritime vehicle intended to transport rescue modules rapidly toward the accident area.



Its target functions include:



\- transport of RescuePods and ScoutPods;

\- transport or deployment of Rescue Islands;

\- high-speed transit away from victims;

\- recovery of secured victims;

\- allocation of safe positions for rescued people;

\- evacuation of victims to shore;

\- repeated accident-zone-to-shore rotations when required.



The Carrier is designed without an onboard pilot or operational rescue crew.



\## 4. ScoutPods



ScoutPods are lightweight unmanned search units.



Their intended functions include:



\- rapid local exploration;

\- visual observation;

\- victim detection and localization;

\- transmission of situational information;

\- assistance in maintaining an updated map of the rescue area.



\## 5. RescuePods



RescuePods are individual robotic recovery units.



Their intended functions include:



\- controlled approach to a victim;

\- low-speed operation near humans;

\- soft and protected physical interaction;

\- assistance in securing passive or active victims;

\- transfer toward a Rescue Island or Rescue Carrier when appropriate.



Propulsion near victims must remain protected and safety-constrained.



\## 6. Rescue Islands



Rescue Islands are temporary mobile floating safety platforms.



Their purpose is to maintain rescued victims in a safer temporary location while the Rescue Carrier performs evacuation rotations.



They are not intended to become the principal evacuation vehicle.



After their occupants have been transferred to the Rescue Carrier, empty Rescue Islands may autonomously return toward shore.



\## 7. Artificial Intelligence Architecture



Artificial intelligence is intended to operate across the mission rather than inside a single vehicle.



The conceptual information and control chain is:



\*\*Sensors → Perception → Mission State → AI Decision Layer → Independent Safety Gate → Actuators\*\*



Potential AI-supported functions include:



\- victim detection and localization;

\- situation interpretation;

\- priority estimation;

\- task allocation;

\- route and mission planning;

\- coordinated deployment of robotic units;

\- assistance during controlled victim approach;

\- evacuation planning;

\- resource management;

\- mission reconfiguration following failures or environmental changes.



\## 8. Independent Safety Layer



AI decisions must not directly bypass safety-critical constraints.



A deterministic safety layer is intended to evaluate actuator commands before execution.



Examples of constraints include:



\- maximum approach speed near a victim;

\- propulsion protection;

\- prohibited contact zones;

\- force limitations;

\- emergency stop conditions;

\- communication-loss behavior;

\- minimum stability requirements.



\## 9. Mission Sequence



A representative target mission is:



1\. distress event detected;

2\. Rescue Carrier deployed from shore;

3\. Carrier reaches the accident area;

4\. ScoutPods search and localize victims;

5\. mission state is updated;

6\. RescuePods are assigned to victims;

7\. victims are progressively secured;

8\. temporary Rescue Islands receive victims when required;

9\. Carrier receives victims into available safe positions;

10\. Carrier returns victims to shore;

11\. Carrier may return to the accident area;

12\. remaining victims are evacuated;

13\. empty Rescue Islands return;

14\. robotic units return and the mission terminates.



\## 10. Architecture Status



This document describes the \*\*target system architecture\*\*.



Individual components and experimental capabilities remain subject to progressive design, prototyping, testing and validation.



\*\*Project status: ongoing research and development — 2026.\*\*

