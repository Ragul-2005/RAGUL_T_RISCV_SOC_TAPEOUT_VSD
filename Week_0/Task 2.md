# ⚙️ SOC_TAPEOUT_VSD — ToolS Installation and Setup Guide

## 🖥️ **Before You Begin – System Checklist**  

Make sure your system is ready for synthesis, simulation, and layout by meeting the **minimum hardware/software requirements** below:  

<div align="center">

| 🔧 **Component** | ✅ **Recommended Setup** |
|------------------|--------------------------|
| 🐧 **OS**        | Ubuntu 20.04 LTS or newer |
| 💾 **Memory**    | 6 GB (8 GB+ preferred 🚀) |
| 💿 **Disk**      | 50 GB free storage |
| ⚡ **CPU Cores** | 4 vCPUs (multi-core boosts speed) |

</div>  

---

## 📑 Tools to Install
Click a tool name to jump to installation instructions 👇

- [Yosys](#1-yosys-synthesis-tool)  
- [Icarus Verilog (iverilog)](#2-icarus-verilog-simulator)  
- [GTKWave](#3-gtkwave-waveform-viewer)  
- [NGSpice](#4-ngspice-circuit-simulator)  
- [Magic](#5-magic-vlsi-layout-tool)  
- [OpenLane](#6-openlane-physical-design-flow)  

---

## 🛠 Installed Tools & Verification

### 1. Yosys (Synthesis Tool)

<details>
<summary><b>Purpose:</b> CYosys is an open-source logic synthesis tool that converts HDL (like Verilog) into gate-level netlists for FPGA or ASIC implementation. It also performs optimization, analysis, and verification of digital designs.</summary>

</details>
