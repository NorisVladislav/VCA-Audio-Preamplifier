# Audio Preamplifier with Voltage-Controlled Gain

## Project Overview

This project focuses on designing and implementing an **audio preamplifier with voltage-controlled gain (VCA)**. The preamplifier allows dynamic control of signal amplification through an external voltage, eliminating the need for mechanical adjustments. The implementation follows modern industry standards, ensuring high-quality audio processing with minimal distortion.

## Table of Contents

1. [Introduction](#introduction)  
2. [Project Specifications](#project-specifications)  
3. [Technical Details](#technical-details)  
4. [SMT & PCB Design](#smt--pcb-design)  
5. [Usage Instructions](#usage-instructions)  
6. [Conclusion](#conclusion)  
7. [References](#references)  

---

## Introduction

A **voltage-controlled amplifier (VCA)** is a crucial component in audio signal processing, enabling precise gain control using an external control voltage. This makes VCAs essential for applications such as mixing, dynamic compression, and sound effect processing. 

This project aims to develop a compact VCA-based preamplifier capable of handling sinusoidal input signals. The amplification is fully controlled by an external voltage while maintaining stability and linearity. The project also integrates **Surface-Mount Technology (SMT)** for PCB design, ensuring a robust and compact implementation that adheres to **IPC-2221A and IPC-A-610** industry standards.

---

## Project Specifications

The designed **audio frequency preamplifier with voltage control** has the following characteristics:

- **Power Supply:** 12V single supply (VCC) or ±12V dual supply (VCC = +12V, VEE = -12V).
- **Input Signal:** Sinusoidal, amplitude between 0 and 20mV.
- **Input Frequency:** 2 kHz.
- **Control Voltage Range:** 0V to 2V.
- **Voltage Gain:** Adjustable between **1x and 20x**.
- **Load Resistance:** 700Ω.
- **Power Indicator:** LED for voltage presence.

---

## Technical Details

### Block Diagram

1. **Sinusoidal Signal Input**  
   - Accepts an input signal of 20mV amplitude at 2kHz.  

2. **Amplifier Stage 1 (Pre-Amplification)**  
   - Boosts the signal to an intermediate level while reducing noise.

3. **Amplifier Stage 2 (Voltage-Controlled Amplification)**  
   - Controls gain based on the applied voltage:
     - **0V Control Voltage → Gain = 1x (Buffer Mode)**
     - **2V Control Voltage → Gain = 20x (Maximum Amplification)**  

4. **Control Voltage Source**  
   - Provides a stable voltage between 0V and 2V to regulate amplification.

5. **Power Indicator LED**  
   - Signals the presence of power to the circuit.

6. **Power Supply**  
   - Provides the necessary 12V DC for circuit operation.

7. **Load Resistance (700Ω)**  
   - Ensures proper impedance matching for signal output.

8. **Amplified Signal Output**  
   - Delivers the amplified sinusoidal signal.

---

## SMT & PCB Design

The preamplifier is designed using **Surface-Mount Technology (SMT)** to minimize size and enhance reliability. The PCB layout includes:

- **Top and Bottom Layer Interconnects**
- **Silkscreen Mask for Component Placement**
- **Solder Mask and Paste Stencil for SMT Assembly**
- **Drilling and Cutting Layers for PCB Fabrication**
- **Mechanical and Electrical Layer Comparisons**

The PCB follows **best practices for SMT soldering**, ensuring durability and precision.

---

## Usage Instructions

### Power Connection:
1. Connect all **negative terminals** of the power supply and input signal to **GND**.
2. Apply **12V DC** to power the circuit.
3. Connect the sinusoidal input signal to the **"IN" terminal**.

### Gain Adjustment:
- Control gain by applying a **voltage between 0V and 2V** to the control terminal:
  - **0V → Gain = 1x (No amplification)**
  - **2V → Gain = 20x (Maximum amplification)**
- Use a **stable voltage source** for optimal performance.

### Safety Precautions:
- **Do not modify or touch** components while the circuit is powered.
- **Handle the PCB carefully** to prevent electrostatic discharge or damage.
- **Avoid moisture, extreme temperatures, and prolonged sunlight exposure.**

### Operating Conditions:
- **Recommended Ambient Temperature:** 25°C
- **Safe Operating Range:** -20°C to 70°C

---

## Conclusion

The **Audio Preamplifier with Voltage-Controlled Gain** is a functional and adaptable solution for precise audio signal amplification. The project successfully demonstrates:

- **Stable and precise gain control** with minimal distortion.
- **Versatile application** in audio processing, mixing, and equalization.
- **Compact SMT-based PCB design** compliant with industry standards.

This preamplifier is a valuable tool for **audio electronics research, education, and professional applications**.

---

## References

- G. Brezeanu, F. Drăghici - *Fundamental Electronic Circuits*, Niculescu Publishing, Bucharest, 2013.
- Dan Dascălu - *Electronic Devices and Circuits*, Didactic & Pedagogical Publishing, Bucharest, 1982.
- Wikipedia - [Variable-Gain Amplifier](https://en.wikipedia.org/wiki/Variable-gain_amplifier)
- All About Circuits - [Operational Amplifiers](https://www.allaboutcircuits.com/textbook/experiments/chpt-5/simple-op-amp/)
- Electronics Tutorials - [Op-Amp Basics](https://www.electronics-tutorials.ws/opamp/opamp_1.html)
