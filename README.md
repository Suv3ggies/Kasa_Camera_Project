# Kasa Pan/Tilt/Zoom Camera Research Project

## 📘 Overview
This project documents my research, analysis, and experimentation with my personally owned **Kasa Pan/Tilt/Zoom camera**.  
The goal is to gain a deeper understanding of the device’s firmware, communication protocols, and system architecture to improve local interoperability, automation, and security auditing.

> ⚠️ Disclaimer:  
> This repository is for **educational and personal research purposes only**.  
> Do **not** use this information to access, modify, or distribute firmware or data belonging to others.  
> All testing is done on **devices I personally own**.

---

## 🧠 Project Objectives
- Document hardware and software components of the Kasa PTZ camera  
- Identify communication interfaces (UART, SPI, I²C, network protocols, etc.)  
- Analyze firmware structure and system logs  
- Explore methods to improve **local control** and **privacy** (e.g., Home Assistant integration, local-only operation)  
- Document safe recovery methods and firmware restoration

---

## ⚙️ Device Information
| Component | Description |
|------------|--------------|
| **Model** | Kasa Spot Pan Tilt 24/7 Recording: EC70 |
| **FCC ID** | 2AXJ4C200V2 |
| **Firmware Version** | [insert firmware version] |
| **Processor/Chipset** | [insert SoC or MCU name] |
| **Memory/Flash** | [insert size/type if known] |
| **Interfaces Found** | UART, SPI |
| **Power Requirements** | 9.6V DC 0.6A |

---

## 🔍 Research Methods
1. **Hardware inspection**
   - Open casing and locate test pads, UART pins, and flash chips  
   - Identify chip markings and manufacturer data sheets  

2. **Firmware analysis**
   - Obtain a **backup of the original firmware** (never distribute binaries)  
   - Examine partition layout, filesystem, and boot process  
   - Look for open-source components or known CVEs  

3. **Network analysis**
   - Observe communication with Kasa servers  
   - Analyze packet capture to identify control protocols (RTSP, MQTT, etc.)  
   - Develop local control scripts or integrations  

---

## 🧰 Tools Used
| Tool | Purpose |
|------|----------|
| **Hardware Tools** |
| CH341A Programmer | SPI flash reading |
| Oscilloscope | Electrical Analysis |
| Multimeter | Voltage Verification |

| Tool | Purpose |
|------|----------|
| ** Software Tools** |
| Binwalk | Firmware unpacking |
| strings / hexdump | Binary inspection |
| Wireshark | Network traffic capture |
| Python | Protocol testing & automation |

---

## 🪛 Progress
- [x] Identified UART interface
- [x] Identified SPI interface
- [x] Dumped factor firmware for analysis
- [ ] Backed up factory firmware safely  
- [ ] Mapped partition table  
- [ ] Analyzed boot logs  
- [ ] Documented network endpoints  
- [ ] Implemented local RTSP access  
- [ ] Tested local control integration  

---

## 🔐 Security & Ethics
- Research is done **only on personally owned devices**  
- No redistribution of firmware or proprietary code  
- Findings are documented to **improve consumer transparency** and **device security**  
- Responsible disclosure will be followed for any vulnerabilities found

---

## 📄 References
- [Kasa Developer Documentation](https://www.kasasmart.com/)
- [Binwalk Documentation](https://github.com/ReFirmLabs/binwalk)
- [OpenWrt Embedded Linux](https://openwrt.org/)
- [FCC ID Lookup](https://fccid.io/)

---

## 🧩 Future Goals
- Full local API documentation  
- Integration into open-source home automation  
- Security hardening and privacy-by-design review  

---

## 🗒️ License
This project is licensed under the **MIT License**.  
You are free to reference the documentation for personal, non-commercial educational purposes.

---

*Author: [Jacob Suveges]*  
*Date: [2025-11-11]*  
