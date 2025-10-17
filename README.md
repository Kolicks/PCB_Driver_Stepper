# 🌀 PCB_Driver_Stepper
**General Stepper Motor Driver Board**

---

## 📘 Overview
**PCB_Driver_Stepper** is a general-purpose stepper motor driver board designed in **KiCad 9**.  
This project was created to explore stepper motor control concepts, test design ideas from friends, and gain real experience with PCB design and STM32 microcontroller integration.  
It also represents my first complete project combining **hardware and STM32 firmware** using **STM32CubeIDE**.

<p align="center">
  <img src="images/3D.png" alt="3D Render" width="500"/>
  <br>
  <em>3D render of the finished PCB_Driver_Stepper board</em>
</p>

---

## ⚙️ General Information
- First real **KiCad 9** project.
- Implemented to test and validate several design ideas.
- Tested multiple implementations, including **ULN2002** and different **power dissipation** techniques.
- Designed with **4 layers**, though a **2-layer** version could be feasible.
- Typical **FR4 PCB**, **1.6 mm thickness**, standard prepreg stackup.
- Serves as my first practical integration within **STM32CubeIDE**, using **STM32F030K6Tx** as the MCU.

<p align="center">
  <img src="images/SCH.png" alt="Schematic" width="600"/>
  <br>
  <em>Full schematic diagram (KiCad 9)</em>
</p>

---

## 🔧 Characteristics
- **Fully functional**, fabricated and tested successfully.
- Tested with **STEPPERONLINE NEMA 17** (2A, 59 N·cm) — achieves over **300 RPM** without load.
- Capable of controlling **two stepper motors** simultaneously.
- Supports up to **2 A per motor**, limited by drivers and onboard potentiometers.
- **Operating voltage:** 12 VDC to 24 VDC (ideal at 24 V).
- Requires **external cooling** (top and bottom) for continuous operation.
- Integrated with **ULN2002A** as input mode (tested and working).
- Uses **pin connectors under driver GND pads** to allow hand-soldering.
- Optional **Schottky diodes** for additional protection and power isolation.

<p align="center">
  <img src="images/PCB.png" alt="PCB Layout" width="600"/>
  <br>
  <em>PCB layout view showing 4-layer design</em>
</p>

---

## ⚠️ Known Issues / Notes
- Thermal pads on the **Rsense GND pads** may restrict efficient heat dissipation.
- Ideally should maintain a **4-layer design** to ensure proper driver thermal management (as recommended in datasheets).
- **No status LEDs** (e.g., Power or Fault indicators) currently included — consider adding in future revisions.

---

## 🧩 Files and Structure

