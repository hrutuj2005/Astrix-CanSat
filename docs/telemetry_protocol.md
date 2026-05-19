# 📡 Telemetry Protocol — Astrix CanSat

---

# 📌 Overview

The Astrix CanSat telemetry system was designed to collect, encode, transmit, receive, and log mission-critical environmental and flight data in real time during aerial deployment and descent.

The telemetry architecture follows the CanSat competition communication and packet requirements defined by Presidency University, Bengaluru.

---

# 🎯 Telemetry Objectives

The telemetry subsystem was designed to:

- Transmit real-time flight data
- Maintain stable wireless communication
- Support ground station visualization
- Log mission data onboard
- Enable post-flight analysis
- Monitor communication quality

---

# 📶 Communication Protocol

## Wireless Communication

The CanSat uses:

- Zigbee-based wireless telemetry communication

## Communication Goals

- Reliable telemetry transmission
- Low packet loss
- Stable signal reception
- Continuous communication during descent

---

# ⏱ Transmission Frequency

Telemetry packets were transmitted at:

```text
1 Hz (1 packet per second)
```

This ensured continuous real-time monitoring throughout the mission.

---

# 📊 Telemetry Parameters

The telemetry system was designed to transmit the following parameters:

| Parameter | Description |
|---|---|
| CanSat ID | Unique mission identifier |
| Mission Time | Mission runtime |
| Packet Number | Packet sequence tracking |
| Temperature | Environmental sensing |
| Pressure | Atmospheric monitoring |
| Humidity | Environmental monitoring |
| Latitude | GPS location |
| Longitude | GPS location |
| Altitude | Flight altitude |
| Battery Percentage | Power monitoring |
| RSSI | Signal strength monitoring |
| Gyroscope Data | Motion sensing |
| Accelerometer Data | Motion analysis |
| Pitch/Roll/Yaw | Orientation tracking |
| Camera Status | Camera monitoring |
| Status Flag | Mission state |

---

# 🧠 Telemetry Packet Structure

The telemetry structure follows the competition telemetry specification.

## Packet Structure

```text
CANSAT_ID,
MISSION_TIME,
PACKET_NO,
TEMPERATURE,
PRESSURE,
HUMIDITY,
SAT_COUNT,
TIMESTAMP,
LATITUDE,
LONGITUDE,
ALTITUDE,
BATTERY_PERCENT,
GYRO_X,
GYRO_Y,
GYRO_Z,
ACCEL_X,
ACCEL_Y,
ACCEL_Z,
PITCH,
ROLL,
YAW,
CAMERA_STATUS,
STATUS_FLAG,
RSSI
```

---

# 💾 Telemetry Logging

The CanSat stores telemetry data onboard using an SD card module.

## Logging Features

- CSV-based storage
- Real-time packet logging
- Backup mission recording
- Post-flight telemetry analysis

## Log File Format

```text
telemetry.csv
```

---

# 🖥 Ground Station Integration

The ground station subsystem was designed to:

- Receive telemetry packets
- Decode incoming data
- Display real-time sensor values
- Plot live telemetry graphs
- Monitor RSSI strength
- Store received CSV logs

---

# 📈 Real-Time Visualization

The telemetry system supports real-time monitoring of:

- Temperature
- Humidity
- Pressure
- Altitude
- Battery status
- RSSI values

---

# 📶 RSSI Monitoring

RSSI monitoring was included to evaluate communication quality during descent.

## Objectives

- Signal quality analysis
- Packet integrity monitoring
- Communication stability testing

---

# 🧪 Telemetry Testing

The telemetry subsystem was validated through:

- Packet transmission testing
- Ground station reception testing
- CSV logging verification
- Communication stability analysis
- Sensor data validation

---

# 🚀 Engineering Highlights

- Real-time telemetry architecture
- Embedded wireless communication
- Aerospace-inspired packet formatting
- Reliable onboard logging
- Ground station visualization
- Signal quality monitoring

---

# 📄 Competition Reference

The telemetry protocol was designed according to the official CanSat telemetry requirements and packet specifications provided by Presidency University, Bengaluru. :contentReference[oaicite:1]{index=1}
