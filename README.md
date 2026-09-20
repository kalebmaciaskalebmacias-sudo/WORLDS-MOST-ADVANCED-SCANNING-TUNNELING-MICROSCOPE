# WhisperSTM

**The World’s First Truly Handheld, Wireless, Low-Cost Scanning Tunneling Microscope (STM).**

WhisperSTM achieves atomic-scale resolution (resolving individual carbon atoms in Highly Oriented Pyrolytic Graphite) under ambient conditions—**while being physically held in a human hand**. 

Traditionally, achieving picometer stability requires multi-million dollar laboratories outfitted with multi-ton floating concrete slabs, active pneumatic tables, and ultra-rigid ultra-high vacuum (UHV) framing. WhisperSTM bypasses expensive physical infrastructure by replacing it with high-speed digital signal processing and adaptive control loop architectures.

---

## 🏆 Project Achievements & World Firsts
* **World’s First Truly Handheld STM:** Functions reliably while subjected to the low-frequency, multi-axis disturbance of human physiological hand tremors.
* **World’s First Wi-Fi Controlled STM:** Streams raw atomic coordinate matrices over a peer-to-peer wireless network directly to consumer devices (like an iPhone 16) without standard network protocol bottlenecks or jitter crashes.
* **World’s Smallest DIY STM:** Eliminates large suspension springs, massive internal stone dampers, and multi-tiered heavy metal plates, shrinking the physical footprint down to a ultra-compact, low-rigidity acrylic K-mount.

---

## 🔬 Core System Architecture
WhisperSTM utilizes a split-architecture cyber-physical design to decouple real-time instrumentation requirements from user telemetry:

1. **Hardware Infrastructure (Open Source):** An entry-level, low-rigidity physical chassis designed using an acrylic K-mount, driven by ultra-precise positioning stages and a specialized piezoelectric actuator. 
2. **Proprietary Core Software Engine (Closed Source):** A high-speed digital signal processing framework that mathematically synthesizes structural rigidity, completely neutralizing real-world mechanical imperfections and external vibrations.

```
+---------------------------------------------------------------------------------+
|                               WhisperSTM System                                |
+---------------------------------------------------------------------------------+
|                                                                                 |
|  [ Physical Layer ]                                                             |
|   Acrylic K-Mount Chassis + Piezo Element + Tungsten/Pt-Ir Tip                  |
|         │                                                                       |
|         ▼ (Nano/Picoamp Tunneling Current Signal)                               |
|  [ Ultra-Low Noise Analog Front-End ]                                           |
|   High-Gain Pre-Amplifier Stage (Shielded Circuitry)                            |
|         │                                                                       |
|         ▼                                                                       |
|  [ High-Performance Control Node ]                                              |
|   18-bit ADC / 20-bit DAC Interface                                             |
|   └── 25kHz Ultrasonic Feedback Loop (40µs Real-Time Window)                    |
|   └── 2nd Order Sigma-Delta Engine (Up to 22-bit Precise Positioning)           |
|   └── 🛑 Core Algorithmic Control Engine (Proprietary / Closed Source)          |
|         ├── Lattice-Locking Algorithm (Real-Time Coordinate Anchoring)          |
|         ├── Thermal Drift Smoothing (Acrylic Material Expansion Subtraction)    |
|         └── 3D Adaptive Self-Tuning Predictive Feed-Forward Matrix              |
|         │                                                                       |
|         ▼ (Raw Matrix & Command Packets via Direct Wi-Fi Sockets / Non-BLE)     |
|  [ Supervisory Tier ]                                                            |
|   Cross-Platform Mobile Display Engine (Real-Time Handheld Telemetry)            |
|                                                                                 |
+---------------------------------------------------------------------------------+
```

---

## ⚙️ Hardware Specifications
This repository contains the full open-source layout blueprints, 3D CAD files, and circuit schematics to manufacture the structural physical instrument:

* **Chassis Frame:** Laser-cut Acrylic Kinematic-mount layout (K-mount).
* **Analog Interface:** Low-noise transimpedance amplifier schematics designed for picoamp/nanoamp extraction.
* **Data Converters:** Reference designs matching 18-bit ADC input telemetry and 20-bit DAC actuator output grids.
* **Actuation Base:** Low-cost, highly responsive segmented piezoelectric buzzer element / tube positioning assembly mapping sub-picometer steps.
MechPanda:

🛠️ Hardware Contributors
Chassis & System Integration: Kaleb Alexander (Me)
PCB Design & Layout: A massive thank you to MechPanda for designing and routing the ultra-low-noise analog front-end and converter PCB layout. Their precision routing made dealing with picoamp-scale signals possible under ambient conditions.
---

## 🔒 Firmware & Software Notice
To maintain the integrity, safety, and proprietary nature of the high-speed computational components, **the raw software code and mathematical matrix profiles are strictly closed-source and omitted from this public repository.**

Users can evaluate the fully operational handheld architecture by downloading pre-compiled execution targets under the [Releases](../../releases) panel. The firmware runs as an encapsulated black-box binary file (.hex/.bin), preserving the internal mathematics of the self-tuning matrices while offering complete integration with the open-source physical hardware listed above.

---

## 📄 License
The physical schematics, mechanical drawings, and BOM files shared within this repository are licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** License. Commercial utilization, manufacturing, or distribution of this hardware frame layout without explicit contractual consent is strictly prohibited.
