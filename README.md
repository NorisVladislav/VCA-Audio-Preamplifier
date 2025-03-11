# National University of Science and Technology POLITEHNICA Bucharest  
## Faculty of Electronics, Telecommunications, and Information Technology  

### Academic Year 2024-2025  

---

# Project 1  

## Design and Implementation of an Audio Preamplifier with Voltage-Controlled Gain  

**Group:** 432B  
**Supervisors:**  
- Prof. Dr. Eng. Dragoș Dobrescu  
- Lecturer Dr. Eng. Mădălin Moise  

---

## Table of Contents  

1. [Introduction](#introduction)  
2. [Initial Project Data](#initial-project-data)  
   - [Project Description](#project-description)  
   - [Block Diagram of the Electrical Circuit](#block-diagram-of-the-electrical-circuit)  
3. [Technical Content](#technical-content)  
   - [Electrical Circuit Diagram](#electrical-circuit-diagram)  
   - [Simulation of the Audio Preamplifier](#simulation-of-the-audio-preamplifier)  
   - [Static Operating Points](#static-operating-points)  
   - [Analytical Calculation of PSF](#analytical-calculation-of-psf)  
   - [Bill of Materials](#bill-of-materials)  
4. [PCB Design using SMT Technology](#pcb-design-using-smt-technology)  
   - [General Layout](#general-layout)  
   - [Top and Bottom Layer Interconnection](#top-and-bottom-layer-interconnection)  
   - [Silkscreen, Solder Mask, and Stencil](#silkscreen-solder-mask-and-stencil)  
   - [Drill and Cutting Layers](#drill-and-cutting-layers)  
   - [Mechanical Layer (FAB)](#mechanical-layer-fab)  
5. [Assembly and Soldering Process](#assembly-and-soldering-process)  
6. [User Manual](#user-manual)  
7. [Conclusion](#conclusion)  
8. [References](#references)  

---

## Introduction  

A **Voltage-Controlled Amplifier (VCA)** is an essential component in audio signal processing, allowing dynamic control of amplification without mechanical intervention. This technology is crucial for applications such as **mixing, dynamic compression, and audio effects processing**.  

This project focuses on designing a **compact VCA-based audio preamplifier** with **precise gain control via an external voltage**. The implementation ensures high stability and linearity of the output signal. Additionally, the **use of Surface-Mount Technology (SMT) for PCB design** provides a compact and robust solution that complies with **IPC-2221A and IPC-A-610** industry standards.  

---

## Initial Project Data  

### Project Description  

The goal is to design and implement a **voltage-controlled audio preamplifier** with the following characteristics:  

- **Power Supply:** 12V 
- **Input Signal:** Sinusoidal, 0-20mV amplitude  
- **Frequency:** 2 kHz  
- **Control Voltage:** 0V to 2V  
- **Gain Range:** 1x to 20x  
- **Load Resistance:** 700Ω  
- **LED Indicator:** For power supply presence  

### Block Diagram of the Electrical Circuit  

![Block Diagram](images/aa.png)  

---

## Technical Content  

### Electrical Circuit Diagram  

![Electrical Schematic](images/SCHMA.png)  
![Electrical Schematic](images/SCHMB.png) 

### Simulation of the Audio Preamplifier  

- **Vcontrol = 0V → Gain = 1x (Buffer Mode)**  
- **Vcontrol = 2V → Gain = 20x (Maximum Amplification)**  

![Simulation Results](images/SIMA.png)  
![Simulation Results](images/SIMB.png)  

### Static Operating Points  

- **Vcontrol = 0V**  
  - Voltage Values: ...  
  - Current Values: ...  
  - Power Dissipation: ...  

- **Vcontrol = 2V**  
  - Voltage Values: ...  
  - Current Values: ...  
  - Power Dissipation: ...  

### Analytical Calculation of PSF  

(Include relevant calculations here)

### Bill of Materials  

![BOM](images/BOM.png) 

## PCB Design using SMT Technology  

### General Layout  

![PCB Layout](path/to/pcb-layout.png)  

### Top and Bottom Layer Interconnection  

![Top Layer](path/to/top-layer.png)  
![Bottom Layer](path/to/bottom-layer.png)  

### Silkscreen, Solder Mask, and Stencil  

- **Silkscreen Layer (SSTOP)**  
  ![Silkscreen](path/to/silkscreen.png)  

- **Solder Mask Layer (SMTOP, SMBOT)**  
  ![Solder Mask](path/to/solder-mask.png)  

- **Solder Paste Stencil (SPTOP)**  
  ![Stencil](path/to/stencil.png)  

### Drill and Cutting Layers  

- **Drill Holes (DRILL)**  
  ![Drill Layer](path/to/drill.png)  

- **Cutting Layer (BO)**  
  ![Cutting Layer](path/to/cutting-layer.png)  

### Mechanical Layer (FAB)  

![Mechanical Layer](path/to/mechanical-layer.png)  

---

## Assembly and Soldering Process  

- **Required Tools:**  
  - Soldering station  
  - Solder wire (SnAgCu alloy)  
  - Flux and desoldering braid  

- **Soldering Procedure:**  
  1. Set soldering iron temperature to **370°C**.  
  2. Apply flux and solder components.  
  3. Use a desoldering braid to remove excess solder if needed.  

---

## User Manual  

### Power Connection  
1. Connect **GND terminals** of power and input signal.  
2. Apply **12V DC power**.  
3. Connect the **sinusoidal input signal**.  

### Gain Adjustment  
- Apply **0V to 2V** at the control terminal:  
  - **0V → Gain = 1x (No amplification)**  
  - **2V → Gain = 20x (Maximum amplification)**  

### Safety Precautions  
- **Do not modify or touch** components while powered.  
- **Handle the PCB carefully** to avoid electrostatic discharge.  
- **Avoid moisture and extreme temperatures.**  

---

## Conclusion  

The **Audio Preamplifier with Voltage-Controlled Gain** successfully demonstrates:  

✅ **Stable and precise gain control**  
✅ **High-fidelity signal amplification**  
✅ **Compact and industry-compliant PCB design**  

The project is useful for **audio processing, research, and education** and serves as a foundation for further development.  

---

## References  

1. G. Brezeanu, F. Drăghici - *Fundamental Electronic Circuits*, Niculescu Publishing, Bucharest, 2013.  
2. Dan Dascălu - *Electronic Devices and Circuits*, Didactic & Pedagogical Publishing, Bucharest, 1982.  
3. Wikipedia - [Variable-Gain Amplifier](https://en.wikipedia.org/wiki/Variable-gain_amplifier)  
4. All About Circuits - [Operational Amplifiers](https://www.allaboutcircuits.com/textbook/experiments/chpt-5/simple-op-amp/)  

---

This structure **preserves the original format** and allows you to **easily attach images**. Let me know if you need any changes! 🚀  
