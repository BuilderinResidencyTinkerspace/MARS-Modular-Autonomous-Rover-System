\# MARS --- Modular Autonomous Rover System 🤖

> **One rover. Multiple capabilities.**

MARS (Modular Autonomous Rover System) is a modular robotics project
that explores how one rover can support different real-world tasks
through interchangeable application modules.

The project combines mobile robotics, embedded systems, electronics,
mechanical design, and remote monitoring.

## Project Overview

MARS has two main parts:

-   **Base Rover:** Provides movement, obstacle detection, wireless
    control, and the interface for attaching modules.
-   **Application Modules:** Add task-specific capabilities, including
    camera-based remote observation and environmental monitoring.

``` text
                         MARS
                          |
             +------------+------------+
             |                         |
       Base Rover                Application Modules
             |                         |
      - Motor control           - Raspberry Pi camera
      - Obstacle detection      - Environmental monitoring
      - Wireless control        - Future modules
      - Modular interface
```

## Main Features

-   Rover movement using DC geared motors
-   Obstacle detection using ultrasonic sensors
-   Wireless control through Bluetooth
-   Modular design for application-specific attachments
-   Raspberry Pi and webcam module for live video streaming
-   Environmental sensing using gas, soil-moisture, temperature, and
    humidity sensors
-   Servo mechanism to raise and lower the soil-moisture sensor

> **Development note:** The ESP32-S3 was considered and tested
> initially. After it was damaged during testing, the base rover was
> adapted to use an Arduino Uno with Bluetooth control.

## Hardware

### Base Rover

  Component                   Purpose
  --------------------------- -------------------------------
  Arduino Uno                 Main rover controller
  DC geared motors            Rover movement
  Motor driver                Motor control
  14.8 V battery              Main power source
  Buck converter              Voltage regulation
  Ultrasonic sensors          Obstacle detection
  Bluetooth module            Wireless control
  65 mm universal hub tyres   Movement
  Perfboard                   Permanent circuit connections
  3D-printed chassis          Mechanical structure

### Raspberry Pi Camera Module

  Component      Purpose
  -------------- --------------------------------
  Raspberry Pi   Processing and video streaming
  Webcam         Live video capture

### Environmental Monitoring Module

  Component                         Purpose
  --------------------------------- --------------------------------------------
  Arduino Nano                      Module controller
  Gas sensor                        Gas detection
  Soil-moisture sensor              Soil-moisture measurement
  Temperature and humidity sensor   Environmental measurements
  Servo motor                       Raises and lowers the soil-moisture sensor

## System Development

The rover was developed through several stages:

1.  Built an initial prototype using a foam-board base.
2.  Tested the motors and basic movement system.
3.  Explored ESP32-S3-based control and obstacle detection.
4.  Adapted the controller to Arduino Uno and changed wireless control
    to Bluetooth.
5.  Integrated three front-facing ultrasonic sensors.
6.  Experimented with autonomous movement and point-to-point navigation.
7.  Designed a more compact chassis and moved from temporary breadboard
    wiring to perfboard.
8.  Developed a Raspberry Pi camera module for live video streaming.
9.  Developed an environmental monitoring module using an Arduino Nano
    and multiple sensors.

The initial foam-board prototype measured approximately 30 × 30 cm. A
later 3D-printed chassis measured approximately 21 × 18 cm. CAD design
and mechanical development used Zoo Keeper and Fusion 360.

## Software and Tools

The project involves:

-   Arduino programming and sensor interfacing
-   Bluetooth serial communication
-   ESP32-S3 and Wi-Fi experimentation
-   Raspberry Pi setup and webcam streaming
-   CAD modelling and 3D printing
-   Circuit assembly, soldering, and testing

## Repository Structure

The following structure is proposed for organising the project files.
Add folders as the corresponding files become available.

``` text
MARS-Modular-Autonomous-Rover-System/
├── README.md
├── docs/
│   ├── week-00.md
│   ├── week-01.md
│   ├── week-02.md
│   └── ...
├── code/
│   ├── base-rover/
│   ├── obstacle-avoidance/
│   ├── bluetooth-control/
│   ├── raspberry-pi-camera/
│   └── environmental-module/
├── cad/
│   ├── rover-base/
│   └── modules/
├── circuit/
└── images/
```

## Development Log

The project is documented week by week, covering design decisions,
implementation, testing, challenges, and lessons learned.

  Week     Focus
  -------- ------------------------------------------------------------
  Week 0   Project concept, architecture, and component planning
  Week 1   Initial prototype and component procurement
  Week 2   Component testing, 3D printing, and PCB design learning
  Week 3   ESP32-S3, Wi-Fi control, and obstacle detection
  Week 4   Autonomous movement experiments and sensor arrangement
  Week 5   Arduino Uno adaptation and Bluetooth control
  Week 6   Ultrasonic integration, point-to-point navigation, and CAD
  Week 7   Tyres, perfboard conversion, and 3D-printed integration
  Week 8   Permanent electrical system and room-based sensor testing
  Week 9   Raspberry Pi camera and environmental monitoring modules

*The timeline summarises the recorded development plan; the individual
weekly reports should contain the detailed progress.*

## Future Improvements

Potential future improvements include:

-   More reliable autonomous navigation and mapping
-   Improved obstacle-avoidance algorithms
-   Wireless transmission of environmental sensor data
-   Battery monitoring
-   A remote monitoring dashboard
-   Additional application modules
-   Improved module mounting and electrical connections
-   Computer-vision integration

These are possible extensions and are not necessarily implemented in the
current version.

## Project Goal

MARS aims to demonstrate how a shared robotic platform can be adapted
for different applications by changing its modules rather than
rebuilding the entire robot.

> **MARS is more than a rover: it is a platform designed to support
> different tasks through modular hardware.**
