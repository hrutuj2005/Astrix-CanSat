# 🔧 Components List — Astrix CanSat

---

# 📌 Overview

This document contains the hardware components used in the Astrix CanSat system along with their subsystem roles and engineering purpose.

The hardware architecture was designed for:
- Real-time telemetry
- Environmental sensing
- Zigbee communication
- Ground station integration
- Autonomous deployment
- Onboard data logging

---

# 🧠 Main Flight Controller

| Component | Purpose |
|---|---|
| Raspberry Pi Pico 2W (RP2350) | Main flight computer responsible for sensor acquisition, telemetry generation, SD logging, and subsystem coordination |

## Key Features

- Dual-core ARM Cortex-M33
- Multiple UART/I2C/SPI interfaces
- Real-time embedded processing
- Low power consumption

---

# 🌡 Sensor Subsystem

| Component | Purpose |
|---|---|
| Arduino Nicla Sense ME | Integrated environmental and motion sensing platform |
| BME688 | Temperature, pressure, humidity sensing |
| BMI270 | Accelerometer and gyroscope sensing |
| BMM150 | Magnetometer and heading support |

## Sensor Functions

- Environmental monitoring
- Altitude estimation
- Motion sensing
- Orientation analysis

---

# 📍 GPS Subsystem

| Component | Purpose |
|---|---|
| NEO-6M GPS Module | Real-time GPS location tracking and timestamp generation |

## GPS Parameters

- Latitude
- Longitude
- Altitude
- Satellite count
- Timestamp

---

# 📡 Communication Subsystem

| Component | Purpose |
|---|---|
| XBee S2 (Zigbee) | Wireless telemetry communication between CanSat and ground station |

## Communication Features

- 2.4 GHz Zigbee communication
- Real-time telemetry transmission
- RSSI monitoring
- 1 Hz packet transmission

---

# 📷 Camera System

| Component | Purpose |
|---|---|
| ESP32-CAM | Live camera feed transmission and visual monitoring |

## Camera Features

- Live video streaming
- Compact embedded design
- Real-time monitoring support

---

# 💾 Data Logging Subsystem

| Component | Purpose |
|---|---|
| Micro SD Card Module | Onboard telemetry logging in CSV format |

## Logging Features

- Real-time CSV storage
- Backup mission recording
- Post-flight analysis support

---

# 🔋 Power Subsystem

| Component | Purpose |
|---|---|
| LiPo 7.4V 850mAh Battery | Primary power source |
| XY3606 Buck Converter | Voltage regulation (7.4V → 5V) |
| INA219 | Battery voltage and current monitoring |
| DPDT Power Switch | External system power control |

## Power Features

- Stable regulated power
- Battery monitoring
- Short-circuit protection
- Power distribution management

---

# 🪂 Recovery System

| Component | Purpose |
|---|---|
| MG90S Servo Motor | Parachute deployment mechanism |
| Parachute System | Controlled descent and payload protection |

## Recovery Features

- Autonomous deployment
- Controlled descent rate
- Structural protection

---

# 🖥 Ground Station Components

| Component | Purpose |
|---|---|
| XBee Receiver Module | Ground telemetry reception |
| USB-to-Serial Adapter | Communication interface |
| Laptop / Ground Station PC | Real-time telemetry visualization |

---

# 📟 Display System

| Component | Purpose |
|---|---|
| OLED Display | Onboard system status display |

---

# 🔌 Communication Interfaces

| Interface | Usage |
|---|---|
| UART | GPS and XBee communication |
| I2C | Sensor and display communication |
| SPI | SD card communication |

---

# 🚀 Engineering Highlights

- Aerospace-inspired embedded architecture
- Real-time telemetry communication
- Integrated environmental sensing
- Autonomous recovery system
- Compact subsystem integration
- Ground station synchronization

---

# 📄 Design Reference

Component selection and subsystem architecture were based on the Astrix CanSat Critical Design Review (CDR). :contentReference[oaicite:1]{index=1}
