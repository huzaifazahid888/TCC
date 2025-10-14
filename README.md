# Fire Control Computer (FCS)

##  Objective
The **Fire Control Computer (FCS)** is a critical embedded computing unit designed to calculate **real-time ballistic firing solutions** for the main battle tank.  
Its primary objective was to process sensor data (environmental, mechanical, and ballistic) and compute **accurate azimuth and elevation corrections** for the gun to ensure high first-round hit probability under varying environmental and terrain conditions.

---

##  Project Overview
The FCS acts as the **brain of the fire control system**, interfacing with multiple subsystems such as:
- **Laser rangefinder**
- **Gyroscopes & inclinometers**
- **Charge temperature & muzzle velocity sensors**
- **Barometric & ambient sensors**
- **Gun Control Box (GCB)** via CAN bus  

The system continuously processes this data through **ballistic models**, applies **real-time compensation algorithms**, and sends corrected commands to the GCB for precise targeting and stabilization.

---

##  Skills Demonstrated
- Embedded firmware development for **real-time ballistic computation** on STM32 platform.  
- Implementation of **multi-sensor data fusion**, filtering, and calibration routines.  
- Development of **interpolation-based ballistic tables** with environmental compensation.  
- Design of **real-time control loops** ensuring sub-millisecond data handling.  
- Implementation of **CAN communication** between FCS and GCB for trajectory synchronization.  
- Optimization of algorithm execution time and memory usage under deterministic constraints.  
- Validation of results through **tank field trials and trajectory testing**.  

---

##  Tools & Technologies Used
| Category | Tools / Technologies |
|-----------|----------------------|
| **Microcontroller** | STM32F407 (ARM Cortex-M4) |
| **Programming Language** | C++ |
| **Development Tools** | STM32CubeIDE, Keil uVision, ST-Link, Logic Analyzer |
| **Communication Protocols** | CAN, UART |
| **Simulation Tools** | MATLAB/Simulink for ballistic modeling |
| **Testing Equipment** | CAN Sniffer, Oscilloscope, Environmental Sensor Rig |
| **Sensors Integrated** | Laser rangefinder, gyroscope, temperature, pressure, crosswind sensors |

---

## ⚙️ System Architecture

**Block Diagram:**

---

##  Implementation Summary
- Implemented **Kalman-style filtering** to smooth noisy sensor inputs (gyro, rangefinder, pressure).  
- Designed **ballistic computation modules** performing:
  - Time-of-flight calculation  
  - Parallax correction  
  - Temperature & altitude compensation  
- Developed **lookup-table interpolation system** for ballistic curves across multiple charge and ammunition types.  
- Implemented **safety and diagnostic routines** for sensor faults and out-of-bound readings.  
- Integrated **CAN-based feedback loop** to synchronize with GCB for servo control updates.

---

##  Results & Testing
- Achieved **>85% first-round hit probability** during tank field trials.  
- Demonstrated **stable and repeatable ballistic performance** across environmental variations.  
- Reduced computational latency to under **1.5 ms per firing cycle**.  
- System validated through **simulated trajectories in MATLAB** and **live tank tests**.  

---

##  Contact
**Muhammad Huzaifa**  
Embedded Systems Designer | Islamabad, Pakistan  
📧 [huzaifazahid888@gmail.com](mailto:huzaifazahid888@gmail.com)  
🔗 [linkedin.com/in/huzaifa-engineer](https://linkedin.com/in/huzaifa-engineer)

