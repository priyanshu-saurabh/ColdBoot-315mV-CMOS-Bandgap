# 315 mV CMOS Reference With Autonomous Cold-Boot


---

## Overview  
NanoVolt-BGR is a **low-voltage CMOS bandgap reference (BGR)** designed to operate at **supply voltages below 1 V** while maintaining **high power supply rejection ratio (PSRR)**.  
This project provides a **stable, precise, and energy-efficient voltage reference** for analog and mixed-signal integrated circuits operating under **strict power constraints**.

The design is particularly suited for:  
- Ultra-low power systems  
- Energy-constrained sensor nodes  
- Mixed-signal SoCs  
- Next-generation analog front-ends  

---

##  Key Features  
- Reference voltage: 315 mV
- Supply range: 1.0 V – 5.0 V
- Temperature coefficient: ≈ 15 ppm/°C (−40 °C to 125 °C)
- PSRR: ≈ 60 dB (low frequency)
- Architecture: MOS-only, OTA-free, resistor-free
- Operation region: Weak to moderate inversion
- Startup: Fully autonomous cold-boot
- Power consumption: Low-µW range
**Applications**
- Energy-harvesting PMUs
- Ultra-low-power sensor interfaces
- Mixed-signal SoCs
- Batteryless and intermittent-power IoT nodes

---

## Design Methodology  
Will be updated  

---

##  Results  

---

## 📂 Repository Structure  
```plaintext
├── schematics/        # Cadence schematic files  
├── layout/            # Layout files and DRC/LVS reports  
├── simulations/       # Testbench and simulation results  
├── docs/              # Design notes, plots, and analysis  
└── README.md          # Project documentation  
