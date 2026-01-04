# Matek H743 V3 – T1 Ranger VTOL ArduPlane Reference Parameters

## Document Information
- **Date:** 25/05/2025  
- **Document ID:** Matek_H743_v3  
- **Version:** V5  

---

## Hardware Configuration

- **Flight Controller:** Matek H743 Wing V3  
- **ESCs:**   
- **Frame:** T1 Ranger VTOL  
- **Motors:** Heewing FX 1806 2000kv  
- **GPS:** Matek M10Q 5883   
- **Receiver:** ELRS DBR4-Xband Gemini (2.4G + 900Mhz)  
- **Transmitter:** RadioMaster GX12  
- **Battery:** 4S LiHV – 3500 mAh  
- **Propellers:**
- **VideoTransmitter:** DJI 04 Pro air unit
- **FPV Goggles:** DJI Goggles 3
- **Companion Computer:**  
- **Data Bearer:**  

---

## Software Configuration

- **FC Firmware:** ArduPlane V4.5.7  bdshot
  - Firmware build used at time of configuration  
  - https://firmware.ardupilot.org/Plane/stable-4.5.7/MatekH743-bdshot/

- **Online Param BASELINE File:**
  - There is a very helpful BASE param file online, other than this one. That was of great help to me
  - https://blog.unmanned.tech/hee-wing-ranger-tuning-guide-6-month-journey-to-perfection-for-ardupilot-vtol/   

- **ESC Firmware:**  
  - BlueJay   
  - Version 0.21.0  
  - 48 kHz PWM  

---

## Intended Use and Warnings

This configuration supports a fixed wing aircraft that transitions into a VTOL. 

This build focusses on the working of a VTOL flown LOS / FPV

Failsafes, link behaviour, and system assumptions in this parameter file
reflect **LOS / FPV**.

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
