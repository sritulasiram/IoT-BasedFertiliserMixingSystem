# IoT-BasedFertiliserMixingSystem

Overview

This project implements an IoT-based fertilizer mixing system designed for precision farming and hydroponic environments. The system integrates sensors to monitor water levels and Total Dissolved Solids (TDS), enabling real-time adjustments of fertilizer ratios. Using the Blynk platform, users can input desired values, monitor the system, and control pumps and solenoids remotely.

Features

Real-time Monitoring: Monitors water levels and TDS levels using sensors.
User Inputs: Users can specify desired fertilizer quantities through the Blynk app.
Automated Dispensing: Activates pumps and solenoids to mix fertilizers based on user input and sensor data.
Flow Sensors: Tracks the volume of fertilizer dispensed and ensures accurate measurements.
Data Logging: Sends real-time data (TDS value, water level, dispensed volume) to the Blynk app for user review.
System Architecture

The system architecture involves multiple sensors, a microcontroller (Arduino/ESP32), pumps, solenoids, and a cloud-based control platform (Blynk). The flowchart below provides a simplified representation of the processes involved:

text
Copy code
Start
 └── Initialize System
      ├── Connect to Wi-Fi
      ├── Connect to Blynk
      └── Setup Pins & Interrupts (for pumps, solenoids, sensors)
           ├── Read Sensors (TDS, Water Level)
           └── Wait for User Input (via Blynk)
                ├── Dispense Fertilizer (Activate Pumps & Solenoids)
                └── Monitor Flow Sensors (Track Volume)
 └── Send Data to Blynk (TDS, Water Level, Dispensed Volume)
End/Repeat
Technologies Used

Hardware: ESP32/Arduino, Flow sensors, TDS sensor, Water level sensors, Pumps, Solenoids
Software: Arduino IDE, Blynk IoT Platform
Programming Languages: C/C++ for Arduino code
