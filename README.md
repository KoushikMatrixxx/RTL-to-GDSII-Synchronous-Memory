<div align="center">

# ⚙️ ASIC Physical Design Laboratory

## RTL-to-GDSII Implementation of a Synchronous Memory

```text
██████╗ ████████╗██╗         ██████╗  ██████╗ ██████╗ ███████╗██╗██╗
██╔══██╗╚══██╔══╝██║        ██╔════╝ ██╔══██╗██╔══██╗██╔════╝██║██║
██████╔╝   ██║   ██║        ██║  ███╗██║  ██║██████╔╝███████╗██║██║
██╔══██╗   ██║   ██║        ██║   ██║██║  ██║██╔══██╗╚════██║██║██║
██║  ██║   ██║   ███████╗   ╚██████╔╝██████╔╝██████╔╝███████║██║██║
╚═╝  ╚═╝   ╚═╝   ╚══════╝    ╚═════╝ ╚═════╝ ╚═════╝ ╚══════╝╚═╝╚═╝
```

**Complete RTL → GDSII Physical Design Flow**

Cadence Innovus • 90nm CMOS • Signoff Clean

</div>

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

# 📊 Implementation Summary

| Metric | Result |
|--------|--------|
| Technology Node | 90nm CMOS |
| Implementation Tool | Cadence Innovus 21.15 |
| Synthesis Tool | Cadence Genus |
| Placement Engine | GigaPlace |
| CTS Engine | CCOpt |
| Routing Engine | NanoRoute |
| Metal Layers | M1–M6 |
| Operating Corner | SS, 0.9V, 125°C |
| WNS | 0.927 ns |
| TNS | 0.000 ns |
| Clock Skew | 0.015 ns |
| Maximum Clock Latency | 0.179 ns |
| Hold Violations | 0 |
| DRC Violations | 0 |
| PG Short Violations | 0 |
| Connectivity Violations | 0 |
| Routing Overflow | 0.00% |

---

# 🎯 Final Results at a Glance

| **Metric** | **Value** | **Status** |
|------------|-----------|------------|
| WNS (Setup, All Modes) | **0.927 ns** | ✅ PASS |
| TNS | **0.000 ns** | ✅ PASS |
| Violating Paths | **0** | ✅ PASS |
| Hold Violations | **0** | ✅ PASS |
| Clock Skew | **0.015 ns** | ✅ PASS |
| Maximum Clock Latency | **0.179 ns** | ✅ PASS |
| DRC Violations | **0** | ✅ PASS |
| Power/Ground Short Violations | **0** | ✅ PASS |
| Connectivity Violations | **0** | ✅ PASS |
| Routing Overflow | **0.00% (Horizontal), 0.00% (Vertical)** | ✅ PASS |
| Maximum Transition | **0.280 ns** | ✅ PASS |
| Final Cell Density | **61.335%** | 📊 Achieved |

---

# 🛠 Tools and Technologies

| **Category** | **Details** |
|--------------|-------------|
| **Implementation Tool** | Cadence Innovus 21.15-s110_1 |
| **Logic Synthesis** | Cadence Genus |
| **Placement Engine** | GigaPlace (Timing-Driven Placement) |
| **Clock Tree Synthesis (CTS)** | CCOpt |
| **Routing Engine** | NanoRoute |
| **Programming & Scripting** | TCL, Linux Bash |
| **Technology Node** | 90 nm CMOS |
| **Standard Cell Library** | LVT Standard Cell Library (e.g., DFFQX1LVT, CLKBUFX6LVT, NAND4XLVT) |
| **Timing Methodology** | MMMC (Multi-Mode Multi-Corner) — Setup: func_ss, Hold: func_ff |
| **Physical Verification** | DRC, PG Short Check, Connectivity Verification |
| **Output Generated** | Final GDSII Layout |

---

# 📚 Key Learnings

Through this project, the following Physical Design concepts were explored and implemented:

- ASIC RTL-to-GDSII Design Flow
- Floorplanning Techniques
- Power Planning
- Standard Cell Placement
- Clock Tree Synthesis (CTS)
- Global and Detailed Routing
- RC Extraction
- Static Timing Analysis (STA)
- Physical Verification (DRC & Connectivity)
- GDSII Generation
- TCL Script Automation

---

# 📂 Repository Structure

```text
RTL-to-GDSII-Synchronous-Memory
│
├── README.md                 # Project documentation
├── screenshots/              # Layout and implementation images
├── reports/                  # Timing and verification reports
├── scripts/                  # Tcl implementation scripts
├── outputs/                  # Final generated outputs (GDSII, etc.)
└── docs/                     # Additional documentation
```

This repository is organized to keep implementation files, reports, scripts, and documentation separate for better readability and easier navigation.

---
