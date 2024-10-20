# IoT-BasedFertiliserMixingSystem

An Internet of Things (IoT)-based fertilizer mixing system designed for precision farming and hydroponic environments. The system automates the process of dispensing fertilizers based on real-time sensor data, providing users with remote control and monitoring through the Blynk IoT platform.

Table of Contents

Overview
Features
Hardware Requirements
Software Requirements
System Architecture
Installation and Setup
Usage
Project Structure
Future Improvements
Contributing
License
Overview

This project automates fertilizer mixing using sensors and an IoT platform to ensure precision and efficiency in hydroponic and traditional farming. By leveraging the Blynk platform, users can monitor sensor data in real-time and adjust fertilizer volumes remotely. This system is designed to improve crop yield by accurately controlling the nutrient mix applied to the plants, ensuring the appropriate concentration of fertilizers is dispensed.

Features

Remote Monitoring and Control: Through the Blynk app, users can monitor TDS (Total Dissolved Solids) and water level sensors and control pumps and solenoids remotely.
Real-time Data Visualization: Sensor data, including TDS values and water levels, are sent to the Blynk platform for real-time monitoring.
User Input for Fertilizer Volume: The user can specify the volume of fertilizer to be dispensed.
Automatic Fertilizer Dispensing: Activates pumps and solenoids based on sensor readings and user-defined volumes.
Flow Monitoring: Monitors flow sensors to ensure accurate dispensing of fertilizer.
Data Logging: Sends real-time data, including dispensed volumes, to the Blynk platform for user reference.
Hardware Requirements

ESP32/Arduino microcontroller (for IoT connectivity)
TDS Sensor (to monitor the concentration of nutrients in the solution)
Water Level Sensors (to monitor water levels in the tank)
Flow Sensors (to monitor the volume of liquid dispensed)
Pumps & Solenoids (to control the flow of fertilizer and water)
Power Supply (appropriate for the microcontroller and connected hardware)
Software Requirements

Arduino IDE (for coding and flashing the microcontroller)
Blynk App (for remote control and monitoring)
Wi-Fi Connectivity (for IoT communication)
Libraries:
Blynk
Flow Sensor library
TDS Sensor library
System Architecture

The system architecture involves sensor integration with an ESP32/Arduino board, communication over Wi-Fi, and control through the Blynk app. The sensors provide real-time data, which is used to regulate the operation of pumps and solenoids responsible for dispensing fertilizer.
