# 🔥 Autonomous Fire-Fighting Robot

An **Arduino-based autonomous robotics project** designed to detect a flame, navigate toward its direction, align an extinguishing mechanism, and activate a water pump when the target is confirmed at close range.

The project combines embedded programming, sensor-driven decision logic, motor control, and mechanical actuation.

## 🎯 System Objective

The robot demonstrates a simple autonomous perception-and-action loop:

**Flame Detection → Direction Estimation → Robot Navigation → Close-Range Verification → Nozzle Alignment → Pump Activation**

## ⚙️ Main Capabilities

- **Multi-direction flame detection** using a three-sensor array.
- **Autonomous navigation** based on relative flame-sensor readings.
- **Close-range verification** using a dedicated fourth flame sensor.
- **Motor control** through an L298N driver and four DC motors.
- **Servo-controlled extinguishing mechanism** for nozzle positioning.
- **Automatic pump activation** after the fire condition is confirmed.

## 🔩 Hardware

| Component | Role |
| --- | --- |
| Arduino Nano / Uno | Main controller |
| 4× IR flame sensors | Fire detection and verification |
| L298N motor driver | DC motor control |
| 4× DC motors | Robot movement |
| 2× SG90 servo motors | Extinguishing mechanism positioning |
| Water pump + relay | Fire-extinguishing action |
| 12V Li-ion battery | System power |

## 💻 Embedded Logic

The controller is programmed in **C++ using the Arduino environment**.

The navigation logic compares the left, front, and right flame-sensor readings to decide whether the robot should move forward or correct its direction.

A separate verification sensor and `FIRE_PUMP_THRESHOLD` are used before activating the pump, helping prevent the extinguishing mechanism from triggering before the robot is sufficiently aligned with the detected flame.

## 🧠 Engineering Concepts Demonstrated

- Sensor-based autonomous decision making
- Embedded C++ programming
- DC motor control
- Servo control
- Threshold-based sensing
- Robotics integration
- Hardware/software coordination

## 🧪 Testing

The robot is intended to be tested only with a **small, controlled flame source** and appropriate supervision. The project is an educational robotics prototype, not certified fire-safety equipment.

## 👥 Project Context

Developed by **Abdulrahman Mohamed** as part of the Robotics course at the College of Information Technology, **Misr University for Science & Technology (MUST)**.

Supervised by **Dr. Mohammed Abdelrahman Marey**.

---

> **Safety note:** This is an educational prototype and must not be relied upon for real-world fire protection or emergency response.
