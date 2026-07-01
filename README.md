# ☀️ Dual Axis Sun Tracking Solar Panel

A Dual Axis Sun Tracking Solar Panel system built using **Arduino Uno**, **Servo Motors**, and **Light Dependent Resistors (LDRs)**. The system automatically tracks the position of the sun throughout the day by adjusting the solar panel in both horizontal and vertical directions, maximizing sunlight exposure and improving energy efficiency.

---

## 📌 Project Overview

Traditional fixed solar panels receive maximum sunlight only for a limited period during the day. This project uses four LDR sensors to detect the direction of the highest light intensity and automatically rotates the solar panel using two servo motors.

The panel continuously follows the sun's movement on both the horizontal (azimuth) and vertical (elevation) axes, increasing the amount of solar energy captured.

---

## ✨ Features

- Dual-axis solar tracking
- Automatic sun detection using four LDR sensors
- Horizontal and vertical movement using servo motors
- Real-time light intensity comparison
- Low-cost Arduino-based implementation
- Energy-efficient tracking algorithm
- Easy to build and modify

---

## 🛠️ Technologies Used

- Arduino Uno
- Embedded C (Arduino IDE)
- Servo Library
- LDR Sensors
- Servo Motors

---

## 🔧 Hardware Requirements

| Component | Quantity |
|----------|----------|
| Arduino Uno | 1 |
| LDR Sensors | 4 |
| Servo Motors (SG90/MG996R) | 2 |
| Solar Panel | 1 |
| Resistors (10kΩ) | 4 |
| Breadboard | 1 |
| Jumper Wires | As Required |
| External Power Supply | Optional |

---

## 🔌 Circuit Connections

### Servo Motors

| Servo | Arduino Pin |
|--------|-------------|
| Horizontal Servo | D10 |
| Vertical Servo | D9 |

### LDR Connections

| LDR Position | Arduino Pin |
|--------------|-------------|
| Top Right | A1 |
| Top Left | A2 |
| Bottom Right | A0 |
| Bottom Left | A3 |

---

## ⚙️ Working Principle

1. Four LDR sensors continuously measure sunlight intensity.
2. The Arduino reads analog values from all four sensors.
3. The average light intensity is calculated for:
   - Top
   - Bottom
   - Left
   - Right
4. If one side receives more sunlight than the opposite side, the corresponding servo motor rotates toward the brighter direction.
5. The process repeats continuously, allowing the solar panel to follow the sun.

---

## 📂 Project Structure

```
Dual-Axis-Solar-Tracker/
│
├── SolarTracker.ino
├── README.md
└── Images/
    ├── CircuitDiagram.png
    ├── Prototype.jpg
    └── Working.jpg
```

---

## 🧠 Algorithm

```
Start

↓

Read all four LDR values

↓

Calculate:
- Average Top
- Average Bottom
- Average Left
- Average Right

↓

Compare Top & Bottom

↓

Move Vertical Servo

↓

Compare Left & Right

↓

Move Horizontal Servo

↓

Repeat
```

---

## 🚀 How to Run

1. Install Arduino IDE.
2. Connect Arduino Uno to your computer.
3. Open the project (`SolarTracker.ino`).
4. Install the **Servo** library (already included in Arduino IDE).
5. Select the correct COM port and Arduino board.
6. Upload the code.
7. Place the solar tracker under sunlight.
8. Observe the panel automatically tracking the sun.

---

## 📷 Project Images

You can add the following images to the repository.

- Prototype
- Circuit Diagram
- Arduino Setup
- Working Demonstration

Example:

```
Images/
    Prototype.jpg
    CircuitDiagram.png
    Working.jpg
```

Then display them using:

```markdown
## Prototype

![Prototype](Images/Prototype.jpg)

## Circuit Diagram

![Circuit](Images/CircuitDiagram.png)
```

---

## 🔮 Future Improvements

- LCD display for angle and light intensity
- IoT monitoring using ESP8266/ESP32
- Solar voltage and current monitoring
- Battery charging system
- MPPT integration
- Weather monitoring sensors
- Automatic night reset
- Mobile application for monitoring

---

## 🎯 Applications

- Solar power plants
- Home rooftop solar systems
- Smart agriculture
- Remote power stations
- Educational projects
- Renewable energy research

---

## 📈 Advantages

- Increased solar energy generation
- Higher efficiency than fixed panels
- Automatic operation
- Low maintenance
- Cost-effective design
- Simple implementation

---

## 👨‍💻 Author

**Deepak Wadgane**

- Java Full Stack Developer
- Computer Engineering Graduate

GitHub: https://github.com/yourusername

LinkedIn: https://www.linkedin.com/in/yourprofile

---

## 📜 License

This project is licensed under the MIT License.

Feel free to use, modify, and contribute to this project.

---

⭐ If you found this project useful, don't forget to give it a **Star** on GitHub!