# README for NOANbot Interface

This documentation provides an overview of the NOANbotInterface code, a user-friendly interface that allows interaction with the OpenAI GPT-3.5 Turbo model through the OpenAI API, utilizing Tkinter for the graphical user interface (GUI).

## GENERAL DESCRIPTION

The **NOANbotInterface** is designed to provide a simple chat interface between the user and the GPT-3.5 Turbo model. This interface allows the user to type messages into a text box, which are then sent to the model, and the model's responses are displayed in a chat-like format. The entire conversation history is saved and shown in the interface.

This project utilizes **Tkinter**, Python's built-in library for creating GUIs, and **OpenAI's GPT-3.5 Turbo API** for natural language processing. The interface is intuitive, featuring a text entry field for user input and a chat display area for model responses.

![Show](images/read1.png)  
![Show](images/read2.png)  

## SYSTEM REQUIREMENTS

Before running the code, ensure you have the following prerequisites:

- **Python 3.x**: Python version 3.x (preferably 3.7 or higher) is required to execute the script.
- **OpenAI API Key**: You must have an active account with OpenAI and obtain an API key to interact with GPT-3.5 Turbo.

### Supported Operating Systems

The code is compatible with:

- Windows
- macOS
- Linux

## REQUIRED PYTHON LIBRARIES

The following Python libraries are required to run this project:

- **Tkinter**: A standard Python library used for creating the GUI.
  - Tkinter comes pre-installed with Python on most systems, but if it is missing, you can install it via your system's package manager.

- **OpenAI**: The official OpenAI Python package for interacting with the GPT-3.5 Turbo API.
  - Install this package via pip:  

  ```bash
  pip install openai
  ```

## INSTALLATION

1. Clone or download the project to your local machine.

   If cloning, run:

   ```bash
   git clone <repository_url>
   ```

2. Install the required Python libraries if they are not already installed:

   ```bash
   pip install openai
   ```

3. Set up your OpenAI API key:

   - Go to OpenAI's API page and sign up or log in to your OpenAI account. Obtain your API key from the dashboard.
   - Open the script and replace `"YOUR_API_KEY"` with your actual OpenAI API key:

   ```python
   openai.api_key = "YOUR_API_KEY"
   ```

## USAGE

1. Run the script: Once the environment is set up and the API key is configured, you can run the Python script:

   ```bash
   python noanbot_interface.py
   ```

2. Using the Interface:

   - Upon running the script, a GUI window will open.
   - **Text area**: Displays the ongoing conversation between you and NOANbot.
   - **Input field**: A place where you can type your message.
   - **Send button ("→")**: Click this button to send your message to the GPT-3.5 model.

3. Interaction:

   - Type your question or message in the input area and click the "→" button to submit.
   - The response from NOANbot will appear in the conversation area.

4. Conversation History:

   - All messages exchanged between you and NOANbot will be displayed in the chat history.
   - The history is stored in memory during the session and shown in the chat window.

## USING A VIRTUAL MACHINE (VM) ON LINUX

This project has been tested on a **Linux virtual machine (VM)**. The steps below outline how to set up the environment in a VM:

### Setting Up a Virtual Machine:

1. **Install VirtualBox or VMware**: If you don’t already have a VM setup, install VirtualBox or VMware.
2. **Download a Linux Distribution**: You can use Ubuntu, Debian, or any other Linux-based OS.
3. **Create a New Virtual Machine**: Allocate at least **2GB RAM** and **10GB disk space**.
4. **Install Python** (if not pre-installed):

   ```bash
   sudo apt update && sudo apt install python3 python3-pip -y
   ```

5. **Clone the Project** into the VM:

   ```bash
   git clone <repository_url>
   cd NOANbotInterface
   ```

6. **Install Dependencies**:

   ```bash
   pip install openai
   ```

7. **Run the Application**:

   ```bash
   python noanbot_interface.py
   ```

![VM Setup](images/vm_setup.png)  
![Running in Linux VM](images/linux_vm.png)  

## CODE STRUCTURE

The code is structured into several main components for ease of understanding and maintenance:

### `NOANbotInterface` Class

This class manages the GUI and controls the interactions between the user and the OpenAI model.  
It initializes the GUI components, handles user inputs, and updates the conversation window.

### `send_message` Method

- This method is triggered when the user clicks the "→" button.
- It takes the user’s input, sends it to the OpenAI API, and retrieves the model’s response.
- The response is then displayed in the conversation area.

### `display_message` Method

- This method formats the chat messages and appends them to the conversation window.
- It distinguishes between user messages and model responses, ensuring proper alignment and display.

## HOW IT WORKS

1. **User Input**: The user types a message into the input area of the GUI.
2. **Sending the Message**: When the user clicks the send button, the message is sent to the OpenAI API.
3. **Processing**: The OpenAI model processes the input, generates a response, and returns it.
4. **Displaying the Response**: The response is then displayed in the conversation area of the GUI.
5. **Conversation History**: Each new message is added to the conversation window, keeping track of the entire chat history.

## TROUBLESHOOTING

- **No API Key**: Ensure that the API key is correctly set in the script. If the key is missing or incorrect, you will receive an error when attempting to connect to the API.
- **Tkinter Errors**: If Tkinter is not installed, you may encounter an ImportError. Ensure Tkinter is installed using your system’s package manager or by reinstalling Python with Tkinter support.
- **OpenAI API Errors**: If you receive errors related to the OpenAI API (e.g., quota exceeded, invalid API key), check your API key and review your OpenAI account's usage and limits.

