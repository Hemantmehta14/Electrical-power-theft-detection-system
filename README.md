# Electrical-power-theft-detection-system

This project is an Arduino-based Electrical Power Theft Detection System designed to identify unauthorized electricity consumption in a distribution line. The system uses two Arduino boards acting as a Main Node and a Consumer Node, along with reed switches for pulse-based energy monitoring. By comparing energy pulses at both ends, the system can detect discrepancies that may indicate power theft.

Features
Real-time power theft detection
Dual-node architecture using Arduino
Pulse monitoring using reed switches
Wireless/serial data communication between nodes
Theft alert generation when energy mismatch exceeds threshold
Low-cost and scalable design
Hardware Components
Main Node
Arduino Uno
Reed Switch
Communication Module (RF/NRF24L01/Serial)
Power Supply
Consumer Node
Arduino Uno
Reed Switch
Communication Module (RF/NRF24L01/Serial)
Power Supply
Working Principle
The Main Node measures the total energy pulses generated at the distribution side using a reed switch.
The Consumer Node measures the energy pulses consumed at the consumer side.
Both nodes exchange pulse count data.
The Main Node continuously compares transmitted and received pulse counts.
If the difference exceeds a predefined threshold, the system flags a potential power theft condition and generates an alert.
System Architecture
Electric Meter (Source)
        |
   Reed Switch
        |
   Main Arduino
        |
Communication Link
        |
Consumer Arduino
        |
   Reed Switch
        |
Electric Meter (Load)
Applications
Smart Grid Monitoring
Residential Energy Management
Industrial Power Distribution
Utility Theft Prevention
Remote Energy Auditing
Future Improvements
IoT-based cloud monitoring
GSM/SMS alert notifications
Mobile application integration
Data logging and analytics
Multiple consumer node support
Technologies Used
Arduino IDE
Embedded C/C++
Arduino Uno
Reed Switch Sensors
Serial/Wireless Communication
Project Outcome

The system successfully detects abnormal differences between supplied and consumed electrical energy, helping identify possible electricity theft and improving power distribution transparency.
