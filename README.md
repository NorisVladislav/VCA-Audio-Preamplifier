# National University of Science and Technology POLITEHNICA Bucharest  
## Faculty of Electronics, Telecommunications, and Information Technology  
# README for NOANbot Interface

### Academic Year 2024-2025  
This documentation provides an overview of the NOANbotInterface code, a user-friendly interface that allows interaction with the OpenAI GPT-3.5 Turbo model through the OpenAI API, utilizing Tkinter for the graphical user interface (GUI).

---
## GENERAL DESCRIPTION

# Project 1  
The **NOANbotInterface** is designed to provide a simple chat interface between the user and the GPT-3.5 Turbo model. This interface allows the user to type messages into a text box, which are then sent to the model, and the model's responses are displayed in a chat-like format. The entire conversation history is saved and shown in the interface.

## Design and Implementation of an Audio Preamplifier with Voltage-Controlled Gain  
This project utilizes **Tkinter**, Python's built-in library for creating GUIs, and **OpenAI's GPT-3.5 Turbo API** for natural language processing. The interface is intuitive, featuring a text entry field for user input and a chat display area for model responses.

**Group:** 432B  
**Supervisors:**  
- Prof. Dr. Eng. Dragoș Dobrescu  
- Lecturer Dr. Eng. Mădălin Moise  
![Show](images/read1.png)  
![Show](images/read2.png)  

---
## SYSTEM REQUIREMENTS

## Table of Contents  
Before running the code, ensure you have the following prerequisites:

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
- **Python 3.x**: Python version 3.x (preferably 3.7 or higher) is required to execute the script.
- **OpenAI API Key**: You must have an active account with OpenAI and obtain an API key to interact with GPT-3.5 Turbo.

---
### Supported Operating Systems

## Introduction  
The code is compatible with:

A **Voltage-Controlled Amplifier (VCA)** is an essential component in audio signal processing, allowing dynamic control of amplification without mechanical intervention. This technology is crucial for applications such as **mixing, dynamic compression, and audio effects processing**.  
- Windows
- macOS
- Linux

This project focuses on designing a **compact VCA-based audio preamplifier** with **precise gain control via an external voltage**. The implementation ensures high stability and linearity of the output signal. Additionally, the **use of Surface-Mount Technology (SMT) for PCB design** provides a compact and robust solution that complies with **IPC-2221A and IPC-A-610** industry standards.  
## REQUIRED PYTHON LIBRARIES

---
The following Python libraries are required to run this project:

## Initial Project Data  
- **Tkinter**: A standard Python library used for creating the GUI.
  - Tkinter comes pre-installed with Python on most systems, but if it is missing, you can install it via your system's package manager.

### Project Description  
- **OpenAI**: The official OpenAI Python package for interacting with the GPT-3.5 Turbo API.
  - Install this package via pip:  

The goal is to design and implement a **voltage-controlled audio preamplifier** with the following characteristics:  
  ```bash
  pip install openai
  ```

- **Power Supply:** 12V 
- **Input Signal:** Sinusoidal, 0-20mV amplitude  
- **Frequency:** 2 kHz  
- **Control Voltage:** 0V to 2V  
- **Gain Range:** 1x to 20x  
- **Load Resistance:** 700Ω  
- **LED Indicator:** For power supply presence  
## INSTALLATION

### Block Diagram of the Electrical Circuit  
1. Clone or download the project to your local machine.

![Block Diagram](images/aa.png)  
   If cloning, run:

---
   ```bash
   git clone <repository_url>
   ```

## Technical Content  
2. Install the required Python libraries if they are not already installed:

### Electrical Circuit Diagram  
   ```bash
   pip install openai
   ```

![Electrical Schematic](images/SCHMA.png)  
![Electrical Schematic](images/SCHMB.png) 
3. Set up your OpenAI API key:

### Simulation of the Audio Preamplifier  
   - Go to OpenAI's API page and sign up or log in to your OpenAI account. Obtain your API key from the dashboard.
   - Open the script and replace `"YOUR_API_KEY"` with your actual OpenAI API key:

- **Vcontrol = 0V → Gain = 1x (Buffer Mode)**  
- **Vcontrol = 2V → Gain = 20x (Maximum Amplification)**  
   ```python
   openai.api_key = "YOUR_API_KEY"
   ```

![Simulation Results](images/SIMA.png)  
![Simulation Results](images/SIMB.png)  
## USAGE

### Static Operating Points  
1. Run the script: Once the environment is set up and the API key is configured, you can run the Python script:

![Static Operating Points](images/STAT1.png)  
![Static Operating Points](images/STAT2.png) 
![Static Operating Points](images/STAT3.png) 
   ```bash
   python noanbot_interface.py
   ```

### Analytical Calculation of PSF  
2. Using the Interface:

![Analytical PSF](images/31.jpg) 
![Analytical PSF](images/30.jpg) 
![Analytical PSF](images/33.jpg) 
![Analytical PSF](images/32.jpg) 
![Analytical PSF](images/34.jpg) 
![Analytical PSF](images/35.jpg) 
![Analytical PSF](images/36.jpg) 
   - Upon running the script, a GUI window will open.
   - **Text area**: Displays the ongoing conversation between you and NOANbot.
   - **Input field**: A place where you can type your message.
   - **Send button ("→")**: Click this button to send your message to the GPT-3.5 model.

3. Interaction:

### Bill of Materials  
   - Type your question or message in the input area and click the "→" button to submit.
   - The response from NOANbot will appear in the conversation area.

![BOM](images/BOM.png) 
4. Conversation History:

## PCB Design using SMT Technology  
   - All messages exchanged between you and NOANbot will be displayed in the chat history.
   - The history is stored in memory during the session and shown in the chat window.

### General Layout  
## USING A VIRTUAL MACHINE (VM) ON LINUX

![PCB Layout](images/LAYOUT.png)  
![PCB Layout](images/0.png)  
This project has been tested on a **Linux virtual machine (VM)**. The steps below outline how to set up the environment in a VM:

### Top and Bottom Layer Interconnection  
### Setting Up a Virtual Machine:

![Top Layer](images/1.jpg)  
![Bottom Layer](images/2.jpg)  
1. **Install VirtualBox or VMware**: If you don’t already have a VM setup, install VirtualBox or VMware.
2. **Download a Linux Distribution**: You can use Ubuntu, Debian, or any other Linux-based OS.
3. **Create a New Virtual Machine**: Allocate at least **2GB RAM** and **10GB disk space**.
4. **Install Python** (if not pre-installed):

### Silkscreen, Solder Mask, and Stencil  
   ```bash
   sudo apt update && sudo apt install python3 python3-pip -y
   ```

- **Silkscreen Layer (SSTOP)**  
  ![Silkscreen](images/3.jpg)  
5. **Clone the Project** into the VM:

- **Solder Mask Layer (SMTOP, SMBOT)**  
  ![Solder Mask](images/4.jpg)
  ![Solder Mask](images/6.jpg) 
   ```bash
   git clone <repository_url>
   cd NOANbotInterface
   ```

- **Solder Paste Stencil (SPTOP)**  
  ![Stencil](images/5.jpg)  
6. **Install Dependencies**:

### Drill and Cutting Layers  
   ```bash
   pip install openai
   ```

- **Drill Holes (DRILL)**  
  ![Drill Layer](images/8.jpg)  
7. **Run the Application**:

- **Cutting Layer (BO)**  
  ![Cutting Layer](images/9.jpg)  
   ```bash
   python noanbot_interface.py
   ```

### Mechanical Layer (FAB)  
![VM Setup](images/vm_setup.png)  
![Running in Linux VM](images/linux_vm.png)  

![Mechanical Layer](images/7.jpg)  
## CODE STRUCTURE

### Stacked
The code is structured into several main components for ease of understanding and maintenance:

- **TOP - SPTOP**
  ![TOP SPTOP](images/10.jpg)
### `NOANbotInterface` Class

- **TOP - SMTOP**
  ![TOP SMTOP](images/11.jpg)
This class manages the GUI and controls the interactions between the user and the OpenAI model.  
It initializes the GUI components, handles user inputs, and updates the conversation window.

- **TOP - BOT**
  ![TOP BOT](images/13.jpg)
### `send_message` Method

- **SMTOP - SSTOP**
  ![TOP SSTOP](images/12.jpg)
- This method is triggered when the user clicks the "→" button.
- It takes the user’s input, sends it to the OpenAI API, and retrieves the model’s response.
- The response is then displayed in the conversation area.

- **TOP - DRILL**
  ![TOP DRILL](images/14.jpg) 
### `display_message` Method

---
- This method formats the chat messages and appends them to the conversation window.
- It distinguishes between user messages and model responses, ensuring proper alignment and display.

## Assembly and Soldering Process  
## HOW IT WORKS

- **Required Tools:**  
  - Soldering station  
  - Solder wire (SnAgCu alloy)  
  - Flux and desoldering braid  
1. **User Input**: The user types a message into the input area of the GUI.
2. **Sending the Message**: When the user clicks the send button, the message is sent to the OpenAI API.
3. **Processing**: The OpenAI model processes the input, generates a response, and returns it.
4. **Displaying the Response**: The response is then displayed in the conversation area of the GUI.
5. **Conversation History**: Each new message is added to the conversation window, keeping track of the entire chat history.

- **Soldering Procedure:**  
  1. Set soldering iron temperature to **370°C**.  
  2. Apply flux and solder components.  
  3. Use a desoldering braid to remove excess solder if needed.  
## TROUBLESHOOTING

---
- **No API Key**: Ensure that the API key is correctly set in the script. If the key is missing or incorrect, you will receive an error when attempting to connect to the API.
- **Tkinter Errors**: If Tkinter is not installed, you may encounter an ImportError. Ensure Tkinter is installed using your system’s package manager or by reinstalling Python with Tkinter support.
- **OpenAI API Errors**: If you receive errors related to the OpenAI API (e.g., quota exceeded, invalid API key), check your API key and review your OpenAI account's usage and limits.

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
