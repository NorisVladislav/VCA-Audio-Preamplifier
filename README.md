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
   - [Stacked]
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

![Static Operating Points](images/STAT1.png)  
![Static Operating Points](images/STAT2.png) 
![Static Operating Points](images/STAT3.png) 

### Analytical Calculation of PSF  

![Analytical PSF](images/31.jpg) 
![Analytical PSF](images/30.jpg) 
![Analytical PSF](images/33.jpg) 
![Analytical PSF](images/32.jpg) 
![Analytical PSF](images/34.jpg) 
![Analytical PSF](images/35.jpg) 
![Analytical PSF](images/36.jpg) 


### Bill of Materials  

![BOM](images/BOM.png) 

## PCB Design using SMT Technology  

### General Layout  

![PCB Layout](images/LAYOUT.png)  
![PCB Layout](images/0.png)  

### Top and Bottom Layer Interconnection  

![Top Layer](images/1.jpg)  
![Bottom Layer](images/2.jpg)  

### Silkscreen, Solder Mask, and Stencil  

- **Silkscreen Layer (SSTOP)**  
  ![Silkscreen](images/3.jpg)  

- **Solder Mask Layer (SMTOP, SMBOT)**  
  ![Solder Mask](images/4.jpg)
  ![Solder Mask](images/6.jpg) 

- **Solder Paste Stencil (SPTOP)**  
  ![Stencil](images/5.jpg)  

### Drill and Cutting Layers  

- **Drill Holes (DRILL)**  
  ![Drill Layer](images/8.jpg)  

- **Cutting Layer (BO)**  
  ![Cutting Layer](images/9.jpg)  

### Mechanical Layer (FAB)  

![Mechanical Layer](images/7.jpg)  

### Stacked

- **TOP - SPTOP**
  ![TOP SPTOP](images/10.jpg)

- **TOP - SMTOP**
  ![TOP SMTOP](images/11.jpg)

- **TOP - BOT**
  ![TOP BOT](images/13.jpg)

- **SMTOP - SSTOP**
  ![TOP SSTOP](images/12.jpg)

- **TOP - DRILL**
  ![TOP DRILL](images/14.jpg) 

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
