# Week 3: Giving MARS Wireless Control and Obstacle Detection

After testing the individual components in Week 2, we began integrating them into the base rover. This week marked an important transition from testing individual parts to making the rover **function as a connected system**.

## Integrating the Rover

We connected the **ESP32-S3, motor driver, DC motors, ultrasonic sensor, and other required components** and started working on the rover's control system.

The ESP32-S3's built-in Wi-Fi was then used to create a **local host interface** through which the rover could be controlled wirelessly. We tested basic movement commands, and the rover was able to move according to the commands sent through the interface.

## Adding Obstacle Detection

We also implemented basic **ultrasonic-based obstacle detection**.

When an obstacle was detected in front of the rover, it would stop and wait until the obstacle was removed before continuing. After testing the system, both the wireless control and basic obstacle detection were functioning as expected.

```text
Wi-Fi Control
      ↓
   ESP32-S3
      ↓
  Motor Driver
      ↓
     Motors

Ultrasonic Sensor
      ↓
   ESP32-S3
      ↓
Obstacle Detected → Stop
```
<img width="287" height="315" alt="image" src="https://github.com/user-attachments/assets/a1d4a005-e2b1-4994-bd00-9947098d4da1" />


## Starting the Mechanical Design

Alongside the electronics, we began planning the mechanical structure of the rover. Before moving into detailed CAD modelling, we created **rough paper sketches** to determine the positioning of the motors, wheels, and other components.

However, we faced a mechanical issue: **the wheels were not attaching properly to the motors**. This meant that the motor and wheel mounting arrangement needed further adjustment before the base structure could be finalized.

<img width="290" height="563" alt="image" src="https://github.com/user-attachments/assets/2e58cbd0-bb6a-4542-b4f8-edab8e3abf1a" />

## Decisions and Next Steps

Based on this week's work, we decided to continue using the **ESP32-S3 Wi-Fi** for wireless control and the local host as the control interface. Ultrasonic-based obstacle detection was also retained as part of the base rover.

For the mechanical design, we planned to improve the motor and wheel mounting and then proceed with the detailed CAD design.

The next stage would focus on **improving the mechanical structure while continuing the integration of the rover's electronics and control system**.



-Photos
<img width="1032" height="560" alt="image" src="https://github.com/user-attachments/assets/6f9b9daa-b97e-46ba-9005-59d4c4cd03de" />

