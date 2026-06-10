# 📊 Bidirectional Visitor Counter using IR Sensors

## 🚀 Overview
This project implements a **Bidirectional Visitor Counter** using two IR sensors and an Arduino. It detects the direction of movement (entry/exit) and maintains:

- 👥 Current number of people inside  
- 📈 Total number of people entered  

### Applications
- Smart classrooms  
- Office occupancy monitoring  
- Retail analytics  
- IoT automation systems  

---

## ⚙️ How It Works
Two IR sensors are placed at a doorway:

- Sensor 1 → Sensor 2 → Person enters  
- Sensor 2 → Sensor 1 → Person exits  

The system detects the **sequence of sensor activation** within a fixed time window to determine direction.

---

## 🧠 Core Logic

Entry:
IR1 → IR2 ⇒ Entry


Exit:
IR2 → IR1 ⇒ Exit


Current Count:
Current = Total Entered - Total Exited

---

## 🔌 Hardware Requirements
- Arduino (Uno / Nano / Mega)
- 2 × IR Sensors (Active LOW)
- Jumper wires
- Breadboard (optional)
- USB cable

---

## 🖥️ Software Requirements
- Arduino IDE

---

## 🔗 Circuit Connections

| Component     | Arduino Pin |
|--------------|------------|
| IR Sensor 1  | D2         |
| IR Sensor 2  | D3         |
| VCC          | 5V         |
| GND          | GND        |

---
