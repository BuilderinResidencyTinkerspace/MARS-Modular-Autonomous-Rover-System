# Week 6

**Goal this week:** Integrate the ultrasonic sensors with the Arduino Uno, develop autonomous movement and start designing the final CAD structure of the base rover.

## What we did

- This week, after testing the ultrasonic sensors individually, we integrated them with the Arduino Uno and started testing the autonomous movement of the rover. We tested the basic movements including forward, backward, left and right. When an obstacle was detected, the robot stopped and remained in that position until the obstacle moved away, after which it continued moving.
- We arranged the three ultrasonic sensors at the front of the rover in a curved arrangement. The left and right sensors were positioned at approximately +25° and -25°, while the third sensor was placed at the centre. This arrangement was tested to improve the obstacle detection coverage at the front of the rover.
- We then worked on making the robot move from one point to another using a predefined map of the room. We provided the dimensions and layout of the room and tested the robot with commands such as A to B, allowing it to follow the required path. We tested the movement multiple times and made adjustments to achieve the desired movement and positioning.
- Along with the electronics and programming, we started developing the CAD design of the base rover. The base was designed with dimensions of approximately 21 × 18 cm. We included provisions for the battery holder and ultrasonic sensor holders in the design. The top section of the base was also designed to include the module integration area, allowing the different modules to be attached to the rover.
- CAD design was developed using Zoo Keeper and Fusion 360. After checking the dimensions of the different components, we made the necessary corrections to the design and then 3D printed the base and required parts.

  <img width="330" height="462" alt="image" src="https://github.com/user-attachments/assets/71e1ac83-8d89-4def-9ba5-8ee2fa37a069" />
  <img width="662" height="567" alt="image" src="https://github.com/user-attachments/assets/a3a19ccc-3738-48b6-8f43-6b780496f1a4" />



## Problems and blockers

- The robot required multiple tests and adjustments to achieve the desired movement from one point to another.
- The dimensions of the different components had to be considered carefully while designing the CAD model.
- Several corrections were required before the CAD design could be 3D printed properly.

## Decisions

- We decided to use three ultrasonic sensors at the front, with the left and right sensors positioned at approximately *±25°* and one sensor at the centre.
- We decided to use a predefined room map to allow the robot to move from one point to another.
- We decided to include the battery holder, ultrasonic sensor holders and module integration area directly in the CAD design of the base.
- We decided to 3D print the designed parts after making the necessary dimensional corrections.


## Next week

- Continue testing and improving the autonomous movement.
- Test the A-to-B movement more accurately.
- Complete and test the 3D-printed base structure.
- Start working on the module integration mechanism.
- Continue making improvements to the CAD design based on testing.

## Links
- https://zoo.dev/docs/zoo-design-studio/zookeeper
- CAD:
  <img width="1917" height="957" alt="image" src="https://github.com/user-attachments/assets/2ad107c9-df21-47ba-b5d2-684773746ac9" />
