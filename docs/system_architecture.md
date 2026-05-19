# 🛰 System Architecture — Astrix CanSat

---

# 📌 Overview

The Astrix CanSat system was designed as a compact aerospace telemetry platform capable of collecting environmental data, processing sensor inputs, transmitting telemetry wirelessly, and logging mission data onboard.

The architecture integrates embedded electronics, communication systems, environmental sensing, power management, and ground station monitoring into a unified mission platform.

---

# 🧠 System Architecture Overview

The CanSat architecture consists of the following major subsystems:

- Embedded Processing Unit
- Sensor Subsystem
- Communication Subsystem
- Power Management System
- Data Logging System
- Ground Station System
- Recovery System

---

# ⚙️ Embedded Processing Unit

The embedded controller acts as the central processing system responsible for:

- Reading sensor data
- Processing telemetry packets
- Managing communication
- Logging mission data
- Monitoring battery status
- Coordinating subsystem operation

## Responsibilities

- Sensor acquisition
- Telemetry formatting
- Serial communication
- SD card management
- Real-time processing
- Ground station synchronization

---

# 🌡 Sensor Subsystem

The sensor subsystem was designed to collect atmospheric and motion-related telemetry data during flight.

## Sensor Parameters

| Parameter | Purpose |
|---|---|
| Temperature | Environmental monitoring |
| Humidity | Atmospheric analysis |
| Pressure | Altitude estimation |
| GPS Coordinates | Real-time tracking |
| IMU Data | Motion and orientation |
| Battery Voltage | Power monitoring |
| RSSI | Communication quality |

---

# 📡 Communication Subsystem

The communication system uses Zigbee-based wireless telemetry transmission.

## Objectives

- Continuous telemetry transmission
- Reliable communication during descent
- Real-time data reception
- Packet integrity monitoring
- RSSI analysis

## Communication Flow

```text
Sensors → ESP32 → Telemetry Encoding → Zigbee Transmission → Ground Station Receiver
```

---

# 💾 Data Logging System

The CanSat includes onboard telemetry logging using an SD card module.

## Logging Features

- CSV telemetry storage
- Real-time packet logging
- Backup mission recording
- Post-flight analysis support

## Logged Parameters

- Environmental data
- GPS data
- IMU values
- Battery status
- RSSI values
- Mission timestamps

---

# 🔋 Power Management System

The power subsystem was designed to ensure stable operation throughout the mission.

## Features

- Battery voltage monitoring
- Power regulation
- Electrical insulation
- Short-circuit protection
- Secure battery mounting

---

# 🪂 Recovery System

The recovery system was designed for controlled descent and payload protection.

## Recovery Objectives

- Stable parachute deployment
- Reduced landing impact
- Structural protection
- Safe payload recovery

---

# 🖥 Ground Station System

The ground station acts as the mission monitoring interface.

## Ground Station Features

- Real-time telemetry display
- Live sensor graphs
- RSSI monitoring
- Battery alerts
- Telemetry CSV logging
- Camera feed visualization

---

# 📊 Telemetry Flow Architecture

```text
[ Sensors ]
     ↓
[ ESP32 Controller ]
     ↓
[ Telemetry Packet Generation ]
     ↓
[ Zigbee Transmission ]
     ↓
[ Ground Station Receiver ]
     ↓
[ Real-Time Visualization ]
     ↓
[ CSV Logging ]
```

---

# 🧪 System Testing Objectives

The system architecture was validated through:

- Sensor testing
- Communication testing
- Telemetry verification
- Power stability testing
- Ground station validation
- Structural testing

---

# 🚀 Engineering Highlights

- Aerospace-inspired subsystem architecture
- Embedded telemetry processing
- Real-time communication system
- Integrated data logging
- Ground station visualization
- Compact mission-oriented design

---

# 📄 Competition Reference

The architecture design was developed according to the official CanSat mission requirements and telemetry specifications provided by Presidency University, Bengaluru. :contentReference[oaicite:0]{index=0}
