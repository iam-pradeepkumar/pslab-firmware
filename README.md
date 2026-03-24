# 🔬 PSLab Firmware

<p align="center">
  <img src="https://pslab.io/images/pslab/pslab_v6.jpg" width="500"/>
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

<p align="center">
  <img src="https://pslab.io/images/features/oscilloscope.png" width="150"/>
  <img src="https://pslab.io/images/features/waveform.png" width="150"/>
  <img src="https://pslab.io/images/features/logic.png" width="150"/>
</p>

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

<p align="center">
  <img src="https://pslab.io/images/pslab-stack.png" width="600"/>
</p>

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

<p align="center">
  <img src="https://fossasia.org/img/fossasia-dark.png" width="300"/>
</p>

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
