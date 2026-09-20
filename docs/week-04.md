# Week 4: Moving Towards Autonomous Navigation

After giving MARS wireless control and basic obstacle detection in Week 3, the next goal was to make the rover **operate more autonomously**. We wanted it to not only detect obstacles but also move between different points without continuous manual control.

## Developing Obstacle Avoidance

Initially, we planned to place three ultrasonic sensors at the **front, left, and right** sides of the rover so that it could detect obstacles from multiple directions.

However, during testing, this arrangement did not provide reliable obstacle avoidance. The rover did not always respond as expected, which showed that the sensor arrangement needed to be reconsidered.

After testing different configurations, we decided to place **all three ultrasonic sensors at the front**. This provided better coverage in the direction of movement and was more suitable for our current obstacle avoidance approach.

## Planning Point-to-Point Movement

We also started working towards a system that could allow the rover to move from one location to another without continuous manual control.

Our approach was to combine **path following with obstacle avoidance**. The idea was for the rover to follow a predefined path while using ultrasonic sensors to detect and respond to obstacles.

To plan this system, we measured the **room dimensions and the intended testing path**. These measurements helped us understand the environment in which the rover would operate.
- <img width="357" height="432" alt="image" src="https://github.com/user-attachments/assets/608b7893-432e-472e-96f1-7d55b7b52be6" />

## Fixing the Wheel Problem

We also returned to the wheel connection problem from the previous week. After making the necessary adjustments, the wheels were properly attached to the motors, allowing the rover to move correctly.

This removed one of the major mechanical issues and allowed us to focus more on autonomous navigation.

## Next Steps

By the end of the week, we had a better understanding of the limitations of our initial sensor arrangement and had established a direction for autonomous movement.

The next stage would focus on:

* Developing the path-following system.
* Integrating path following with obstacle avoidance.
* Testing point-to-point movement.
* Further improving the three-front-ultrasonic configuration.

The rover was gradually moving from being **remotely controlled to making movement decisions based on its environment**.





