# VSD RISC-V SoC Tapeout Program 
[![VSD](https://img.shields.io/badge/VSD-RISC--V%20SoC-blue?style=for-the-badge)](https://www.vlsisystemdesign.com/)
![Linux](https://img.shields.io/badge/OS-Linux%20%7C%20Ubuntu-orange?style=for-the-badge&logo=linux)
![Git](https://img.shields.io/badge/Version%20Control-Git-black?style=for-the-badge&logo=git)
![RISC-V](https://img.shields.io/badge/Architecture-RISC--V-blue?style=for-the-badge&logo=riscv)


---

## 📌 Table of Contents  
- [Introduction](#-introduction)  
- [Tasks Overview](#-tasks-overview)  
- [Week 0 – Tool Installation & Verification](#-week-0--tool-installation--verification)  
- [Week 1 – Coming Soon](#-week-1--coming-soon)  
- [Acknowledgments](#-acknowledgments)  
- [References](#-references)  

---

## 🔰 Introduction  
This repository documents my **learning journey and weekly submissions** for the **VSD RISC-V SoC Tapeout Program**.  

The program is designed to provide hands-on exposure to:  
- 🛠️ Setting up open-source EDA tools  
- ⚡ Understanding RISC-V SoC design flow  
- 🐧 Working with Linux & Git  
- 🚀 RTL design, synthesis, verification, and tapeout  

💡 The aim is to **learn → implement → verify → document → share**.  

---

## 📝 Tasks Overview  

| Week | Focus Area | Status |
|------|------------|--------|
| **0** | Tool installation, environment setup, Teardrop verification | ✅ Completed |
| **1** | RISC-V toolchain exploration, basic simulation | 🔜 Coming soon |
| **2** | RTL design & synthesis | ⏳ Planned |
| **3** | Physical design & layout | ⏳ Planned |

---

## 📦 Week 0 – Tool Installation & Verification  

### 🔹 Step 1: Update & Install Essential Packages  
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install git make gcc g++ vim build-essential -y
```

---

### 🔹 Step 2: Install Required Tools  

#### ✅ Yosys  
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt-get install build-essential clang bison flex     libreadline-dev gawk tcl-dev libffi-dev git     graphviz xdot pkg-config python3 libboost-system-dev     libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
git submodule update --init --recursive
make
sudo make install
```
📸 *Screenshot:*  
![Yosys Installation](./images/week0_yosys_done.png)  

---

#### ✅ Icarus Verilog (Iverilog)  
```bash
sudo apt-get update
sudo apt-get install iverilog
```
📸 *Screenshot:*  
![Iverilog Status](./images/week0_iverilog_done.png)  

---

#### ✅ GTKWave  
```bash
sudo apt-get update
sudo apt install gtkwave
```
📸 *Screenshot:*  
![GTKWave Installation](./images/week0_gtkwave_done.png)  

---

### 🔹 Step 3: Verify with Teardrop Example  
Run the included test to confirm installation:  

```bash
make test
```

✅ **Expected Output:**  
```text
[INFO] Toolchain working correctly
[PASS] Teardrop verification complete
```

📸 *Screenshot:*  
![Teardrop Verification](./images/week0_teardrop_output.png)  

---

### ✅ Learnings from Week 0  
- Set up Ubuntu VM inside VirtualBox  
- Installed open-source tools (Yosys, Iverilog, GTKWave)  
- Verified installation with **Teardrop test case**  
- Learned Linux command-line basics  

---

## ⚙️ Week 1 – Coming Soon  

🔜 Planned tasks:  
- Setup RISC-V toolchain  
- Run sample RISC-V programs  
- Capture waveforms & document simulation results  

---

## 🙏 Acknowledgments  
I sincerely thank:  
- **VSD (VLSI System Design)** team for this initiative  
- Mentors & community for guidance  
- Open-source developers for tools like Yosys, Iverilog, GTKWave  

---

## 📚 References  
- [VSD Official GitHub](https://github.com/vlsisystemdesign)  
- [RISC-V International](https://riscv.org)  
- [Yosys Documentation](http://www.clifford.at/yosys/)  
- [Linux Command Handbook](https://linuxcommand.org/)  

---

✨ *This repository will be updated weekly with tasks, commands, outputs, and screenshots as I progress through the program.*  
