# SpeedyBee F405-Mini – 7″ ArduCopter Reference Parameters

## Document Information
- **Date:**   
- **Document ID:** SB_F405 Mini  
- **Version:** V  

---

## Hardware Configuration

- **Flight Controller:** SpeedyBee F405 mini  
- **ESCs:** SpeedyBee 55A AIO  
- **Frame:** 5″  
- **Motors:**   
- **GPS:** TBS M10Q  
- **Receiver:**   
- **Transmitter:** RadioMaster GX12  
- **Battery:** 4S LiPo – 1300 mAh  
- **Propellers:**   
- **Companion Computer:** Raspberry Pi Zero 2 W  
- **Data Bearer:** 4G cellular USB dongle  

---

## Software Configuration

- **FC Firmware:** ArduPilot Copter 4.6.3  
  - Firmware build used at time of configuration  
  - https://firmware.ardupilot.org/Copter/stable-4.6.3/SpeedyBeeF405Mini/

- **ESC Firmware:**  
  - BlueJay (J-H-40)  
  - Version 0.21.0  
  - 48 kHz PWM  

---

## Intended Use and Warnings

This configuration supports a **7″ BVLOS-capable UAS** using a **cellular (4G) bearer**
to deliver **video and MAVLink telemetry** back to a Ground Control Station (GCS).

Failsafes, link behaviour, and system assumptions in this parameter file
reflect **BVLOS and cellular operation**.

⚠️ **Important**  
If your operational intent differs, **review all parameters carefully**
before use. This file is provided **for reference only**.

---

## Load and Setup Procedure

### 1. Initial Parameter Load
Load and write this `.param` file to the aircraft using **Mission Planner**.

---

### 2. Mission Planner Mandatory Setup

Complete the following setup steps:

#### Mandatory
- Accelerometer calibration  
- Compass calibration  
- Radio calibration  
- Initial tune parameters  
  - Apply suggested settings for ArduPilot 4.0 and higher  

#### Optional Hardware
- Joystick configuration  
- Motor test  

---

### 3. Final Parameter Load
After completing setup, **reload this parameter file** to ensure
the intended configuration is restored.

---

## Notes
- UART mappings and peripheral configuration are **hardware-specific**
- Companion computer settings assume a Raspberry Pi Zero 2 W
- Cellular latency and packet loss have **not been optimised**
