# Week 2: From Individual Components to an Integrated Design

After building the initial physical base of the rover in Week 1, the next challenge was to make sure that the components we had purchased were actually ready to be integrated. Instead of immediately assembling everything together, we decided to first understand and test each component individually.

At the same time, this week introduced us to an important part of the project that we had not worked with much before: **designing the mechanical and electronic systems that would eventually hold the rover together.**

## Testing the Building Blocks

The main focus of the week was testing the components purchased for the base rover. We tested the major components individually, including the **ESP32-S3, ultrasonic sensors, motor driver, DC motors, buck converter, battery, and other supporting components**.

The purpose of this approach was straightforward: before connecting several components together, we needed to verify that each one was functioning correctly.

This also gave us an opportunity to understand the characteristics and requirements of the individual components. In particular, we spent more time studying the **ESP32-S3**, since it would act as the main controller of the rover.

> **Before integrating the system, we first needed to understand the individual building blocks.**

Testing the components separately would also make future troubleshooting easier. If a problem occurred during integration, we would have a better idea of which components had already been verified and which part of the system needed to be investigated.

<img width="785" height="432" alt="image" src="https://github.com/user-attachments/assets/8c2511e8-0843-464a-bdd9-441f9af4c60e" />

## Learning About 3D Printing

Another important part of this week was learning how 3D printing could be used in the mechanical development of MARS.

We had a discussion with **Kurian, COO of TinkerSpace**, who introduced us to the fundamentals of 3D printing and explained how the design of a part affects the final printed result.

One of the important concepts discussed was **tolerance**.

A dimension specified in a CAD model does not always translate into exactly the same physical dimension after printing. Factors such as the printer, material, layer settings, and design itself can affect the final dimensions.

This was particularly relevant to MARS because we planned to use 3D-printed parts for components such as motor mounts and other mechanical structures. Understanding tolerances at this stage would help us avoid problems when assembling parts later.

## Introduction to PCB Designing

We were also introduced to the basics of **PCB designing**.

Kurian explained the general process of converting an electronic circuit into a PCB and introduced us to **KiCad**, which we decided to use as we progressed with the project.

Until this point, our electronic connections were mainly being considered at the individual component and wiring level. Learning about PCB design helped us start thinking about how these connections could eventually be organized into a more permanent and structured system.

The overall process can be viewed as:

```text
Circuit Idea
     ↓
Schematic
     ↓
PCB Layout
     ↓
Fabrication
     ↓
Physical PCB
```

This became particularly important because the final rover would contain multiple electronic components that would need to communicate and receive power reliably.

## Learning From Existing Projects

During the session, Kurian also shared and explained some of the projects he had previously worked on.

Seeing these projects helped us understand how **electronic, mechanical, and software components come together in practical systems**. It also gave us a better perspective on the design process beyond individual components.

For MARS, this reinforced the importance of considering the complete system rather than developing the electronics, mechanical structure, and software independently.

## The Main Challenges

This week did not involve a major mechanical assembly milestone. Instead, the main challenge was building the knowledge required for the next stage of development.

Some components needed to be tested individually before they could be integrated into the rover. At the same time, we needed to become familiar with PCB design and 3D printing before beginning our own designs.

The concept of **3D-printing tolerances** was particularly important. A mechanical part that looks correct in a CAD model may not fit as expected after printing if manufacturing tolerances are not considered.

Therefore, the testing and learning carried out this week were not separate from the rover development. They were preparation for the integration stage that would follow.

## Decisions Made This Week

Based on the work and discussions during the week, we made several decisions for the next stages of MARS:

* Major components would be **tested individually before integration**.
* **KiCad** would be used for PCB design as the project progressed.
* 3D-printing tolerances would be considered while designing mechanical components.
* The ESP32-S3 would continue to be studied in greater detail to understand its capabilities and requirements.
* Mechanical and electronic design would be developed alongside the physical rover rather than being treated as separate stages.

## What Comes Next

With the individual components being tested and the basics of PCB design and 3D printing understood, the next step was to begin developing the rover's structure around these components.

The plan for the coming week was to:

* Continue developing the base structure of the rover.
* Start designing the motor mounting structure.
* Continue testing and integrating the electronic components.
* Begin the PCB design process using KiCad.
* Improve the mechanical parts based on the results of testing.

Week 2 was therefore less about making MARS perform a new function and more about **preparing the foundation for reliable integration**.

We had started with individual components, but the next challenge was to turn those components into a single working system.


<img width="997" height="502" alt="image" src="https://github.com/user-attachments/assets/746dc957-e593-43fa-b10c-0818d53951ca" />
<img width="867" height="285" alt="image" src="https://github.com/user-attachments/assets/12fec207-55cb-41fb-8195-1314a842c052" />


## Links

-https://learn.pcbcupid.com/documentation/modules/glyph/glyph-esp32s3/glyph-s3-overview
-Photos
<img width="1852" height="858" alt="image" src="https://github.com/user-attachments/assets/e53e0474-4ca3-42de-a1f4-a79061660c8f" />

