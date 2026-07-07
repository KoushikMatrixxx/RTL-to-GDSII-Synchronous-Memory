# RTL-to-GDSII Physical Design of a Synchronous Memory

> **Complete ASIC Backend Implementation using Cadence Innovus 21.15 on 90nm CMOS Technology**

![Cadence](https://img.shields.io/badge/Cadence-Innovus%2021.15-red?style=flat-square)
![Technology](https://img.shields.io/badge/Technology-90nm-blue?style=flat-square)
![Flow](https://img.shields.io/badge/Flow-RTL--to--GDSII-green?style=flat-square)
![ASIC](https://img.shields.io/badge/ASIC-Physical%20Design-orange?style=flat-square)

---

## 📖 Project Overview

This repository presents the complete ASIC Physical Design implementation of a synchronous memory block, starting from a synthesized gate-level netlist and progressing through every major stage of the RTL-to-GDSII flow.

The implementation was carried out using **Cadence Innovus 21.15** on a **90nm CMOS technology**, covering floorplanning, power planning, placement, clock tree synthesis (CTS), post-CTS optimization, routing, physical verification, and final GDSII stream-out.

The project covers the complete ASIC backend flow, including:
- Floorplanning
- Power Planning
- Placement
- Clock Tree Synthesis (CTS)
- Post-CTS Optimization
- Routing
- Physical Verification
- GDSII Stream-Out

---

# 📋 Design Specifications

| Parameter | Value |
|-----------|-------|
| **Design Name** | Memory |
| **Design Type** | Synchronous Memory Block |
| **Technology Node** | 90nm CMOS |
| **Implementation Tool** | Cadence Innovus 21.15 |
| **Synthesis Tool** | Cadence Genus |
| **Operating System** | Linux x86_64 |
| **PVT Corner** | SS, 0.9V, 125°C |
| **Metal Layers Used** | M1–M6 |
| **Timing Methodology** | MMMC |
| **Final Output** | GDSII |

---

---

# 🔄 Physical Design Flow

```text
RTL Design
      │
      ▼
Logic Synthesis (Cadence Genus)
      │
      ▼
Gate-Level Netlist
      │
      ▼
Floorplanning
      │
      ▼
Power Planning
      │
      ▼
Placement
      │
      ▼
Clock Tree Synthesis (CTS)
      │
      ▼
Post-CTS Optimization
      │
      ▼
Routing
      │
      ▼
Physical Verification
      │
      ▼
GDSII Stream-Out
```

---
