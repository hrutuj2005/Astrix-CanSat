# 🔌 Pin Configuration — Astrix CanSat

---

# 📌 Overview

This document contains the GPIO assignments and communication interface mapping used in the Astrix CanSat system.

The Raspberry Pi Pico 2W acts as the primary flight controller and interfaces with all onboard subsystems including sensors, GPS, Zigbee telemetry, SD logging, display systems, and parachute deployment hardware.

---

# 🧠 Main Controller

| Component | Description |
|---|---|
| Raspberry Pi Pico 2W (RP2350) | Main flight controller and subsystem coordinator |

---

# 🔌 GPIO Pin Mapping

| GPIO Pin | Connected Peripheral | Interface | Purpose |
|---|---|---|---|
| GPIO 0 | GPS NEO-6M TX/RX | UART0 | GPS communication |
| GPIO 1 | GPS NEO-6M TX/RX | UART0 | GPS communication |
| GPIO 2 | Nicla Sense ME SDA | I2C1 | Sensor communication |
| GPIO 3 | Nicla Sense ME SCL | I2C1 | Sensor communication |
| GPIO 5 | XBee S2 SLEEP_RQ | Digital | Zigbee sleep/wake control |
| GPIO 6 | INA219 SDA | I2C | Battery monitoring |
| GPIO 7 | INA219 SCL | I2C | Battery monitoring |
| GPIO 8 | OLED SDA | I2C0 | Display communication |
| GPIO 9 | OLED SCL | I2C0 | Display communication |
| GPIO 13 | ESP32-CAM | GPIO | Camera interface |
| GPIO 15 | MG90S Servo | PWM | Parachute deployment |
| GPIO 16 | SD Card MISO | SPI0 | SD communication |
| GPIO 17 | SD Card CS | SPI0 | SD communication |
| GPIO 18 | SD Card SCK | SPI0 | SD communication |
| GPIO 19 | SD Card MOSI | SPI0 | SD communication |

---

# 📡 UART Communication

UART communication is used for:

| Device | Usage |
|---|---|
| NEO-6M GPS Module | GPS telemetry and positioning |
| XBee S2 Zigbee Module | Wireless telemetry communication |

---

# 🌡 I2C Communication

I2C communication is used for sensor and monitoring subsystems.

## Connected Devices

| Device | Function |
|---|---|
| Arduino Nicla Sense ME | Environmental and IMU sensing |
| INA219 | Battery voltage/current monitoring |
| OLED Display | System status display |

---

# 💾 SPI Communication

SPI communication is used for onboard telemetry storage.

| Device | Purpose |
|---|---|
| Micro SD Card Module | Real-time CSV telemetry logging |

---

# 🪂 Servo Control Interface

The MG90S servo motor is connected to:

```text
GPIO 15
```

## Servo Responsibilities

- Parachute deployment
- Recovery activation
- Deployment locking mechanism

---

# 📷 Camera Interface

The ESP32-CAM subsystem is connected for live video transmission support.

## Camera Objectives

- Live video feed
- Mission monitoring
- Camera status telemetry

---

# 🔋 Power Distribution Overview

| Voltage Rail | Components |
|---|---|
| +5V Rail | Pico, ESP32-CAM, GPS, SD Module, Servo |
| +3.3V Rail | XBee S2, OLED, INA219 |

---

# 🧠 Communication Architecture

```text
Sensors
   ↓
Raspberry Pi Pico 2W
   ↓
Telemetry Packet Generation
   ↓
XBee S2 Zigbee Transmission
   ↓
Ground Station
```

---

# ⚙️ Embedded System Highlights

- Multi-interface embedded architecture
- UART/I2C/SPI subsystem integration
- Real-time telemetry communication
- Autonomous deployment control
- Aerospace-oriented hardware design

---

# 📄 Design Reference

GPIO assignments and subsystem architecture were derived from the Astrix CanSat Critical Design Review (CDR). :contentReference[oaicite:0]{index=0}
