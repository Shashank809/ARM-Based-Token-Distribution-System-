# ARM based Token Distribution System

## Overview
This project implements a real-time Token Distribution System using the ARM7 LPC2148 microcontroller.

The system is designed to manage token generation and display using an infrared (IR) sensor for detection and a 7-segment display for output. It is suitable for applications like queue management in events, cafeterias, and service centers.

---

## Problem Statement
Design a system that:
- Detects user presence using an IR sensor
- Generates tokens sequentially
- Displays token number on a 7-segment display
- Ensures accurate counting without duplication
- Works in real-time with reliable detection

---

## Key Features
- IR Obstacle Sensor for detection
- Automatic Token Increment System
- 7-Segment Display Output
- Real-Time Operation
- Simple and Efficient Embedded Design
- Low Power Consumption

---

## System Architecture
The system consists of:
- IR Sensor connected to LPC2148 for detection
- Microcontroller processes input signal
- Token counter logic increments value
- Output displayed on 7-segment display

Flow:
- Object detected → Signal sent to MCU  
- MCU increments token count  
- Updated token displayed  

---

## Hardware Components

| Component            | Description                          | LPC2148 Pin |
|---------------------|--------------------------------------|------------|
| IR Sensor           | Detects object/person                | P0.x       |
| LPC2148 MCU         | Main controller                      | -          |
| 7-Segment Display   | Displays token number                | P0.x / P1.x |
| Power Supply        | 3.3V / 5V                            | VCC, GND   |

---

## Interfacing
As shown in the diagram:
- IR sensor provides digital output to the microcontroller
- 7-segment display connected to GPIO pins
- MCU reads sensor input and updates display accordingly

---

## Working Principle
1. IR sensor detects presence of an object/person  
2. Signal is sent to LPC2148  
3. Microcontroller increments token count  
4. Token number is displayed on 7-segment display  
5. System waits for next detection  

---

## Software Design
- Embedded C
- GPIO-based input/output handling
- Delay-based debouncing for sensor stability

---

## Applications
- Queue management systems
- Event token distribution
- Cafeteria and mess systems
- Hospital patient token systems

---

## Advantages
- Simple implementation
- Cost-effective
- Real-time performance
- Easy to scale

---

## Limitations
- Limited display (single digit unless extended)
- No remote monitoring
- Depends on sensor accuracy

---

## Conclusion
The Token Distribution System provides a simple and efficient solution for managing queues using embedded systems. By integrating IR sensing with real-time processing, the system ensures accurate and reliable token generation.

---
