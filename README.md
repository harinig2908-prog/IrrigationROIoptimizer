# 🌱 Irrigation ROI Optimizer

> A smart irrigation monitoring system using Arduino Uno and a rain sensor to reduce unnecessary irrigation and water wastage.

## 📌 Overview

The **Irrigation ROI Optimizer** is an Arduino-based smart agriculture project that detects rainfall and alerts the user using a buzzer.

The system helps prevent unnecessary irrigation when rain is detected, which can reduce water wastage, energy consumption, and irrigation costs.

## 🎯 Problem Statement

Traditional irrigation systems may continue watering crops even during rainfall. This can result in:

- Water wastage
- Unnecessary electricity consumption
- Increased irrigation costs
- Overwatering
- Reduced irrigation efficiency

## 💡 Solution

The project uses a **rain sensor** connected to an **Arduino Uno**.

When rainfall is detected:

**Rain Sensor → Arduino Uno → Buzzer → User Alert**

The alert can be used to prevent unnecessary irrigation during rainfall.

## ⚙️ Working

1. The rain sensor monitors the environment.
2. The sensor sends the rainfall condition to the Arduino Uno.
3. Arduino processes the sensor reading.
4. If rain is detected, the buzzer turns ON.
5. If no rain is detected, the buzzer remains OFF.
6. The process continuously repeats.

## 🔧 Components

- Arduino Uno
- Rain Sensor
- Buzzer
- Breadboard
- Jumper Wires
- USB Cable

## 🔌 Circuit Connections

### Rain Sensor

| Rain Sensor | Arduino Uno |
|-------------|-------------|
| VCC | 5V |
| GND | GND |
| AO | A0 |

### Buzzer

| Buzzer | Arduino Uno |
|--------|-------------|
| Positive (+) | D8 |
| Negative (-) | GND |

## 🧠 Algorithm

```text
START
  ↓
Initialize Arduino
  ↓
Initialize Rain Sensor
  ↓
Initialize Buzzer
  ↓
Read Rain Sensor
  ↓
Is Rain Detected?
  ├── YES → Buzzer ON
  │
  └── NO → Buzzer OFF
  ↓
Repeat
