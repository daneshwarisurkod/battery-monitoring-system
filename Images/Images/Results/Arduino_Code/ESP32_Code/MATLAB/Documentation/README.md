Abstract
Multi-cell lithium-ion batteries may suffer from cell imbalance, overheating, and reduced battery life.
Monitoring only total battery voltage cannot identify weak or faulty cells.
This project develops a battery monitoring system for a multi-cell battery pack.
The system measures individual cell voltage, State of Charge (SOC), current, and temperature.
BQ76925 IC is used for accurate cell voltage sensing.
Arduino UNO and ESP32 are used for data collection, processing, and SOC calculation.
The system continuously monitors battery parameters in real time.
It detects abnormal conditions such as overcharging, deep discharge, overheating, and cell imbalance.

  Introduction
Lithium-ion batteries are used in EVs, solar applications, power banks, and portable devices.
A battery pack contains multiple cells connected together.
Each cell may behave differently in voltage, temperature, and charging/discharging.
Unequal cell conditions reduce battery life, efficiency, and safety.
State of Charge (SOC) shows the remaining battery capacity.
Accurate SOC helps prevent overcharging and deep discharge.
This project monitors individual cell voltage, SOC, current, and temperature in real time.

PROBLEM STATEMENT
In multi-cell battery packs, each cell may charge and discharge differently, causing voltage imbalance, overheating, reduced efficiency, and shorter battery life. Monitoring only the total battery voltage cannot identify weak or damaged cells, which may lead to unsafe conditions. To overcome these issues, this project develops a battery monitoring system that measures individual cell SOC, voltage, current, and temperature in real time, thereby improving battery safety, performance, and lifespan.

OBJECTIVE
To design a battery monitoring system for a multi-cell lithium-ion battery pack.
To measure individual cell voltages and estimate State of Charge (SOC).
To monitor pack voltage, current, and temperature in real time.
To display battery parameters continuously for analysis.
To improve battery safety, efficiency, and lifespan.

Methodology
Connect the multi-cell lithium-ion battery pack to the monitoring circuit.
Use BQ76925 IC to measure individual cell voltages & pack voltage accurately.
Use a current sensor to measure current.
Use a temperature sensor to monitor battery temperature.
Arduino UNO collects data from all sensors.
ESP32 is used for data processing and SOC calculation of each cell.
Total battery pack voltage is calculated from cell voltages.
All parameters are monitored continuously in real time.
The system detects overcharging, deep discharge & overheating.
Final output is displayed for battery condition analysis.

HARDWARE COMPONENTS
Arduino Uno – Used as the main controller for processing sensor data and system control. 
ESP32 – Used because BQ76925 gives 3.3V output (compatible with ESP32), provides more analog pins, and is used to calculate individual cell voltage SOC of each cell. 
BQ76925 IC – Used to measure individual cell voltages of the battery pack & pack voltage. 
Current Sensor – Used to measure current. 
Temperature Sensor – Used to monitor battery temperature. 
Lithium-ion Cells – Used as the battery source for testing and monitoring. 
Resistors (Voltage Divider) – Used to safely step down voltage for controller input. 
DC Motor – Used as a load to consume battery power and test battery performance during discharge

Results 
Successfully measured individual cell voltages of the battery pack. 
Calculated State of Charge (SOC) for each cell accurately. 
Monitored total battery voltage, current, and temperature in real time. 
Detected voltage imbalance between cells during operation. 
Displayed battery parameters continuously through the controller system. 
Improved battery safety by identifying abnormal conditions. 
Achieved a low-cost and efficient battery monitoring solution. 

Conclusion
The project successfully developed a smart battery monitoring system for a multi-cell lithium-ion battery pack. 
It accurately measured individual cell voltage, SOC, current, and temperature in real time. 
The system helped detect cell imbalance and unsafe battery conditions. 
It improved battery safety, performance, and lifespan through continuous monitoring. 
This low-cost solution can be effectively used in electric vehicles, solar systems, and portable devices. 

References 
[1] S. Li, C. Mi and M. Zhang, "Battery Management System for Electric Vehicles", IEEE Transactions on Industrial Electronics, vol. 65, no. 4, pp. 1–10, 2018.
 
[2] H. He, R. Xiong and J. Fan, "Evaluation of Lithium-Ion Battery Equivalent Circuit Models for State of Charge Estimation", Applied Energy, vol. 102, pp. 808–815, 2013.
 
[3] Texas Instruments, "BQ76925 Analog Front-End for Battery Monitoring System", Datasheet, 2015.
 
[4] A. Emadi, Y. J. Lee and K. Rajashekara, "Power Electronics and Motor Drives in Electric, Hybrid Electric, and Plug-In Hybrid Electric Vehicles", IEEE Transactions on Industrial Electronics, vol. 55, no. 6, pp. 2237–2245, 2008.
 
[5] M. Chen and G. A. Rincon-Mora, "Accurate Electrical Battery Model Capable of Predicting Runtime and I–V Performance", IEEE Transactions on Energy Conversion, vol. 21, no. 2, pp. 504–511, 2006.
