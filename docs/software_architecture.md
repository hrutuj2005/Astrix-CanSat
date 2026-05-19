# 💻 Software Architecture — Astrix CanSat

---

# 📌 Overview

The Astrix CanSat flight software was developed to manage real-time telemetry acquisition, wireless communication, sensor monitoring, onboard logging, parachute deployment, and mission state management.

The software architecture follows a modular embedded systems design approach optimized for real-time aerospace mission operation.

---

# 🧠 Software Objectives

The flight software was designed to:

- Collect sensor telemetry in real time
- Manage wireless Zigbee communication
- Control parachute deployment
- Log telemetry to SD card
- Maintain mission state transitions
- Support ground station synchronization

---

# ⚙️ Software Platform

| Component | Description |
|---|---|
| Raspberry Pi Pico 2W | Main embedded flight controller |
| Embedded C++ | Primary programming language |
| Arduino Framework | Embedded development framework |

---

# 🛰 Software Architecture Overview

The software architecture is divided into the following modules:

- Sensor Acquisition Module
- Telemetry Processing Module
- Communication Module
- SD Logging Module
- Deployment Control Module
- Ground Station Interface
- Flight State Machine

---

# 🔄 Flight State Machine

The CanSat operates using a structured mission-state architecture.

| State | Purpose |
|---|---|
| BOOT | System initialization |
| READY | Waiting for deployment |
| ASCENT | Pre-release monitoring |
| DESCENT | Free-fall detection |
| DEPLOYED | Parachute deployed |
| LANDED | Mission complete |
| ERROR | Failure handling |

---

# 🚀 Flight Workflow

```text
BOOT
  ↓
READY
  ↓
ASCENT
  ↓
DESCENT
  ↓
DEPLOYED
  ↓
LANDED
```

---

# 🌡 Sensor Acquisition Module

The sensor subsystem continuously collects telemetry from onboard sensors.

## Data Sources

| Sensor | Data Collected |
|---|---|
| BME688 | Temperature, Pressure, Humidity |
| BMI270 | Gyroscope, Accelerometer |
| BMM150 | Magnetometer |
| NEO-6M GPS | GPS coordinates and time |
| INA219 | Battery monitoring |

---

# 📡 Telemetry Processing Module

Telemetry data is formatted into competition-compliant packets before transmission.

## Responsibilities

- Packet formatting
- Packet numbering
- Timestamp generation
- CSV serialization
- Data synchronization

---

# 📶 Communication Module

The communication subsystem handles Zigbee telemetry transmission.

## Features

- 1 Hz telemetry transmission
- Packet integrity handling
- RSSI monitoring
- Ground station synchronization

---

# 💾 SD Logging Module

Telemetry data is simultaneously stored onboard.

## Logging Features

- CSV file generation
- Real-time logging
- Backup mission recording
- Telemetry archive generation

## Output File

```text
telemetry.csv
```

---

# 🪂 Deployment Control Module

The deployment subsystem autonomously controls parachute deployment.

## Deployment Logic

- Free-fall detection
- Acceleration threshold analysis
- Servo actuation
- Single-trigger protection

---

# 📷 Camera Control System

The ESP32-CAM subsystem supports live video feed monitoring.

## Camera Objectives

- Live mission monitoring
- Camera status telemetry
- Ground station integration

---

# 🧪 Timing Architecture

The software uses a non-blocking timing structure.

## Features

- millis()-based scheduling
- Independent subsystem updates
- Real-time execution
- Stable telemetry intervals

---

# 📊 Telemetry Packet Structure

The software generates telemetry packets containing:

- Environmental data
- GPS data
- IMU data
- Battery status
- RSSI values
- Mission state information

---

# 🖥 Ground Station Synchronization

The software continuously synchronizes telemetry with the ground station.

## Ground Station Features

- Real-time data display
- Live graph plotting
- RSSI monitoring
- CSV logging
- Alert generation

---

# 🚨 Error Handling

The software includes error-management mechanisms for:

- Sensor failures
- Communication loss
- SD card errors
- GPS signal loss
- Deployment faults

---

# ⚡ Engineering Highlights

- Real-time embedded architecture
- Aerospace-style mission states
- Non-blocking telemetry system
- Autonomous deployment logic
- Integrated telemetry logging
- Ground station synchronization

---

# 📄 Design Reference

The software architecture and mission-state implementation were derived from the Astrix CanSat Critical Design Review (CDR). :contentReference[oaicite:1]{index=1}
