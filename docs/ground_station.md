# 🖥 Ground Station System — Astrix CanSat

---

# 📌 Overview

The Astrix CanSat ground station was designed to receive, decode, visualize, and log telemetry data transmitted from the CanSat during mission deployment and descent.

The ground station acts as the mission monitoring interface, enabling real-time observation of environmental parameters, communication quality, and mission status.

---

# 🎯 Ground Station Objectives

The ground station system was designed to:

- Receive telemetry packets in real time
- Decode incoming sensor data
- Display live mission parameters
- Visualize telemetry graphs
- Monitor communication quality
- Log telemetry data for post-flight analysis

---

# 📡 Communication Interface

The ground station communicates with the CanSat using Zigbee wireless telemetry communication.

## Communication Goals

- Stable telemetry reception
- Low packet loss
- Reliable packet decoding
- Continuous mission monitoring

---

# 📊 Real-Time Telemetry Display

The ground station displays mission-critical telemetry parameters including:

| Parameter | Purpose |
|---|---|
| Temperature | Environmental monitoring |
| Humidity | Atmospheric analysis |
| Pressure | Altitude estimation |
| GPS Coordinates | Real-time tracking |
| Altitude | Flight monitoring |
| Battery Status | Power monitoring |
| RSSI | Signal quality analysis |
| IMU Data | Motion monitoring |

---

# 📈 Live Graph Visualization

The system supports real-time telemetry graph plotting for:

- Temperature
- Humidity
- Pressure
- Altitude
- RSSI
- Battery Percentage

These visualizations improve mission analysis and monitoring during flight.

---

# 💾 Telemetry Logging

The ground station stores received telemetry packets in CSV format for post-flight review and analysis.

## Logging Features

- Real-time packet storage
- Timestamp recording
- CSV export support
- Mission replay capability

## Output File

```text
telemetry.csv
```

---

# 📶 RSSI Monitoring

RSSI monitoring was integrated to evaluate communication stability during mission operation.

## RSSI Objectives

- Signal quality monitoring
- Packet reliability analysis
- Communication diagnostics
- Telemetry stability verification

---

# 🚨 Alert and Monitoring System

The ground station includes monitoring features for mission safety and diagnostics.

## Alerts

- Low battery warning
- Signal loss indication
- Telemetry interruption alerts

---

# 🧠 Ground Station Workflow

```text
Zigbee Receiver
       ↓
Telemetry Packet Reception
       ↓
Packet Decoding
       ↓
Real-Time Visualization
       ↓
Graph Plotting
       ↓
CSV Data Logging
```

---

# 🧪 Ground Station Testing

The ground station subsystem was validated through:

- Telemetry reception testing
- Packet decoding verification
- Live graph testing
- RSSI monitoring validation
- CSV logging verification

---

# 🚀 Engineering Highlights

- Real-time telemetry visualization
- Embedded communication monitoring
- Aerospace-style mission dashboard
- Sensor data visualization
- Communication quality analysis
- Post-flight data logging

---

# 📷 Future Additions

The following visuals will be added:

- Ground station screenshots
- Telemetry graph images
- RSSI monitoring visuals
- Live dashboard images

---

# 📄 Competition Reference

The ground station system was designed according to the telemetry visualization and communication requirements defined by the official CanSat competition guidelines provided by Presidency University, Bengaluru. :contentReference[oaicite:0]{index=0}
