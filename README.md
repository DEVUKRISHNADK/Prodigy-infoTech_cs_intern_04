
---

# Keylogger Script

This Python script logs keystrokes on the system, recording them in a text file. It captures both standard keys and special keys, making it a basic yet functional keylogger. The script terminates when the "Esc" key is pressed.

## Introduction

This script uses the `pynput` library to monitor and log keyboard input. Each keypress is recorded into a text file (`key_log.txt`). The script also handles special keys (e.g., Enter, Shift, Esc) and stops logging when the "Esc" key is pressed.

## Features

- **Logs All Keystrokes:** Captures and logs both standard characters and special keys.
- **Stop Logging:** Stops the keylogger when the "Esc" key is pressed.
- **Simple and Lightweight:** The script is easy to use and requires minimal setup.

## Prerequisites

To run this script, you'll need:

- Python 3.x installed on your machine.
- The `pynput` library, which can be installed using pip.

## Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/keylogger.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Prodigy-infoTech_cs_intern_04
   ```

3. Install the required `pynput` library:

   ```bash
   pip install pynput
   ```

## Usage

1. Run the script using Python:

   ```bash
   python keylogger.py
   ```

2. The script will start capturing and logging keystrokes. All keys pressed will be recorded in a file named `key_log.txt` in the same directory as the script.

3. To stop the keylogger, press the "Esc" key.

### Example:

```bash
# When typing "Hello, World!" on the keyboard
key_log.txt content:
H e l l o ,   W o r l d !
```

## Functions Overview

- **on_press(key):**
  - **Description:** Logs each key press into the `key_log.txt` file.
  - **Arguments:**
    - `key`: The key that was pressed.
  
- **on_release(key):**
  - **Description:** Stops the keylogger when the "Esc" key is pressed.
  - **Arguments:**
    - `key`: The key that was released.

- **Listener:** A `pynput` listener that listens for key presses and releases.

## File Structure

```bash
.
├── keylogger.py       # Main keylogger script
├── key_log.txt        # File where keystrokes will be logged (created after running the script)
└── README.md          # This README file
```

---

### Notes:
- Replace `"https://github.com/your-username/keylogger.git"` with your actual GitHub repository URL.
- Ensure that you understand and comply with all legal requirements before using this script.
