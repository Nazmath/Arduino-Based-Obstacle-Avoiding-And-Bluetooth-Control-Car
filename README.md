# 🤖 Smart Bluetooth-Controlled Obstacle Avoidance Car

This project demonstrates a **smart robotic car** controlled via **Bluetooth (HC-05)** and enhanced with **ultrasonic and IR sensors** for obstacle detection and reverse safety alerts.  
It also includes **horn patterns, headlights, backlights, and buzzer alerts** for a realistic driving experience.  
Built using an **Arduino Uno** and **L298N Motor Driver**, this robot is ideal for IoT and robotics beginners who want to integrate multiple sensors and actuators.

---

## 📜 Table of Contents
- [Features](#-features)
- [Components Used](#-components-used)
- [Pin Connections](#-pin-connections)
- [Working Principle](#-working-principle)
- [Bluetooth Command List](#-bluetooth-command-list)
- [How to Run](#-how-to-run)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## ✨ Features
✔ Control the car via a **Bluetooth app** (forward, reverse, left, right, stop)  
✔ **Ultrasonic sensor** for front obstacle detection (auto-stop)  
✔ **IR sensor** for rear object detection (reverse alerts)  
✔ Automatic **headlights and backlights** with blinking patterns  
✔ **Horn pattern simulation** with buzzer  
✔ Adjustable **speed control** via Bluetooth  
✔ Uses **L298N motor driver** for 2 DC motors  
✔ Neat modular code for easy understanding  

---

## 🔧 Components Used
| Component                     | Quantity |
|-------------------------------|----------|
| Arduino Uno / Nano            | 1        |
| HC-05 Bluetooth Module        | 1        |
| L298N Motor Driver Module     | 1        |
| Ultrasonic Sensor (HC-SR04)   | 1        |
| IR Obstacle Sensor            | 1        |
| DC Motors                     | 2        |
| Robot Car Chassis             | 1        |
| Buzzer                        | 1        |
| LEDs for Headlight/Backlight  | 2+       |
| Battery Pack (7.4V or 9V)     | 1        |
| Jumper Wires, Breadboard      | As needed |

---

## 🛠 Pin Connections
| Component / Signal        | Arduino Pin |
|---------------------------|------------|
| Bluetooth RX/TX           | 2 (TX), 3 (RX) |
| Motor Driver ENA/ENB      | 5, 6       |
| Motor Driver IN1/IN2/IN3/IN4 | 7, 8, 9, 10 |
| Ultrasonic Trigger/Echo   | 12, 11     |
| IR Sensor Signal          | A0         |
| Headlight LED             | 13         |
| Backlight LED             | A1         |
| Buzzer                    | 4          |

---

## ⚙️ Working Principle
1. The robot receives commands via **Bluetooth** from a smartphone app.  
2. It drives forward, backward, left, or right based on user input.  
3. The **ultrasonic sensor** monitors front distance. If an obstacle is too close, the car **automatically stops**.  
4. The **IR sensor** monitors rear objects while reversing and makes the backlight blink faster.  
5. A **buzzer horn pattern** is activated via a command for alerts.  
6. **LED headlights and backlights** simulate a realistic car look.  

---

## 🎮 Bluetooth Command List
| Command | Function               |
|---------|----------------------|
| `F`     | Forward Drive        |
| `B`     | Reverse Drive        |
| `L`     | Turn Left            |
| `R`     | Turn Right           |
| `S`     | Stop Motors          |
| `Y`     | Play Horn Pattern    |
| `X`     | Headlights ON        |
| `x`     | Headlights OFF       |
| `+`     | Increase Speed       |
| `-`     | Decrease Speed       |

---

## ▶️ How to Run
1. **Assemble the robot** as per wiring diagram.  
2. Install the **Arduino IDE** and upload `smart_bluetooth_robot_car.ino` to your board.  
3. Pair your phone with the **HC-05 Bluetooth module** (default password: `1234` or `0000`).  
4. Install a Bluetooth terminal app (like *Arduino Bluetooth Controller*).  
5. Send commands (`F`, `B`, `L`, `R`, etc.) to control the robot.  
6. Test ultrasonic stop and IR reverse alert features.

---

## 🚀 Future Enhancements
- Add **line following mode** or **autonomous navigation**  
- Implement **voice control** via a smartphone app  
- Add **camera streaming** for FPV driving  
- Integrate with **IoT dashboards** for remote monitoring  

---

## 📜 License
This project is open-source for educational purposes.  
You’re free to modify and share it with proper attribution.

---

### 👨‍💻 Author
**NAZMATH PASHA**  
Robotics & Embedded Systems Enthusiast 🚀  
