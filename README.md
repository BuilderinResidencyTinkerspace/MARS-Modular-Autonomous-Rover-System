# MARS — Modular Autonomous Rover System

**One rover. Multiple capabilities.**

MARS (Modular Autonomous Rover System) is a modular robotic platform designed to perform different tasks using a common rover base and interchangeable application modules.

Instead of building a separate robot for every application, MARS allows different modules to be integrated into a single rover. The current prototype combines mobile movement, obstacle detection, Bluetooth control, live video streaming, and environmental monitoring.

The project explores how modular robotics can make robotic systems more flexible, reusable, and adaptable to real-world applications.

## Table of Contents

- [What is MARS?](#what-is-mars)
- [Key Features](#key-features)
- [Components Used](#components-used)
- [How Does MARS Work?](#how-does-mars-work)
- [Rover Design](#rover-design)
- [Application Modules](#application-modules)
- [Assembly and Integration](#assembly-and-integration)
- [Software and Control](#software-and-control)
- [Development Timeline](#development-timeline)
- [Final Result](#final-result)
- [Challenges and Troubleshooting](#challenges-and-troubleshooting)
- [Future Improvements](#future-improvements)

## What is MARS?

MARS is designed around a simple idea: **one robotic platform can support multiple applications through interchangeable modules.**

The rover provides the basic movement and control system. Additional modules can be attached depending on the task, allowing the same platform to be used for environmental monitoring, remote inspection, live video streaming, and other applications.

This modular approach reduces the need to build separate robots for different purposes.

## Key Features

- **Modular design:** Supports different application-specific modules.
- **Bluetooth control:** Allows wireless control of the rover.
- **Obstacle detection:** Uses ultrasonic sensors to detect nearby obstacles.
- **Live video streaming:** Uses a Raspberry Pi and webcam for remote visual monitoring.
- **Environmental monitoring:** Collects gas, soil-moisture, temperature, and humidity data.
- **3D-printed chassis:** Provides a compact structure for mounting the electronics and modules.
- **Expandable platform:** Can be improved with additional sensors and applications.

## Components Used

The following components form the base rover and its application modules.

### Base Rover

| Component | Purpose |
|---|---|
| Arduino Uno | Main rover controller |
| DC geared motors | Drive the rover |
| Motor driver | Control motor movement |
| Ultrasonic sensors (3) | Detect nearby obstacles |
| Bluetooth module | Wireless control |
| 14.8 V battery | Main power source |
| Buck converter | Provide regulated voltage |
| 65 mm wheels | Rover movement |
| 3D-printed chassis | Support the components |
| Perfboard and wires | Circuit connections |

### Application Modules

| Component | Purpose |
|---|---|
| Raspberry Pi | Process and stream camera data |
| Webcam | Capture live video |
| Arduino Nano | Control the environmental monitoring module |
| Gas sensor | Detect selected gases |
| Soil-moisture sensor | Measure soil moisture |
| Temperature and humidity sensor | Monitor environmental conditions |
| Servo motor | Raise and lower the soil-moisture sensor |

*Component specifications and connections may vary as the prototype develops.*

## How Does MARS Work?

MARS consists of a common rover base and interchangeable application modules.

1. **Movement:** The Arduino Uno controls the DC geared motors through the motor driver.
2. **Obstacle detection:** Three ultrasonic sensors measure the distance to nearby objects.
3. **Wireless control:** Bluetooth allows the rover to receive movement commands.
4. **Module operation:** The selected module performs its specific task independently or alongside the rover.
5. **Data collection:** Sensors or the camera collect information for monitoring and remote observation.

The rover base can be reused while the application module is changed according to the requirement.

## Rover Design

The chassis went through multiple design stages during development.

Initially, a 30 × 30 cm foam-board chassis was used to explore the basic layout. The design was later refined into a compact 3D-printed chassis measuring approximately 21 × 18 cm.

Zoo Keeper and Autodesk Fusion 360 were used during the design process to develop and refine the mechanical structure.

The final design provides mounting space for the motors, wheels, battery, controller, sensors, and application modules.

## Application Modules

### 1. Live Video Streaming Module

This module uses a Raspberry Pi and webcam to capture and stream live video.

**Main functions:**
- Capture live video.
- Support remote visual monitoring.
- Provide visual information from the rover's surroundings.

**Possible applications:** Remote inspection, surveillance, and visual exploration.

### 2. Environmental Monitoring Module

This module uses an Arduino Nano with environmental sensors to collect information about the surrounding environment.

**Main functions:**
- Detect selected gases.
- Measure soil moisture.
- Monitor temperature and humidity.
- Use a servo motor to raise and lower the soil-moisture sensor.

**Possible applications:** Environmental observation, soil monitoring, and basic field data collection.

These modules demonstrate how a single rover platform can be adapted for different tasks without redesigning the entire robot.

## Assembly and Integration

The development process involved both mechanical and electronic integration.

1. Design the chassis and determine the component layout.
2. Mount the DC geared motors and wheels.
3. Install the Arduino Uno, motor driver, battery, and buck converter.
4. Position the ultrasonic sensors for obstacle detection.
5. Establish Bluetooth communication for rover control.
6. Develop the camera and environmental monitoring modules.
7. Integrate the modules with the rover platform.
8. Test movement, sensor readings, wireless communication, and module operation.

Each stage helps identify mechanical, electrical, and software issues before adding more functionality.

## Software and Control

The software is divided according to the responsibilities of the rover and its application modules.

### Rover Control

The Arduino Uno manages motor control and receives wireless movement commands through Bluetooth. The ultrasonic sensors provide distance measurements for obstacle detection.

### Camera Module

The Raspberry Pi handles the webcam and live video streaming functionality.

### Environmental Monitoring Module

The Arduino Nano reads the environmental sensors and controls the servo mechanism used to position the soil-moisture sensor.

The modules are developed separately to simplify testing, debugging, and future upgrades.

## Development Timeline

| Stage | Work Completed |
|---|---|
| Initial concept | Defined the modular rover idea and its applications |
| Base design | Planned the chassis and component arrangement |
| Mechanical development | Built and refined the rover chassis |
| Electronics integration | Integrated the controller, motors, sensors, and power system |
| Wireless control | Developed Bluetooth-based rover control |
| Application modules | Developed the camera and environmental monitoring modules |
| Testing and refinement | Worked on integration, calibration, and system improvements |

## Final Result

MARS demonstrates the concept of a modular rover that can support multiple applications using a shared mobile platform.

The base rover provides movement, wireless control, and obstacle detection. The camera module enables live video streaming, while the environmental module collects sensor data.

The project also provides practical experience in embedded systems, robotics, sensor integration, CAD design, 3D printing, and modular system development.

MARS is an evolving prototype, with further improvements planned for autonomy, integration, and reliability.

## Challenges and Troubleshooting

### Rover does not move

- Check the battery and power connections.
- Verify the motor driver wiring.
- Confirm that the motors and wheels are mounted correctly.

### Bluetooth control does not work

- Check the Bluetooth module connections.
- Verify that the controller is paired with the correct device.
- Check the serial communication settings and control commands.

### Ultrasonic sensors give incorrect readings

- Check the sensor wiring and power supply.
- Ensure the sensors have a clear path to the target.
- Verify the distance-measurement logic.

### Environmental sensor readings are unstable

- Check the sensor connections and supply voltage.
- Allow the sensors to stabilize.
- Calibrate the sensors where necessary.

### Application modules do not work correctly

- Test each module separately before integration.
- Verify its power requirements and communication connections.
- Check the mechanical mounting and cable arrangement.

## Future Improvements

- Implement more advanced autonomous navigation.
- Improve obstacle avoidance and movement control.
- Develop a more standardized module-mounting mechanism.
- Improve power management and battery monitoring.
- Integrate sensor data and live video into a unified interface.
- Add more application modules for inspection, delivery, and environmental monitoring.
- Improve the chassis and electronics for greater reliability.

## Conclusion

MARS explores a practical approach to modular robotics by combining a reusable rover base with interchangeable application modules.

The project demonstrates how embedded systems, sensors, wireless communication, mechanical design, and software can work together to create a flexible robotic platform.

The long-term goal is to develop a rover that can be adapted to different real-world tasks by changing its modules rather than building an entirely new robot each time.
