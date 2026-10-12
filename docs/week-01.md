# Week 1: Turning the MARS Concept into a Physical Rover

Last week, MARS existed mostly as an idea—a modular rover platform designed around a common base that could eventually support different application-specific modules.

This week, the goal was much more straightforward:

**Start building the rover.**

After discussing the project concept and the requirements of the base platform, we moved from planning to the first physical prototype. Before worrying about autonomous navigation or application modules, we needed to establish a stable base on which everything else could be built.

---

## From a Concept to a Chassis

The first task was to create the physical base of the rover.

For the initial prototype, we decided to use **foam board** as the chassis material. It was lightweight, inexpensive, and easy to cut and modify during the early stages of development.

We cut the board to a size of **30 × 30 cm**, giving us a basic platform on which the motors, electronics, battery, and other components could eventually be mounted.

```text
              30 cm
       ┌──────────────────┐
       │                  │
       │    Rover Base    │
       │                  │ 30 cm
       │                  │
       └──────────────────┘
```

The intention was not to create the final mechanical structure immediately. At this stage, the foam-board chassis served as a practical prototype that allowed us to experiment with the component placement and overall dimensions of the rover.

 <img width="1536" height="1536" alt="image" src="https://github.com/user-attachments/assets/16314653-095b-4ba3-b096-2e7062a71f17" />

---

## Getting the Hardware Together

Once the basic chassis was prepared, we began collecting the components required to build the base rover.

The initial hardware included:

| Component              | Purpose                       |
| :--------------------- | :---------------------------- |
| **ESP32-S3**           | Main controller               |
| **DC Motors**          | Drive the rover               |
| **Tyres**              | Provide traction and movement |
| **Motor Driver**       | Control the motors            |
| **Ultrasonic Sensors** | Obstacle detection            |
| **Battery**            | Main power source             |
| **Buck Converter**     | Voltage regulation            |

Having the major components physically available made the project feel significantly different from the previous week. We could now begin thinking about actual component placement, wiring, and mechanical assembly rather than only discussing the architecture.

---

## The Battery Holder Problem

The first practical obstacle appeared before we could even complete the power system.

We were unable to obtain a suitable battery holder for the battery we had selected. Since the rover required a **12 V supply**, we needed a way to establish a reliable connection between the battery and the rest of the system.

Instead of delaying the prototype, we decided to **solder the battery connections directly** to obtain the required power supply.

This allowed us to continue with the initial prototype, although it also highlighted an important consideration for the later stages of development: the final rover would need a safer and more convenient battery connection method.

```text
Battery
   │
   │  Direct soldered connection
   ↓
12 V Supply
   │
   ├────────→ Motor System
   │
   └────────→ Buck Converter
                    │
                    ↓
              Low-voltage electronics
```

The solution was therefore useful for getting the prototype running, but it was treated as a temporary arrangement rather than the final power architecture.

---

## The First Physical Version of MARS

By the end of the week, we had completed the first physical foundation of the rover.
The 30 × 30 cm foam-board base provided the platform for the next stage, while the major electronic and mechanical components had been acquired.


<img width="1536" height="1536" alt="image" src="https://github.com/user-attachments/assets/3b9a8554-cf92-4dcc-9b60-0e179a760614" />

---


## Next Week: Making It Move

With the basic platform and components ready, the next step was to begin assembling the actual drive system.

We planned to mount the **DC motors and tyres**, install the **motor driver and ESP32-S3**, and begin connecting the power system to the rover.


> **Make MARS move forward and backward.**

Once basic motor control was working, we could begin building towards turning, sensor integration, and eventually autonomous movement
Now we needed to make all of them work together.

  <img width="1536" height="1536" alt="image" src="https://github.com/user-attachments/assets/3b9a8554-cf92-4dcc-9b60-0e179a760614" />
  

  



- Photos
 <img width="1536" height="1536" alt="image" src="https://github.com/user-attachments/assets/d3d787ff-0fa6-463f-9a74-fb5e97ffa4fa" />

