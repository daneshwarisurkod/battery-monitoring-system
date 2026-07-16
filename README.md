# battery-monitoring-system
IoT-enabled Li-ion Battery Monitoring System using ESP32, Embedded C, and MATLAB/Simulink.
# Battery Monitoring System using ESP32 and Arduino Uno

## Project Overview

This project presents a Battery Monitoring System (BMS) for multi-cell lithium-ion battery packs. The system continuously monitors critical battery parameters including individual cell voltage, pack voltage, current, temperature, and State of Charge (SOC) in real time.

The project combines Arduino Uno for sensor data acquisition, ESP32 for data processing and SOC estimation, the BQ76925 battery monitoring IC for cell voltage measurement, and MATLAB/Simulink for system simulation and validation.

---

## Problem Statement

In multi-cell lithium-ion battery packs, individual cells may charge and discharge unevenly, leading to voltage imbalance, overheating, reduced efficiency, and shorter battery life. Monitoring only the total battery voltage cannot detect weak or damaged cells, which may result in unsafe operating conditions.

This project addresses these challenges by monitoring individual cell parameters and identifying abnormal battery conditions in real time.

---

## Objectives

- Design a battery monitoring system for a multi-cell lithium-ion battery pack.
- Measure individual cell voltages and estimate State of Charge (SOC).
- Monitor pack voltage, current, and temperature continuously.
- Detect abnormal operating conditions.
- Improve battery safety, efficiency, and lifespan.

---

## Hardware Components

- Arduino Uno
- ESP32
- BQ76925 Battery Monitoring IC
- Current Sensor
- Temperature Sensor
- Lithium-ion Battery Pack
- Voltage Divider Circuit
- DC Motor (Load)

---

## Software Used

- Arduino IDE
- Embedded C
- MATLAB
- Simulink

---

## System Workflow

1. Arduino Uno collects battery voltage, current, and temperature data.
2. BQ76925 measures individual cell voltages.
3. ESP32 processes sensor data and calculates State of Charge (SOC).
4. The system continuously checks battery conditions.
5. Results are displayed through the Serial Monitor.
6. Abnormal conditions such as overcharging, deep discharge, overheating, and cell imbalance are detected.

---

## Features

- Real-time battery monitoring
- Individual cell voltage measurement
- Pack voltage monitoring
- Current sensing
- Temperature monitoring
- State of Charge (SOC) estimation
- Cell imbalance detection
- Overcharge protection
- Deep discharge detection
- MATLAB/Simulink validation

---

## Hardware Circuit

> Add the hardware circuit image here.

![Hardware Circuit](Images/Hardware_Circuit.png)

---

## Flow of Operation

> Add the flowchart image here.

![Flowchart](Images/Flowchart.png)

---

## Hardware Output

> Add screenshots of the Serial Monitor output and hardware setup.

![Hardware Output](Images/Hardware_Output.png)

---

## MATLAB/Simulink Model

The battery monitoring system was simulated using MATLAB/Simulink to validate voltage monitoring, current sensing, temperature monitoring, and protection logic before hardware implementation.

![Simulation Model](Images/Simulink_Model.png)

---

## Results

The implemented system successfully monitored:

- Individual Cell Voltage
- Pack Voltage
- Current
- Temperature
- State of Charge (SOC)

The system was able to identify abnormal battery conditions including:

- Overcharging
- Deep discharge
- Cell imbalance
- Overheating

---

## Waveform Analysis

Include screenshots of the following simulation waveforms:

- Voltage waveform
- Current waveform
- Temperature waveform
- State of Charge (SOC) graph

---

## Applications

- Electric Vehicles (EVs)
- Battery Management Systems
- Solar Energy Storage
- Robotics
- Portable Energy Storage Systems
- Industrial Automation

---

## Future Improvements

- Cloud-based battery monitoring
- Mobile application integration
- CAN Bus communication
- State of Health (SOH) estimation
- Predictive maintenance using Machine Learning

---

## Conclusion

A Battery Monitoring System for multi-cell lithium-ion battery packs was successfully designed and implemented using Arduino Uno, ESP32, and the BQ76925 battery monitoring IC.

The system continuously monitored battery voltage, current, temperature, and State of Charge (SOC), enabling early detection of unsafe operating conditions. MATLAB/Simulink simulations complemented the hardware implementation by validating system performance under different operating scenarios.

This project demonstrates the practical application of embedded systems and battery management techniques for electric vehicles and renewable energy systems.

---

## Repository Structure

```text
Arduino_Code/
ESP32_Code/
MATLAB/
Images/
Results/
Documentation/
```

---

## Author

**Daneshwari B. Surkod**

Bachelor of Engineering (Electrical and Electronics Engineering)

BNM Institute of Technology
