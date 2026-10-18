# Intelligent Embedded Battery Management System for an Autonomous Solar Drone

## 📌 Context

This project was developed during my **End-of-Studies Internship at Capgemini Engineering Tunisia**. It focuses on designing a simulation-based intelligent Battery Management System (BMS) for an autonomous solar agricultural drone, combining embedded software, battery monitoring, artificial intelligence, and flight simulation.

## 🎯 Objectives

- Develop an STM32-based embedded BMS for battery monitoring.
- Estimate battery State of Charge (SoC) and State of Health (SoH).
- Predict short-term energy consumption and estimate remaining flight endurance.
- Detect battery and energy-system anomalies using machine learning.
- Integrate battery data with simulated flight telemetry.
- Provide real-time monitoring, risk assessment, and decision support through a web dashboard.

## 🧠 Technologies & Tools

- **Embedded Systems:** STM32F446RE, C, STM32CubeIDE, FreeRTOS
- **Battery Management:** SoC estimation using Coulomb Counting, voltage and current monitoring
- **Machine Learning:** Scikit-learn, MLP Regression, Isolation Forest, Z-score-based anomaly detection
- **Drone Simulation:** ArduPilot SITL, MAVLink, pymavlink
- **Backend & Dashboard:** Python, Flask
- **Communication:** UART, UDP, MAVLink
- **Data Processing:** Pandas, NumPy, data preprocessing and feature scaling

## 🏗 System Architecture

The system consists of four main layers:

- **Embedded BMS:** STM32 firmware with FreeRTOS for battery monitoring and SoC estimation.
- **Flight Simulation:** ArduPilot SITL provides simulated flight telemetry through MAVLink.
- **AI Processing:** Machine learning models predict future energy consumption and identify abnormal operating conditions.
- **Monitoring & Decision Support:** A Flask dashboard combines battery and flight data to display system status, remaining energy, risk indicators, and recommendations.

The STM32 and flight simulation operate as separate data sources, with Python scripts collecting and integrating their data into the dashboard.

## 📊 Results

- Implemented an STM32-based BMS prototype with FreeRTOS.
- Integrated battery monitoring with simulated drone flight telemetry.
- Achieved an **R² score of approximately 0.87** with the selected MLP energy prediction model on the evaluation dataset.
- Developed an anomaly detection pipeline using Isolation Forest and rule-based checks.
- Integrated AI outputs into a Flask dashboard for energy assessment and decision support.

*Note: Results are based on model evaluation and simulation; they do not represent validation on a physical drone.*

## 🔒 Note

This repository presents a simulation-based prototype. Physical drone flight tests and real hardware integration with a complete battery sensing system were not performed. Any datasets, source code, and technical materials published in this repository must comply with applicable confidentiality requirements.

## 👤 Author

**Ameni Frada**  
Engineering Graduate in Advanced Technologies  
Specialization: Advanced Electronics and Nanotechnology  
ENSTAB — Tunisia
