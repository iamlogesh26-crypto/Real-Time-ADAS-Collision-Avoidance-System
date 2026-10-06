# Real-Time ADAS Collision Avoidance System

## Overview

The **Real-Time ADAS Collision Avoidance System** is an ESP32-based four-wheel vehicle prototype developed to demonstrate real-time collision avoidance and safety-aware vehicle control.

The system continuously monitors the surrounding environment and vehicle motion using multiple sensors. Sensor information is processed to support collision-risk assessment, fault isolation, and safety supervision.

## Key Features

- Real-time obstacle detection
- Sensor fusion
- Fault isolation
- Collision-risk assessment
- Safety supervision
- Bluetooth-based vehicle control
- Real-time task prioritization
- Emergency motor stopping
- OLED status display
- Red LED and buzzer safety indication

## Hardware Components

- ESP32 Development Board
- HC-SR04 Ultrasonic Sensor
- IR Sensors
- MPU6050
- L298N Motor Drivers
- DC Gear Motors
- OLED Display
- Buzzer
- Red LED
- Lithium Battery
- Four-Wheel Chassis
- Breadboard and connecting wires

## System Architecture

Sensors  
↓  
Sensor Monitoring  
↓  
Sensor Fusion  
↓  
Fault Isolation  
↓  
Collision Risk Assessment  
↓  
Safety Supervision  
↓  
Vehicle Action

## Working Principle

The ESP32 receives movement commands through Bluetooth and continuously monitors the vehicle using the ultrasonic sensor, IR sensors and MPU6050.

When an obstacle is detected within the defined safety region, the safety mechanism can override the normal movement command and stop the vehicle.

## Safety Features

### Sensor Fusion
Information from multiple sensors is considered together to improve the reliability of the decision.

### Fault Isolation
Abnormal or unavailable sensor information can be identified so that faulty sensor data does not directly control the safety decision.

### Mixed-Criticality Scheduling
Safety-related operations are given higher priority than less critical operations.

### Safety Supervision
The safety supervisor monitors the system and can override normal vehicle control when a dangerous condition is detected.

## Vehicle Control

The prototype supports Bluetooth movement commands:

- `F` → Forward
- `B` → Backward
- `L` → Left
- `R` → Right
- `S` → Stop

## Project Status

**Working Hardware Prototype**

## Documentation

- Project Poster
- Project Report

## Applications

- Automotive ADAS
- Collision detection and driver assistance
- Autonomous vehicle safety concepts
- Industrial AGVs
- Warehouse robots
- Safety-critical embedded systems

## Author

**Logesh S**

Electronics and Communication Engineering
