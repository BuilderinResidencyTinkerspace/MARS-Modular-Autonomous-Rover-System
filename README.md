# MARS — Modular Autonomous Rover System

## Overview

MARS (Modular Autonomous Rover System) is a modular robotic platform designed to perform different tasks using a single rover with interchangeable application modules.

The base rover supports wireless control, obstacle detection, and autonomous movement. Additional modules provide live video streaming and environmental monitoring.

## Features

- Autonomous movement and obstacle detection
- Bluetooth-based wireless control
- Modular design for different applications
- Raspberry Pi-based live video streaming
- Environmental monitoring using multiple sensors
- 3D-printed chassis and permanent circuit integration

## System Architecture

MARS consists of three main parts:

1. **Base Rover:** Handles movement, obstacle detection, and control.
2. **Camera Module:** Uses a Raspberry Pi and webcam for live video streaming.
3. **Environmental Monitoring Module:** Uses sensors to measure gas levels, soil moisture, temperature, and humidity.

## Hardware Components

| Module | Components |
|---|---|
| Base Rover | Arduino Uno, DC geared motors, motor driver, ultrasonic sensors, Bluetooth module, battery, buck converter |
| Camera Module | Raspberry Pi, webcam |
| Environmental Module | Arduino Nano, gas sensor, soil moisture sensor, temperature and humidity sensor, servo motor |

## Development

The project progressed through the following stages:

- Initial prototype using a foam-board chassis
- Motor control and obstacle detection
- Wireless communication using Bluetooth
- Autonomous movement experiments
- CAD modelling and 3D-printed chassis development
- Permanent circuit assembly using perfboard
- Raspberry Pi camera integration
- Environmental monitoring module development

The rover initially used an ESP32-S3 for Wi-Fi control. After hardware failure, the system was adapted to an Arduino Uno with Bluetooth-based control.

## Technologies Used

- Arduino Uno and Arduino Nano
- ESP32-S3
- Raspberry Pi
- Embedded C/C++
- Bluetooth and Wi-Fi communication
- CAD modelling and 3D printing
- Sensor interfacing and motor control

## Future Improvements

- Improved autonomous navigation and mapping
- GPS-based outdoor navigation
- Wireless transmission of sensor data
- Additional application modules
- Computer vision integration
- Battery monitoring and remote dashboard

## Project Goal

MARS aims to provide a flexible robotic platform that can be adapted for different applications by changing its modules instead of building a separate robot for every task.
