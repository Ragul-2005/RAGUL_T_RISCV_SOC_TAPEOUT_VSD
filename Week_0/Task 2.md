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
<summary><b>Purpose:</b> Yosys is an open-source logic synthesis tool that converts HDL (like Verilog) into gate-level netlists for FPGA or ASIC implementation. It also performs optimization, analysis, and verification of digital designs.</summary>

</details>

## ✅ **Yosys Installation**

```bash
# Day 0 - Tools Installation
## Yosys

# Clone the Yosys repository from GitHub
$ git clone https://github.com/YosysHQ/yosys.git

# Change directory to the cloned yosys folder
$ cd yosys

# Install 'make', a build automation tool
$ sudo apt install make

# Install all dependencies required to build Yosys
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Configure Yosys to use GCC for compilation
$ make config-gcc

# Initialize Git submodules (required for abc)
$ git submodule update --init --recursive

# Compile the Yosys source code into executable binaries
$ make

# Install the compiled Yosys binaries system-wide
$ sudo make install
```


## 📷 **Installation Verification**

```bash
# Run Yosys after installation
$ yosys

# Verify license
$ license
```

<p align="center">
 
  <img src="https://github.com/Ragul-2005/RAGUL_T_RISCV_SOC_TAPEOUT_VSD/blob/main/Week_0/Images/yosys.png?raw=true" 
       alt="Yosys Installed" width="600"/>
</p>

<div align="center">
  ✅ **Yosys Successfully Installed**
</div>


