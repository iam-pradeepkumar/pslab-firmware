# 🔬 PSLab Firmware

<p align="center">
  <img src="https://imgs.search.brave.com/PqX-QZoJzXboFRKTgW9g0MzaUYoLo4W633jjL_276IE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pMC53/cC5jb20vY29kZWhl/YXQub3JnL3dwLWNv/bnRlbnQvdXBsb2Fk/cy8yMDI1LzA2L3Bz/bGFiaW8uanBnP3Jl/c2l6ZT03MDAsNTAw/JnNzbD0x" width="300"/>
</p>

<p align="center">
  Firmware for the <b>Pocket Science Lab (PSLab)</b> — a portable open-source electronics laboratory.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/build-passing-brightgreen"/>
  <img src="https://img.shields.io/badge/license-Apache%202.0-blue"/>
  <img src="https://img.shields.io/badge/platform-Embedded-orange"/>
  <img src="https://img.shields.io/badge/language-C-blue"/>
</p>

---

## 🌟 Overview

The **Pocket Science Lab (PSLab)** is a compact, powerful hardware platform that integrates multiple scientific instruments into a single device.

This repository contains the **firmware** that powers PSLab hardware (v5 & v6), enabling:

- Device control  
- Communication handling  
- Instrument execution  

---

## ⚡ Features


- 📊 Oscilloscope  
- 🌊 Waveform Generator  
- 🔢 Frequency Counter  
- 🔌 Programmable Voltage & Current Sources  
- 📈 Logic Analyzer  

### 🔗 Connectivity

- UART  
- I2C  
- SPI  

---

## 🧩 Open Source Ecosystem



PSLab is part of a complete open-source ecosystem:

- 🔧 Hardware  
- ⚙️ Bootloader  
- 💻 Firmware *(this repo)*  
- 🐍 Python Library  
- 🖥️ Desktop Application  
- 📱 Android Application  

---

## 🛒 Get a PSLab Device

You can purchase the Pocket Science Lab from:

- 🛍️ **FOSSASIA Official Store**  
  👉 https://fossasia.com/shop  

- 🌐 **Official PSLab Website (Resellers List)**  
  👉 https://pslab.io  

> 💡 Availability may vary by region. Check the official website for global distributors.

---

## 🔔 Stay Updated

Stay connected with the PSLab community:

- 💬 **Gitter Chat**  
  👉 https://gitter.im/fossasia/pslab  

- 📧 **Mailing List**  
  👉 https://groups.google.com/g/pslab  

- 🐦 **Twitter / X Updates**  
  👉 https://twitter.com/fossasia  

- 🌐 **Official Website**  
  👉 https://pslab.io  

---

## 🏢 About FOSSASIA



**FOSSASIA** is a global open-source organization focused on:

- 🌍 Promoting open technologies  
- 🎓 Supporting student developers  
- 🤖 Building AI, hardware, and software solutions  
- 🧑‍💻 Running programs like **Google Summer of Code (GSoC)**  

### 🌟 What FOSSASIA Does

- Maintains **100+ open-source projects**  
- Organizes **FOSSASIA Summit**  
- Supports developers worldwide  

👉 Learn more: https://fossasia.org  

---

## 🛠️ Tech Stack

| Component     | Technology        |
|--------------|------------------|
| Language      | C                |
| Build System  | CMake            |
| Compiler      | Microchip XC16   |

---

## 📦 Repository Structure

```bash
pslab-firmware/
├── src/
│   ├── bus/
│   ├── helpers/
│   ├── instruments/
│   ├── registers/
│   ├── sdcard/
│   ├── main.c
│   └── commands.c
├── external/
│   └── cmake-microchip/
├── CMakeLists.txt
├── flash.mdbscript
└── README.md
```

---

## 🚀 Getting Started

### 1️⃣ Clone Repository

```bash
git clone https://github.com/fossasia/pslab-firmware.git
cd pslab-firmware
```

### 2️⃣ Setup Submodules

```bash
git submodule init
git submodule update
```

### 3️⃣ Build Firmware

```bash
mkdir build
cd build
cmake ..
make
```

📌 Output:

```bash
pslab-firmware.hex
```

---

## 🧪 Build for PSLab v5

```bash
cmake -DLEGACY_HARDWARE=true ..
```

---

## 🔥 Flashing Firmware

### 🔌 USB Method (Recommended)



```
bashmcbootflash --port <PORT> -b 460800 pslab-firmware.hex
```

### Steps:

1. Hold **BOOT**
2. Press **RESET**
3. Wait for LED blinking
4. Release BOOT
5. Flash firmware

---

### ⚠️ Using Programmer (PICkit3)

```bash
mdb.sh flash.mdbscript
```

> ⚠️ This may overwrite the bootloader

---

## 🔁 Bootloader Mode (PSLab v5)



Steps:

1. Bridge **BOOT + GND pins**
2. Reset device
3. LED starts blinking

---

## 🐳 Dev Container Support



* Open in VS Code
* Click **Reopen in Container**
* Start development instantly

---

## 🤝 Contributing

We welcome contributions!

1. Fork the repository
2. Create a branch
3. Commit changes
4. Submit a Pull Request

---

## 📄 License

Licensed under **Apache 2.0**

---

## 🌍 Why PSLab?

* 🧪 Affordable lab equipment
* 🌐 Fully open-source
* 🎓 Ideal for education & research

---

## ⭐ Support

If you like this project:

* ⭐ Star the repo
* 🍴 Fork it
* 🚀 Contribute

---

# ❤️ Built by FOSSASIA
