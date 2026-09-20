# Week 8: From a Prototype to a Fully Integrated Rover

After spending the previous weeks developing the rover's mechanical structure and transferring the temporary wiring to a perfboard, Week 8 focused on **testing the permanent electrical system and integrating the complete rover**.

The next challenge was no longer simply getting individual components to work. We needed to make sure that all the components could operate together reliably inside the 3D-printed structure before moving towards mapping and autonomous navigation.

## Finalizing the Electrical System

We started the week by testing the completed **perfboard circuit**. Since the connections were now permanently soldered, each part of the circuit had to be checked carefully to make sure there were no incorrect connections or short circuits.

The perfboard contained the main electronic components of the rover:

* Arduino Uno
* Buck converter
* Bluetooth module
* Ultrasonic sensors
* Motor driver
* Motor connections

After checking the individual connections, we powered the system using the **14.8 V battery** through the required power arrangement.

We then tested the communication between the **Arduino Uno and Bluetooth module**, followed by the motor driver and motors. The rover was able to respond to commands and move correctly with the new permanent wiring.
<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/4f78a7c2-b36a-4362-abb7-6ce342e1b762" />


## Integrating Everything into the 3D-Printed Base

Once the electrical system was verified, we mounted the perfboard and other components inside the **3D-printed rover base**.

This required careful positioning because the available space was limited. The components had to be arranged so that the wiring remained compact while avoiding interference with the mechanical parts of the rover.

The goal was to move away from the earlier breadboard-based prototype and create a more **compact, organized, and reliable base rover**.

```text
14.8 V Battery
       ↓
  Power System
       ↓
  ┌───────────────┐
  │   Perfboard   │
  │               │
  │ Arduino Uno   │
  │ Buck Converter│
  │ Bluetooth     │
  │ Motor Driver  │
  └───────────────┘
       ↓
     Motors

Ultrasonic Sensors
       ↓
   Arduino Uno
```

## Testing the Ultrasonic Sensors in a Real Environment

With the major components integrated, we turned our attention to the **ultrasonic sensors**.

Until this point, much of the sensor testing had been carried out during development. We now needed to understand how the sensors behaved in an actual room environment because their measurements would eventually be used for **mapping and autonomous navigation**.

We placed the rover at different positions and tested the sensors at different distances from walls and other obstacles. We compared the measured distances and observed how the readings changed depending on the sensor's position and the surrounding environment.

This was important because even a small error in distance measurement could affect where the rover believed an obstacle was located. Since the planned mapping system would depend on these measurements, we needed to understand and improve the accuracy before moving forward.
<img width="1600" height="717" alt="image" src="https://github.com/user-attachments/assets/0235e1c4-64c6-4ca7-8d73-1a53db566050" />



## From Testing to Mapping

The room-based testing also helped us identify minor issues with **wiring, sensor positioning, and component placement**. These were corrected before moving towards the mapping stage.

The development process was now becoming clearer:

```text
Component Testing
       ↓
Permanent Perfboard
       ↓
3D-Printed Integration
       ↓
Sensor Calibration
       ↓
Room Testing
       ↓
Mapping
       ↓
Autonomous Navigation
```
<img width="960" height="1280" alt="image" src="https://github.com/user-attachments/assets/3d31a3fc-271c-4c8f-a0b0-f472cfd80183" />
This week therefore represented an important transition. The rover was no longer just a collection of tested components or a temporary prototype. It was becoming a **single integrated platform**, ready for the next stage of autonomous navigation.

## Challenges and Decisions

The main challenges were checking the large

