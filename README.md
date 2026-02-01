# 🔥 Autonomous Fire-Fighting Robot

An advanced robotics project featuring a mobile robot designed to detect, navigate toward, and extinguish fires automatically using Arduino and embedded sensors.

---

## 🚀 Key Features
- **Autonomous Detection:** Uses a 3-sensor array to scan and locate fire sources in a 180° range.
- **Smart Navigation:** Real-time logic to adjust movement (Forward, Left, Right) based on fire intensity.
- **Precision Extinguishing:** A dedicated 4th sensor on a servo-controlled arm ensures the water pump only activates when directly facing the flame.
- **Dual-Axis Control:** Uses servo motors to adjust the nozzle's angle for effective firefighting.

---

## 🛠️ Hardware Components
- **Microcontroller:** Arduino Nano / Uno.
- **Sensing:** 4x Flame Sensors (Infrared).
- **Actuators:** - L298N Motor Driver + 4x DC Motors.
  - 2x SG90 Servo Motors (Base & Arm).
  - Submersible Water Pump + Relay Module.
- **Power:** 12V Li-ion Battery.

---

## 💻 Software & Logic
The robot's brain is programmed in **C++ (Arduino IDE)**. 
- **Navigation Logic:** Compares values between Left, Front, and Right sensors.
- **Verification Logic:** Uses a `FIRE_PUMP_THRESHOLD` to prevent accidental water spray unless a fire is confirmed at close range.

---

## 📁 Project Structure
- `Code/`: Arduino (.ino) source code for the robot's logic.
- `Documentation/`: Full project report and methodology.
- `Design/`: Circuit diagrams and Fritzing files (`.fzz`).
- `Presentation/`: PowerPoint slides detailing the build and testing phases.

---

## 🔧 Installation & Usage
1. Upload the code provided in `por_code.pdf` (converted to .ino) to your Arduino.
2. Connect the hardware according to the circuit diagram in the `Design` folder.
3. Power the robot and place it in an area with a controlled fire source (e.g., a candle) for testing.

---

## 👥 Project Team
- **Abdulrahman Mohamed**
- **Under supervision of: Dr. Mohammed Abdelrahman Marey**

---

> **Note:** This project was developed as part of the Robotics course at the College of Information Technology, Misr University for Science & Technology (MUST).
