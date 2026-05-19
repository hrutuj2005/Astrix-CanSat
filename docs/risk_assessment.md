# ⚠️ Risk Assessment — Astrix CanSat

---

# 📌 Overview

This document identifies potential technical, operational, structural, communication, and power-related risks associated with the Astrix CanSat mission.

The objective of the risk assessment process is to improve mission reliability, enhance subsystem safety, and reduce the probability of mission failure during deployment and descent operations.

---

# 🎯 Risk Assessment Objectives

The risk assessment process was designed to:

- Identify mission-critical failure points
- Evaluate subsystem vulnerabilities
- Define mitigation strategies
- Improve operational reliability
- Enhance mission safety

---

# 📡 Communication Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Zigbee signal loss | Loss of telemetry data | Continuous 1 Hz packet transmission |
| Packet corruption | Invalid telemetry | Packet numbering and validation |
| RSSI degradation during rotation | Weak communication | Omnidirectional antenna placement |
| Ground station synchronization failure | Data interruption | Continuous telemetry retry mechanism |

---

# 🔋 Power System Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Battery voltage drop | System instability | INA219 battery monitoring |
| Short circuit | Hardware damage | Insulated wiring and secure mounting |
| Regulator overheating | Power failure | Efficient XY3606 buck converter |
| Excessive current draw | Unexpected shutdown | Power budgeting and subsystem testing |

---

# 🌡 Sensor System Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Sensor calibration drift | Incorrect telemetry | Calibration and validation testing |
| GPS signal loss | Invalid location data | Outdoor GPS acquisition testing |
| IMU noise | Orientation instability | Filtering and averaging methods |
| Sensor communication failure | Missing telemetry fields | Structured error handling |

---

# 💾 Data Logging Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| SD card corruption | Loss of mission data | Real-time CSV logging |
| Write failure | Missing telemetry records | Logging verification routines |
| File formatting error | Competition penalties | Appendix A compliance validation |
| Storage initialization failure | No telemetry archive | Startup validation checks |

---

# 🪂 Recovery System Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Parachute deployment failure | High-speed impact | Servo deployment testing |
| Shroud line tangling | Unstable descent | Multiple deployment validation tests |
| Excessive descent velocity | Payload damage | Descent rate optimization |
| Recovery system misfire | Mission failure | Single-trigger deployment logic |

---

# 🏗 Structural Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Structural deformation | Payload damage | Reinforced cylindrical design |
| Loose electronics | System instability | Secure internal mounting |
| Wiring disconnection | Communication failure | Fixed cable routing |
| Impact shock damage | Mission failure | Internal shock absorption |

---

# 📷 Camera System Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Camera feed interruption | Loss of visual monitoring | ESP32-CAM testing |
| Camera power instability | Video failure | Stable regulated power rail |
| Communication delay | Feed interruption | Lightweight streaming architecture |

---

# 🖥 Ground Station Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Ground station crash | Telemetry interruption | Real-time CSV backup logging |
| Serial communication failure | Data loss | Continuous communication validation |
| Graph rendering delay | Monitoring instability | Optimized real-time plotting |

---

# 🚀 Operational Risks

| Risk | Impact | Mitigation Strategy |
|---|---|---|
| Improper deployment handling | Mission delay | Pre-launch checklist |
| Battery undercharge | Reduced mission runtime | Full battery verification |
| Incorrect subsystem initialization | Startup failure | Structured boot sequence |
| Human operational error | Mission instability | Team role allocation |

---

# 🧪 Validation-Based Risk Reduction

The following tests were conducted to reduce mission risk:

- Structural drop testing
- Zigbee range testing
- Telemetry verification
- SD logging validation
- Parachute deployment testing
- Power stability testing
- Sensor calibration testing

---

# 📊 Risk Management Strategy

The Astrix CanSat system follows a layered risk mitigation strategy:

```text
Subsystem Testing
        ↓
Validation Procedures
        ↓
Failure Detection
        ↓
Redundancy & Monitoring
        ↓
Mission Reliability Improvement
```

---

# 🛰 Engineering Highlights

- Aerospace-oriented risk analysis
- Mission reliability planning
- Embedded subsystem protection
- Communication failure mitigation
- Structured validation procedures
- Operational safety planning

---

# 📄 References

Risk assessment planning was derived using:
- Official CanSat competition requirements provided by Presidency University, Bengaluru :contentReference[oaicite:0]{index=0}
- Astrix CanSat Critical Design Review (CDR) documentation :contentReference[oaicite:1]{index=1}
