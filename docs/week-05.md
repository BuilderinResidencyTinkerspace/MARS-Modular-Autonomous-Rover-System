# Week 5: Adapting MARS After a Controller Failure

After working towards autonomous navigation in Week 4, this week brought an unexpected setback. A change in the power system led to the failure of the ESP32-S3, forcing us to reconsider the controller and communication system of the rover.

## The Controller Failure

We changed the battery to a **14.8 V battery** and began testing the motor driver. During testing, we noticed that the two motor-driver channels were not receiving equal voltage, so we started troubleshooting the system.

While the battery was connected during this testing, a **short circuit occurred and damaged the ESP32-S3**. Since the controller was an important part of the rover's control system, we needed to find an alternative quickly.

<img width="561" height="483" alt="image" src="https://github.com/user-attachments/assets/d66237ea-5e6d-4bf3-9e93-fe8a31e4d51a" />
## Moving to Arduino Uno

After considering the available options, we decided to replace the ESP32-S3 with an **Arduino Uno**.

However, this was not simply a controller replacement. The change required us to modify the **wiring, code, and communication system** to suit the new controller.

The Arduino Uno also does not have built-in Wi-Fi, so the previous local-host control system could no longer be used. We therefore shifted to **Bluetooth communication**, using a Bluetooth Serial Terminal app to send movement commands to the rover.

```text
Bluetooth Serial Terminal
          ↓
      Bluetooth
          ↓
      Arduino Uno
          ↓
     Motor Driver
          ↓
        Motors
```

## Getting the Rover Moving Again

After rewiring the rover and modifying the code, we tested the Bluetooth-controlled movement.

The rover was able to respond to commands and perform the basic movements successfully. However, the ultrasonic sensors had not yet been integrated with the Arduino Uno, so autonomous obstacle avoidance was temporarily put on hold.

This week showed us that hardware changes can affect the entire system, not just a single component. We had to adapt both the electrical and software sides of MARS to continue development.

## Next Steps

The next stage would focus on:

* Integrating the ultrasonic sensors with the Arduino Uno.
* Implementing autonomous obstacle avoidance.
* Testing the sensors while the rover is moving.
* Improving the Bluetooth control system.
* Working towards combining remote control with autonomous operation.

The main objective was now to **stabilize the new Arduino-based system and continue towards autonomous navigation**.


<img width="780" height="571" alt="image" src="https://github.com/user-attachments/assets/e156726e-c153-436b-a06b-38b1591a3fd7" />

<img width="1265" height="637" alt="image" src="https://github.com/user-attachments/assets/f88efc22-1a6c-4351-afd2-f3f24ecd5091" />


## Links

- Photos
  <img width="716" height="1600" alt="image" src="https://github.com/user-attachments/assets/b9a1421d-0649-4b42-be84-4d5a7e79cfa1" />
<img width="717" height="1600" alt="image" src="https://github.com/user-attachments/assets/9c93b243-d13b-4d2d-a38e-1ab72f38d95e" />
