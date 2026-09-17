# Week 0

**Goal this week:** Develop an initial concept for a modular autonomous rover platform and evaluate the hardware, software, and mechanical requirements needed to build a functional prototype within the available project duration.

## What we did

- Brainstormed multiple robotics project ideas suitable for the project development period.
- Finalized the initial concept: MARS— a modular autonomous rover system designed as a flexible robotic platform that can be adapted for different real-world applications.
- Identified the main idea of developing a common rover base onto which different application-specific modules could be mounted.
- Considered potential applications for the modular rover, including:

  * Disaster search and assistance
  * Material/package delivery
  * Remote inspection
  * Other field-based robotic applications
* Planned the rover around a common base platform consisting of:

  * Microcontroller
  * DC geared motors
  * Motor driver
  * Battery system
  * Obstacle-detection sensors
  * Chassis
  * Modular mounting system
    
* Initially selected ESP32-S3 as the main controller because of its processing capability, wireless communication features, and suitability for future autonomous and IoT-based features.
* Planned to use ultrasonic sensors for obstacle detection and distance measurement.
* Considered a rechargeable high-voltage battery system for powering the motors and electronics.
* Studied the requirements for integrating:

  * Motor control
  * Obstacle detection
  * Power regulation
  * Autonomous movement
  * Application-specific modules
* Evaluated the feasibility of completing the rover base and selected modules within the project development period.
 <img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/54661693-bd73-4b19-b388-dccaa8869fd1" />



## Problems and blockers

-  The proposed system combines mechanical, electrical, and software components, making integration one of the main challenges.
-  The ESP32-S3 required careful testing because it was planned to act as the main controller for the rover.
-  The power system required consideration because the motor supply voltage is significantly higher than the voltage required by the microcontroller and sensors.
-  A suitable power-regulation system was required to safely supply the low-voltage electronics from the main battery.
-  The modular design introduced additional mechanical considerations, particularly for securely mounting and removing application-specific modules.
-  Autonomous operation requires reliable interaction between:

  * Motor driver
  * Motors
  * Ultrasonic sensors
  * Microcontroller
  * Power supply
* The project timeline required the scope to be controlled carefully so that the base rover could be completed before developing the application modules.

## Decisions

- Finalized the project concept as a modular autonomous rover platform.
- Selected ESP32-S3 as the initial main controller.
- Decided that the rover would have a common base platform that could support multiple interchangeable modules.
- Selected ultrasonic sensors as the initial obstacle-detection method.
- Planned a high-voltage rechargeable battery as the main power source for the rover.
- Planned to use a motor driver to control the DC motors.
- Decided to develop the project in stages:

  1. Base chassis
  2. Motor and base system
  3. Power system
  4. Sensor integration
  5. Basic autonomous movement
  6. Modular interface
  7. Application-specific modules
* Decided to limit the final prototype to two application modules so that the project could be completed and properly tested within the available development period.
* The initial controller and architecture were kept flexible so that hardware changes could be made if required during development.

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/dd2b6b7c-dfd7-498e-a4db-505b5ea45380" />

## Next week

- Begin physical development of the rover base:

  * Fabricate/prepare the chassis
  * Mount the DC motors
  * Install the wheels
  * Position the battery
  * Mount the motor driver
* Begin testing the ESP32-S3 with the motor-control system.
* Test individual motors and verify motor-driver operation.
* Design and implement the power distribution system.
* Test the buck converter for supplying the required voltage to the control electronics.
* Begin testing the ultrasonic sensors.
* Develop basic forward, backward, left, right, and stop motor-control functions.
* Start documenting the hardware connections and system architecture.


## Links

- https://gamma.app/docs/Modular-Autonomous-Rover-System-r9c271r7w8i100q

  <img width="642" height="642" alt="image" src="https://github.com/user-attachments/assets/1a190a96-0a21-4c55-b019-10ec533f2b7c" />

