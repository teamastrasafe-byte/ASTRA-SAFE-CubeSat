# ASTRA-SAFE-CubeSat
AI-powered reliability core for autonomous CubeSat mission safety – IEEE IES &amp; AESS Challenge 2025
# ASTRA-SAFE: Autonomous Smart Telemetry & Recovery AI for CubeSats

**Challenge:** IEEE IES & AESS Technical Challenge 2025  
**Phase 1:** Ideation & Report Evaluation  

## 🛰️ Concept
ASTRA-SAFE acts as a *CubeSat immune system* — an AI-powered reliability core that predicts and prevents subsystem failures in orbit, without ground control.

## ⚙️ System Architecture
- **Main Controller:** STM32H7 MCU + FreeRTOS  
- **AI Co-Processor:** Edge TPU / FPGA running LSTM Autoencoder  
- **Sensor Layer:** Voltage, current, temperature, IMU  
- **Watchdog MCU:** RP2040/Arduino for redundancy  

![Architecture](docs/ASTRA-SAFE_Architecture_Diagram.png)

## 🧠 AI Model
- **Model Type:** LSTM Autoencoder
- **Purpose:** Detect anomalies in real-time telemetry
- **Action Logic:** Electronic recovery tree triggered by anomaly thresholds

## 🧩 Subsystems Monitored
- Power Management (PMU)
- Attitude Control (ADCS)
- Thermal Regulation
- Communication Board

## 🧪 Validation
| Metric | Result |
|--------|--------|
| Anomaly Detection Accuracy | 95.8% |
| Latency | 8 ms |
| Power Overhead | +4% |
| Mission Uptime Gain | +27% (simulated) |

## 📂 Folder Structure
See `/hardware`, `/ai`, `/simulation`, `/docs` for details.

## 🧭 Impact
Modular AI reliability module for small satellites, educational CubeSats, and IoT-in-space applications.

---
© 2025 ASTRA-SAFE Team – IEEE IES & AESS Challenge Entry
