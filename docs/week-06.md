# Week 6: Autonomous Movement and the First CAD Structure

After adapting the rover to the Arduino Uno in Week 5, this week we focused on **autonomous movement** and began developing the final mechanical structure of the base rover.

## Developing Autonomous Movement

We integrated the three ultrasonic sensors with the Arduino Uno and tested the rover's basic movements: **forward, backward, left, and right**.

When an obstacle was detected, the rover stopped and remained stationary until the obstacle moved away. It could then continue its movement.

To improve the detection coverage, the three ultrasonic sensors were arranged at the front in a curved configuration. The left and right sensors were positioned at approximately **+25° and -25°**, with the third sensor at the centre.
<img width="330" height="462" alt="image" src="https://github.com/user-attachments/assets/71e1ac83-8d89-4def-9ba5-8ee2fa37a069" />

## Point-to-Point Navigation

We then worked on making the rover move between predefined points using a **map of the testing area**.

After providing the room dimensions and layout, we tested commands such as **A to B** and adjusted the movement several times to achieve the required path and positioning.

This helped us move from simple obstacle detection towards a more structured form of autonomous navigation.

## Developing the CAD Model

Alongside the electronics and programming, we started designing the base rover in **Zoo Keeper and Fusion 360**.

The base was designed at approximately **21 × 18 cm**, with dedicated spaces for:

* Battery holder
* Ultrasonic sensor holders
* Module integration area

After checking the dimensions of the physical components, we made several corrections to ensure that the parts would fit properly. The final design was then **3D printed**.

```text id="x3v8j7"
CAD Design
    ↓
Check Component Dimensions
    ↓
Make Corrections
    ↓
3D Printing
    ↓
Physical Rover Base
```

## Challenges and Next Steps

The main challenges this week were achieving accurate A-to-B movement and ensuring that the CAD dimensions matched the actual components.

By the end of the week, we had a working direction for autonomous movement and a first 3D-printed structure for the base rover.

Next week, we planned to:

* Improve autonomous movement and A-to-B navigation.
* Complete and test the 3D-printed base.
* Begin developing the module integration mechanism.
* Continue refining the CAD design based on testing.

Week 6 marked an important step from a temporary prototype towards a **structured autonomous rover platform**.

  <img width="662" height="567" alt="image" src="https://github.com/user-attachments/assets/a3a19ccc-3738-48b6-8f43-6b780496f1a4" />


## Links
- https://zoo.dev/docs/zoo-design-studio/zookeeper
- CAD:
  <img width="1917" height="957" alt="image" src="https://github.com/user-attachments/assets/2ad107c9-df21-47ba-b5d2-684773746ac9" />
