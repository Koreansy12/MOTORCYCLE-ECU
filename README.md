# 🚀 FCU32 – Fuel Control Unit Based on ESP32

## 📌 Overview  
**FCU32** is an **experimental project** to build a simple **Fuel Control Unit (ECU)** using the **ESP32** platform.  
The main goal is to control a fuel injector based on standard engine sensors (RPM, MAP, TPS, O2, etc.).  

⚠️ **Disclaimer:**  
This project is still **theoretical**. The components and system have been designed and validated on paper, but **not yet fully realized in hardware**. It’s more like a **concept validation** and research documentation.

---

## 🛠️ Main Components
- **ESP32-S3** (main MCU)  
- **MAP + IAT + TPS Sensor** (from MAQS injector system)  
- **O2 Sensor** (Beat FI)  
- **RPM Pickup Sensor**  
- **Injector (Mio J)**  
- **Power Supply & MOSFET Driver** for injector control  

---

## 📊 Planned Features
- Fuel Injection Control via **lookup/VE table**  
- RPM sensing using **interrupts**  
- TPS & MAP input for engine load calculation  
- O2 sensor input for **closed-loop fuel correction** (planned)  
- UART/I2C communication with a **second ESP32-S3** (for display, logging, fuzzy logic)  
- Multitasking support using **FreeRTOS**  

---

## 📂 Project Status
- ✅ RPM sensor tested on ESP32 (MicroPython)  
- ✅ Pinout and main components planned  
- 🟡 Fuel mapping table (draft stage)  
- 🟡 Injector MOSFET driver (design stage)  
- ❌ Full hardware implementation not yet realized  

---

## 🚧 Next Steps
1. Implement fuel mapping → injector duty cycle control  
2. Test MOSFET driver with actual injector  
3. Integrate O2 sensor for closed-loop correction  
4. Optimize multitasking using FreeRTOS  

---

## ⚡ Why FCU32?
Most aftermarket ECUs are:  
- Expensive 💸  
- Closed-source 🔒  
- Not flexible for DIY/research purposes  

FCU32 aims to be **open-source, affordable, and flexible**, making it suitable for electronics/automotive students and hobbyists who want to experiment.

---

## 📜 License
MIT License – free to use, modify, and develop.  
⚠️ **Note:** This is **not a plug-and-play ECU**. Use at your own risk.

---

## 🤝 Contribution
Contributions are welcome! You can help by:  
- Adding MicroPython / C++ code for injector control  
- Designing hardware (driver + protection circuits)  
- Engine simulation (EngineSim, MATLAB, etc.)  
- Testing on real engines (⚠️ do it at your own risk)  

---

## 🔥 Notes
> This component is theoretically right but has not been realized yet.  
> FCU32 is still in the **concept stage**, and this documentation is mainly to track progress and guide future development.  
