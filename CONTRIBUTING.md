# 🤝 Contributing Guidelines — Astrix CanSat

Thank you for contributing to the Astrix CanSat project.

This repository contains documentation, embedded software, telemetry systems, hardware architecture, and testing procedures developed for aerospace mission simulation and CanSat competition deployment.

---

# 📌 Contribution Objectives

Contributors should focus on improving:

- Embedded software reliability
- Telemetry communication
- Ground station visualization
- Hardware documentation
- Testing procedures
- Mission analysis
- System integration

---

# 📂 Repository Structure

```text
docs/            -> Technical documentation
hardware/        -> Hardware architecture and pin mapping
software/        -> Embedded software documentation
images/          -> Build and testing visuals
data/            -> Telemetry logs and datasets
presentations/   -> PPTs and project presentation files
```

---

# 🧠 Contribution Rules

## 1. Maintain Documentation Quality

- Use clear technical language
- Keep formatting consistent
- Use proper markdown structure
- Add diagrams/screenshots when possible

---

## 2. Follow Engineering Standards

All updates should maintain:

- Clean architecture
- Structured telemetry design
- Hardware safety
- Reliable communication
- Proper testing methodology

---

## 3. Commit Message Guidelines

Use meaningful commit messages.

## ✅ Good Examples

```text
Added telemetry protocol documentation
Integrated Zigbee RSSI monitoring
Updated parachute deployment logic
Added SD logging validation results
```

## ❌ Avoid

```text
final update
misc changes
new stuff
```

---

# 💻 Software Contributions

When modifying embedded systems logic:

- Maintain 1 Hz telemetry timing
- Preserve packet structure compatibility
- Avoid blocking delays
- Keep subsystem modules independent

---

# 📡 Communication System Contributions

Ensure:

- Zigbee compatibility
- Reliable packet formatting
- RSSI logging support
- Ground station synchronization

---

# 🧪 Testing Contributions

All subsystem updates should be validated using:

- Communication testing
- Telemetry verification
- SD logging checks
- Structural testing
- Deployment testing

---

# 📷 Media & Documentation Contributions

When adding visuals:

- Use descriptive filenames
- Organize images into proper folders
- Avoid low-quality or duplicate uploads

---

# 🔒 Safety Guidelines

Contributors must avoid:

- Unsafe battery handling
- Improper wiring
- Unsupported RF modules
- Structural instability
- Unverified deployment logic

---

# 🚀 Engineering Philosophy

The Astrix CanSat project follows:

- Aerospace-oriented engineering
- Real-time embedded system design
- Structured subsystem integration
- Reliability-focused development
- Mission-driven architecture

---

# 👨‍💻 Team Astrix

Developed by:

- Hrutuj Dudhabale
- Team Astrix Members

---

# 📄 References

This repository follows the mission requirements and telemetry specifications defined by:
- Presidency University CanSat competition guidelines :contentReference[oaicite:0]{index=0}
- Astrix CanSat Critical Design Review (CDR) documentation :contentReference[oaicite:1]{index=1}
