# Week 9: Bringing the Modular Concept to Life

After completing the main base rover and integrating its electrical and mechanical systems, Week 9 was focused on demonstrating what made MARS different from a conventional rover: **the ability to perform different tasks by changing its modules**.

This week, we developed two different modules. The first focused on **remote visual monitoring using a Raspberry Pi and webcam**, while the second was designed for **environmental sensing** using an Arduino Nano.

## Raspberry Pi Camera Module

The first module was built using a **Raspberry Pi and a webcam** to provide the rover with a visual monitoring capability.
<img width="1600" height="717" alt="image" src="https://github.com/user-attachments/assets/efe43574-6a7b-494c-af40-24c63bd44cc5" />

Setting up the Raspberry Pi was itself a learning process. I worked through the process of installing the operating system, configuring the Raspberry Pi, connecting it to the required network, and learning how to interface the webcam with it.

Once the setup was completed, we developed a **live video streaming system**. The webcam connected to the Raspberry Pi could capture video and stream it remotely, allowing the rover to be used for applications such as **remote inspection and surveillance**.

```text id="rpi7m2"
Webcam
   ↓
Raspberry Pi
   ↓
Wi-Fi Network
   ↓
Live Video Stream
   ↓
Remote User
```
<img width="1600" height="717" alt="image" src="https://github.com/user-attachments/assets/3d5074ff-3857-489f-8f7f-8a4f7eb56e0d" />

<img width="716" height="1600" alt="image" src="https://github.com/user-attachments/assets/50ae639f-80b9-4e93-9902-9b0c73d7d3f5" />

Working with the Raspberry Pi also introduced me to a different type of development compared with the Arduino-based rover. From installing the OS and configuring the system to connecting peripherals and setting up the camera, I gained practical experience with the complete setup process.

## Environmental Sensing Module

The second module was designed for **environmental monitoring**.

We used an **Arduino Nano** as the controller and integrated multiple sensors to measure different environmental parameters:

* Gas sensor
* Soil moisture sensor
* Temperature and humidity sensor

  <img width="717" height="1600" alt="image" src="https://github.com/user-attachments/assets/eadb93ee-f043-4618-87e7-5fdb2962388d" />
  <img width="899" height="1599" alt="image" src="https://github.com/user-attachments/assets/9d649021-584d-4daf-85da-54e4e85f1e69" />



This module was intended to allow the rover to collect environmental information while moving through an area.

```text id="7t8k2a"
Gas Sensor ─────────┐
                    │
Soil Moisture ──────┤
                    ↓
Temperature/Humidity → Arduino Nano
                    │
                    ↓
             Sensor Readings
```

## Adding a Servo Mechanism

We also added a **servo motor** to the environmental sensing module.

The servo was used to **raise and lower the soil-moisture sensor when required**. This allowed the sensor to be moved into position for taking measurements and then lifted when it was not needed.

This was an important addition because it demonstrated that a module could contain not only sensors but also **mechanical actuation** for carrying out a specific task.

## The Modular System Takes Shape

With these two modules, the original idea behind MARS became more tangible.

The base rover provided the common mobility platform, while different modules could give it different capabilities.

```text
                 MARS BASE ROVER
                       │
          ┌────────────┴────────────┐
          ↓                         ↓
 Raspberry Pi Camera          Environmental
      Module                     Module
          │                         │
     Live Video              Arduino Nano
     Streaming               ├── Gas Sensor
                             ├── Moisture Sensor
                             ├── Temp/Humidity
                             └── Servo Motor
```

The Raspberry Pi module demonstrated **remote visual monitoring**, while the Arduino Nano module demonstrated **environmental data collection and sensing**.

## Challenges and Learning

The main learning experience this week came from working with hardware that was different from the electronics used in the base rover.

Working with the Raspberry Pi required learning the setup process from the beginning, including **OS installation, configuration, peripheral connections, networking, and camera streaming**.

At the same time, developing the Arduino Nano-based module required integrating several sensors and coordinating them with the servo mechanism.

This week showed us that the modular architecture could actually be used to extend the rover's functionality without redesigning the entire base system.

## Next Steps

With the first two application-specific modules developed, the next focus would be on **testing their integration with the MARS base rover**, improving their physical mounting, and ensuring that the modules can be attached and operated reliably.

Week 9 was therefore a major milestone for MARS: the project had moved beyond simply building an autonomous rover and had started demonstrating the idea of **one common rover platform supporting multiple specialized applications**.
