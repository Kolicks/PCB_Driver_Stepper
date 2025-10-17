# 🌀 PCB_Driver_Stepper
**General Stepper Motor Driver Board**

---

## 📘 Overview
**PCB_Driver_Stepper** is a general-purpose stepper motor driver board designed in **KiCad 9**.  
This project serves as a real hardware implementation to test stepper control concepts and some design ideas proposed by friends.  
It also represents one of my first practical projects involving **STM32 firmware development** using **STM32CubeIDE**.

---

## ⚙️ General Information
- First real **KiCad 9** project.
- Implemented to experiment with motor control ideas and hardware layout.
- Designed with **4 layers** (though can likely be reduced to 2 layers).
- Typical FR4 PCB, **1.6 mm thickness**, standard prepreg.
- Includes experimentation with components such as **ULN2002** and various power dissipation techniques.
- Serves as a learning and test platform for integration with **STM32CubeIDE**.

---

## 🔧 Characteristics
- **Fully functional**, fabricated and tested.
- Tested with **STEPPERONLINE NEMA 17 (2A, 59 N·cm)** — achieves >300 RPM (no load).
- Supports **2 stepper motors**.
- Current: up to **2 A per motor**, limited by driver and potentiometer configuration.
- **Operating voltage:** 12–24 VDC (ideal 24 V).
- Requires **external cooling** (top and bottom) for driver reliability.
- Compatible with **ULN2002A** as input driver (tested and functional).
- Optional **Schottky diodes** for protection.
- Uses **pin connectors under driver GND pads** for easier hand-soldering.

---

## ⚠️ Known Issues / Notes
- Thermal pads under **Rsense GND pads** may limit thermal dissipation.
- Should ideally remain **4-layer** for better driver heat performance (per datasheet recommendations).
- Missing **indicator LEDs** (e.g., Power or Status).
- Consider adding LEDs and improving heat dissipation in future revisions.

---

## 🧩 Files and Structure
