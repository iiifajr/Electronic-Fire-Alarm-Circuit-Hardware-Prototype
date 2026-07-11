# 🚨 Electronic Fire Alarm Circuit (Electrical Circuits Hardware Prototype)

A standalone, hardware-level physical electrical circuit project implementing an automated analog Electronic Fire Alarm System. The system functions as an autonomous warning network engineered to trigger immediate auditory indicators upon detecting critical thermal thresholds. By utilizing the precise thermal-resistance boundaries of a solid-state thermistor coupled with switching NPN transistors, the circuit executes instant alarm actuation directly driven by ambient environmental heat, operating independently without microcontrollers or software assistance.

---

## 🔗 Project Resources & Drive Link

The complete hardware architecture schematics, full-scale assembly guides, and operational benchmarking datasets are fully accessible via the links below:

https://drive.google.com/drive/folders/1TxMhLyLK0fBRKNBXKQLcOuhqSqCZd2h-

🎥 **Inside the Drive Folder:** You will find an exclusive step-by-step video demonstration detailing the physical component alignment, breadboard rail connections, and live heat-testing execution.

---

## 📊 Core Objectives & System Architecture

This prototype serves as a direct hardware implementation of analog circuit design, focusing on voltage division, semiconductor switching properties, and thermal signal transduction.

### 🎯 Key Project Milestones:
* **Hardware Network Assembly:** Constructing and wiring the entire discrete electrical control layout on a solderless breadboard using an independent DC battery supply.
* **Thermal Response Validation:** Testing dynamic circuit feedback using external heat sources to verify instantaneous transistor region switching transitions.
* **Multi-Output Auditory Testing:** Configuring and validating the automated warning system utilizing distinct types of audible buzzers to analyze sound output stability.

---

## 🛠️ System Components & Technical Specifications

The system relies entirely on discrete laboratory hardware parts curated and calibrated for automated sensory switching:

| Component | Specification / Value | Operational Function |
| :--- | :--- | :--- |
| **BC548 Transistor** | NPN Bipolar Junction Transistor | Serves as the active current switch, triggering the active load upon bias threshold activation. |
| **Thermistor ($10\text{ kΩ}$)** | NTC/PTC Thermal Resistor | Acts as the central analog heat sensor, varying loop resistance dynamically with temperature shifts. |
| **Active Piezo Buzzer** | Standard Discrete DC Buzzer | Internal onboard acoustic load used to run baseline frequency threshold test runs. |
| **External High-Output Buzzer**| Extended Wired Module (SFM-27) | Secondary external alarm load tested to benchmark higher sound decibel outputs. |
| **Signal Diode** | Silicon PN Junction Diode | Provides unidirectional circuit pathway control and protects against inductive feedback spikes. |
| **Biasing Resistor** | Fixed $1\text{ kΩ}$ Resistor | Works within the input sensory divider branch to establish operational transistor baseline bias. |
| **9V Battery** | DC Power Source (Panasonic NEO) | Provides stable baseline voltage and steady current loop drive across the hardware array. |
| **Mechanical Switch & Clips** | Toggle Switch / Battery Snap | Governs initial system-wide power-up gating and physical rail connections. |
| **Breadboard & Wires**| Solderless Grid & Jumper Wires | The physical prototyping platform used to wire, interconnect, and ground all circuit nodes. |

---

## 🔌 Circuit Interfacing & Theory of Operation

The circuit leverages basic passive electronic configurations to behave as an autonomous thermal comparator:

1. **Ambient State (Alarm OFF):** At safe room temperatures, the thermistor's static resistance value forces the voltage divider node to keep the base voltage ($V_{be}$) of the BC548 NPN transistor well below the critical $0.7\text{ V}$ forward-bias threshold. The transistor remains in the **Cut-off** state, acting as an open switch that restricts load current.
2. **Thermal Activation State (Alarm ON):** When external heat is introduced, the thermistor's internal resistance changes rapidly. This dynamically reallocates voltage across the divider network, forcing $V_{be}$ to cross the $0.7\text{ V}$ conduction barrier. The transistor immediately jumps into the **Saturation** region, working as a closed switch that completes the path to ground and activates the buzzer continuously.

---

## 🚀 Physical Hardware Verification & Inventory

### 1. Pre-Assembly Component Inventory
Discrete inventory preparation phase showcasing all necessary components cleanly labeled before physical deployment.

<img width="661" height="1165" alt="IMG_5487" src="https://github.com/user-attachments/assets/48edaaef-2bc2-4c85-b6de-907574025ebc" />


<img width="674" height="1171" alt="IMG_5488" src="https://github.com/user-attachments/assets/5c65cd30-f5a3-4ea2-94f9-217bcc69a4cb" />


<img width="657" height="1133" alt="IMG_5489" src="https://github.com/user-attachments/assets/f39a12a0-bc58-4383-a9a4-470a7b4ba203" />


<img width="652" height="1059" alt="IMG_5490" src="https://github.com/user-attachments/assets/7bb31073-2722-4023-b5fe-a1903a9485f5" />


### 2. Complete Breadboard Assembly & Testing Layouts
Top-down and profile views capturing the finalized physical control path wiring, showcasing the integration of both buzzer variations tested during the experimentation phases.

<img width="1280" height="716" alt="IMG_5485" src="https://github.com/user-attachments/assets/2eaabbdc-ca3a-48d8-ba19-6126b0c12ad6" />


<img width="1280" height="725" alt="IMG_5486" src="https://github.com/user-attachments/assets/3f7fec3b-a412-4dfd-b3c0-0460f68ba39b" />


---

## 🌐 Industrial & Real-World Applications

The solid-state automation principles validated in this design are directly applicable to commercial security sectors:
* **Industrial Facility Fire Safety Loops:** Scalable into low-cost localized zoning sensors for electrical cabins and warehouse bays.
* **Overheat Safety Overrides:** Integrates easily into heavy manufacturing machinery to trip relays and cut power during cooling pump failures.
* **Server Room Environmental Alarms:** Serves as a failsafe hardware alarm system backing up cloud-based climate control tracking grids.

---

## 📈 Engineering Outlook & Future Enhancements

To upgrade this primitive analog assembly into an industrial, commercially deployment standard, several revisions can be applied:
1. **Adding an Electromechanical Relay:** Interfacing a high-current relay parallel to the collector path to trigger $220\text{ V}$ industrial exhaust fans or sprinkler solenoids safely.
2. **Integrating a Tuning Potentiometer:** Placing a multi-turn trimmer potentiometer inside the voltage divider branch to allow users to manually calibrate the precise alarm temperature activation point.
3. **LED Visual Warning Indicators:** Appending a low-power red LED branch synchronized with the sound output to provide dual visual-audible sensory alerts during alarm windows.

---

## 👥 Project Owner & Affiliation

* **Lead Engineer:** Eng. Fajr Aldajani
* **Collaboration:** Individual Project (Developed Independently)
* **Course:** Electrical Circuits
* **Affiliation:** Taif University
* **Project Status:** Completed Successfully! 🚀
