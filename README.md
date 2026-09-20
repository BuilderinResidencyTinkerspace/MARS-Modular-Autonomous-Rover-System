# MARS — Modular Autonomous Rover System 🤖

> **One rover. Multiple capabilities.**

MARS (**Modular Autonomous Rover System**) is a modular robotic platform developed to explore how a single autonomous rover can be adapted for different real-world applications through interchangeable modules.

The project started with a simple question:

> **Instead of building a different robot for every task, can one rover be designed to perform multiple tasks by changing its module?**

This idea led to the development of a common rover base with autonomous movement, obstacle detection, wireless control, and interchangeable application-specific modules.

---

## 🚀 Project Overview

MARS consists of two main parts:

```text
                 ┌──────────────────────┐
                 │      MARS BASE       │
                 │      ROVER           │
                 │                      │
                 │ • Autonomous Motion  │
                 │ • Obstacle Detection │
                 │ • Wireless Control   │
                 │ • Modular Interface  │
                 └──────────┬───────────┘
                            │
             ┌──────────────┴──────────────┐
             │                             │
             ▼                             ▼
   ┌───────────────────┐       ┌────────────────────┐
   │ Raspberry Pi      │       │ Environmental      │
   │ Camera Module     │       │ Monitoring Module  │
   │                   │       │                    │
   │ • Webcam          │       │ • Gas Sensor       │
   │ • Live Streaming  │       │ • Soil Moisture    │
   │                   │       │ • Temperature      │
   └───────────────────┘       │ • Humidity         │
                               │ • Servo Mechanism  │
                               └────────────────────┘
```

The **base rover** provides mobility and autonomous navigation, while application-specific modules extend its functionality.

---

## 🎯 Objectives

The main objectives of MARS are:

* Develop a functional autonomous rover platform.
* Implement obstacle detection and avoidance.
* Enable wireless control of the rover.
* Develop a modular mechanism for attaching different application modules.
* Explore Raspberry Pi-based vision and remote monitoring.
* Develop an environmental sensing module.
* Integrate mechanical, electronic, and software systems into a single platform.
* Create a flexible platform that can be adapted for different field applications.

---

## 🛠️ Hardware

### Base Rover

| Component                 | Purpose              |
| ------------------------- | -------------------- |
| Arduino Uno               | Main controller      |
| DC Geared Motors          | Rover movement       |
| Motor Driver              | Motor control        |
| 14.8 V Battery            | Main power source    |
| Buck Converter            | Voltage regulation   |
| Ultrasonic Sensors        | Obstacle detection   |
| Bluetooth Module          | Wireless control     |
| 65 mm Universal Hub Tyres | Rover movement       |
| Perfboard                 | Permanent circuit    |
| 3D-Printed Chassis        | Mechanical structure |

### Camera Module

| Component    | Purpose                  |
| ------------ | ------------------------ |
| Raspberry Pi | Processing and streaming |
| Webcam       | Live video capture       |

### Environmental Monitoring Module

| Component                     | Purpose                                |
| ----------------------------- | -------------------------------------- |
| Arduino Nano                  | Module controller                      |
| Gas Sensor                    | Gas detection                          |
| Soil Moisture Sensor          | Soil moisture measurement              |
| Temperature & Humidity Sensor | Environmental monitoring               |
| Servo Motor                   | Raises/lowers the soil moisture sensor |

---

## ⚙️ Base Rover

The base rover went through several stages of development.

### 1. Initial Prototype

The first prototype was built using a temporary foam-board base. This allowed the basic components and movement system to be tested before developing the final mechanical structure.

### 2. Controller and Communication

The project initially used an **ESP32-S3** because of its built-in Wi-Fi capability.

During testing, the ESP32-S3 was damaged following a short circuit. We then adapted the rover to an **Arduino Uno**.

Since the Arduino Uno does not have built-in Wi-Fi, the communication system was changed from Wi-Fi-based control to **Bluetooth control**.

```text
Bluetooth Serial Terminal
            ↓
      Bluetooth Module
            ↓
        Arduino Uno
            ↓
       Motor Driver
            ↓
          Motors
```

### 3. Obstacle Detection

Three ultrasonic sensors were used at the front of the rover.

The sensors were arranged approximately as:

```text
             Front
               ↑

       \       |       /
        \      |      /
       +25°   0°   -25°

       Ultrasonic Sensors
```

This arrangement was tested to improve obstacle detection coverage in the direction of movement.

### 4. Autonomous Movement

The rover was developed to:

* Move forward
* Move backward
* Turn left
* Turn right
* Stop when an obstacle is detected
* Continue movement after the obstacle is removed

We also experimented with **point-to-point movement using a predefined room map**, testing movements such as A → B.

---

## 🔧 Mechanical Development

The mechanical structure evolved throughout the project.

The initial prototype used a **30 × 30 cm foam-board base**. Later, a more compact 3D-printed structure was developed with approximate dimensions of **21 × 18 cm**.

The CAD structure included provisions for:

* Battery mounting
* Ultrasonic sensor mounting
* Electronic component placement
* Module integration

The design was developed using **Zoo Keeper and Fusion 360**, followed by 3D printing and physical testing.

---

## 🔌 Electrical Development

The rover initially used a breadboard for temporary connections.

As the design became more stable, the circuit was transferred to a **perfboard**.

```text
Breadboard Prototype
        ↓
Component Testing
        ↓
Circuit Verification
        ↓
Perfboard
        ↓
Soldering & Wiring
        ↓
3D-Printed Integration
```

The permanent circuit contains the main control, communication, sensing, motor-control, and power-regulation components.

---

# 🧩 Application Modules

The modular architecture is the main concept behind MARS.

Instead of modifying the entire rover for every application, different modules can be attached to the same base platform.

## 📷 1. Raspberry Pi Camera Module

A Raspberry Pi and webcam were integrated as a separate module to provide **live video streaming**.

The development involved learning the Raspberry Pi setup process, including:

* Operating system installation
* Initial configuration
* Connecting the Raspberry Pi
* Connecting the webcam
* Network configuration
* Live video streaming

### System Flow

```text
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

This module can be used for applications such as:

* Remote inspection
* Surveillance
* Visual monitoring
* Disaster-area observation

---

## 🌱 2. Environmental Monitoring Module

The second module was developed using an **Arduino Nano**.

It combines multiple sensors to collect environmental information.

### Sensors

* Gas sensor
* Soil moisture sensor
* Temperature sensor
* Humidity sensor

A **servo motor** was also incorporated to mechanically raise and lower the soil-moisture sensor when required.

```text
Gas Sensor ─────────────┐
                        │
Soil Moisture Sensor ───┤
                        │
Temperature/Humidity ───┤
                        ↓
                    Arduino Nano
                        │
                        ↓
                   Sensor Data

                  Servo Motor
                       ↓
          Raise / Lower Moisture Sensor
```

This module demonstrates how MARS can be adapted for environmental monitoring applications.

---

# 📅 Development Timeline

| Week       | Major Development                                                     |
| ---------- | --------------------------------------------------------------------- |
| **Week 0** | MARS concept, system architecture and component planning              |
| **Week 1** | Initial rover prototype and component procurement                     |
| **Week 2** | Component testing, 3D-printing and PCB design learning                |
| **Week 3** | ESP32-S3 integration, Wi-Fi control and obstacle detection            |
| **Week 4** | Autonomous movement experiments and sensor arrangement                |
| **Week 5** | ESP32-S3 failure, Arduino Uno adaptation and Bluetooth control        |
| **Week 6** | Ultrasonic integration, point-to-point navigation and CAD development |
| **Week 7** | New tyres, perfboard conversion and 3D-printed integration            |
| **Week 8** | Permanent electrical system and room-based sensor testing             |
| **Week 9** | Raspberry Pi camera module and environmental monitoring module        |

---

# 🧠 Key Learning

The development of MARS involved learning across multiple areas:

### Electronics

* Motor drivers
* DC motor control
* Ultrasonic sensing
* Voltage regulation
* Battery-powered systems
* Perfboard soldering
* Sensor integration

### Embedded Systems

* Arduino Uno
* Arduino Nano
* ESP32-S3
* Bluetooth communication
* Wi-Fi communication
* Sensor interfacing

### Raspberry Pi

* OS installation
* Initial configuration
* Peripheral connections
* Webcam integration
* Network configuration
* Live video streaming

### Mechanical Design

* CAD modelling
* 3D printing
* Mechanical tolerances
* Component mounting
* Chassis design
* Module integration

### Robotics

* Obstacle detection
* Autonomous movement
* Point-to-point navigation
* Environmental sensing
* Modular robotic architecture

---

# 📂 Repository Structure

```text
MARS-Modular-Autonomous-Rover-System/
│
├── README.md
│
├── docs/
│   ├── week-00.md
│   ├── week-01.md
│   ├── week-02.md
│   ├── week-03.md
│   ├── week-04.md
│   ├── week-05.md
│   ├── week-06.md
│   ├── week-07.md
│   ├── week-08.md
│   └── week-09.md
│
├── code/
│   ├── base-rover/
│   ├── obstacle-avoidance/
│   ├── bluetooth-control/
│   ├── raspberry-pi-camera/
│   └── environmental-module/
│
├── cad/
│   ├── rover-base/
│   └── modules/
│
├── images/
│   ├── base-rover/
│   ├── camera-module/
│   └── environmental-module/
│
└── circuit/
    └── perfboard/
```

---

# 🔮 Future Improvements

Possible future developments for MARS include:

* Improved autonomous navigation
* More accurate mapping
* GPS-based outdoor navigation
* Better obstacle avoidance algorithms
* Wireless sensor-data transmission
* Additional application modules
* Improved modular attachment mechanism
* Battery monitoring
* Remote monitoring dashboard
* Integration of computer vision
* Autonomous task-based module selection

---

# 👥 Project

**MARS — Modular Autonomous Rover System**

Developed as a collaborative engineering project with a focus on **robotics, embedded systems, IoT, mechanical design, and modular architecture**.

The project documentation records the development process, challenges, design decisions, testing, and learning throughout the build.

---

> **MARS is not just a rover. It is a platform designed to become different robots for different tasks.**
