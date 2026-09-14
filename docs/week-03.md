# Week 3

**Goal this week:** Continue working on the MARS prototype by integrating the base rover components with the ESP32-S3 and developing the basic wireless control and obstacle avoidance system.

## What we did

- This week, we started working on the electrical and control side of the rover. We integrated the main components of the base rover with the *ESP32-S3*, including the motor driver, DC motors, ultrasonic sensor and other required components.

We then connected the rover to the *integrated Wi-Fi module of the ESP32-S3* and created a *local host* through which we could remotely control the movement of the robot. We tested the basic movement commands and the robot was able to move according to the commands given through the local host.

We also implemented *obstacle avoidance* using the ultrasonic sensor. When an obstacle was detected in front of the robot, the robot stopped and waited until the obstacle moved away before continuing its movement. We tested the system and the basic wireless control and obstacle detection were working properly.

Along with the electrical work, we also started planning the mechanical design of the rover. We made a *rough sketch of the CAD design on paper* to get an idea of the structure and positioning of the different components before proceeding with the detailed CAD design.

## Problems and blockers

- The wheels were not attaching properly to the motors.
The mechanical structure needed further improvement before the base could be completed.
We needed to adjust the mechanical design to ensure that the wheels and motors were properly positioned.

## Decisions

- We decided to use the *ESP32-S3 Wi-Fi module* for wireless control of the rover.
We decided to use a *local host* as the interface for controlling the robot's movement.
We decided to include ultrasonic-based obstacle detection so that the robot would stop when an obstacle was detected and continue only after the obstacle moved away.
We decided to make a rough paper sketch before continuing with the detailed CAD design.

## Next week

- We decided to use the *ESP32-S3 Wi-Fi module* for wireless control of the rover.
We decided to use a *local host* as the interface for controlling the robot's movement.
We decided to include ultrasonic-based obstacle detection so that the robot would stop when an obstacle was detected and continue only after the obstacle moved away.
We decided to make a rough paper sketch before continuing with the detailed CAD design.

## Links

- Code:
- Photos / CAD:
