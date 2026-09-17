# Week 5

**Goal this week:**  Replace the damaged ESP32-S3, adapt the rover to a new controller, and continue testing the base rover movement and control system.

## What we did

- This week, we changed the battery to a *14.8 V battery*. While testing the motor driver, we noticed that both channels of the motor driver were not receiving equal voltage, so we started troubleshooting and testing the motor driver to identify the issue.
- During the testing, the ESP32-S3 was connected to the battery, and a short circuit occurred while we were testing the motor driver. As a result, the ESP32-S3 was damaged. This became a major problem because we needed to select another suitable controller for the project.
- After considering the available options, we decided to move forward with an Arduino Uno. Since the Arduino Uno was different from the ESP32-S3, we had to change the complete wiring, code and other connections to adapt the rover to the new controller.
- Another problem was that the Arduino Uno does not have an inbuilt Wi-Fi module, so we could not continue using the previous Wi-Fi-based local host control system. Instead, we decided to control the robot using Bluetooth. We used a Bluetooth Serial Terminal app to send movement commands to the robot.
- After completing the wiring and modifying the code, we tested the rover using Bluetooth control. The robot was able to respond to the commands and the basic remote-controlled movement was working well. At this stage, we had not yet integrated the ultrasonic sensors with the Arduino Uno for autonomous obstacle avoidance.
<img width="561" height="483" alt="image" src="https://github.com/user-attachments/assets/d66237ea-5e6d-4bf3-9e93-fe8a31e4d51a" />

<img width="780" height="571" alt="image" src="https://github.com/user-attachments/assets/e156726e-c153-436b-a06b-38b1591a3fd7" />

<img width="1265" height="637" alt="image" src="https://github.com/user-attachments/assets/f88efc22-1a6c-4351-afd2-f3f24ecd5091" />



## Problems and blockers

- The two channels of the motor driver were not receiving equal voltage during testing.
The ESP32-S3 was damaged due to a short circuit while testing the motor driver with the battery connected.
The Arduino Uno did not have an inbuilt Wi-Fi module, so the previous local-host control system could not be used.
The complete wiring and code had to be changed to adapt the rover to the Arduino Uno.
The ultrasonic sensors had not yet been integrated for autonomous operation.

## Decisions

- We decided to replace the damaged ESP32-S3 with an *Arduino Uno*.
We decided to use *Bluetooth communication* instead of Wi-Fi for remote control.
We decided to use the *Bluetooth Serial Terminal app* to control the rover.
We decided to first make the remote-controlled system stable before integrating autonomous obstacle avoidance.

## Next week

- Integrate the ultrasonic sensors with the Arduino Uno.
Start implementing autonomous obstacle avoidance.
Test the ultrasonic sensors with the rover during movement.
Continue improving the remote-control system.
Work towards combining remote control and autonomous operation.

## Links

- Photos
  <img width="716" height="1600" alt="image" src="https://github.com/user-attachments/assets/b9a1421d-0649-4b42-be84-4d5a7e79cfa1" />
<img width="717" height="1600" alt="image" src="https://github.com/user-attachments/assets/9c93b243-d13b-4d2d-a38e-1ab72f38d95e" />
