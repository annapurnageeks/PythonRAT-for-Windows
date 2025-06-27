
# PythonRAT for Windows

> ⚠️ **Disclaimer:**  
> This project is for **educational and research purposes only**. Unauthorized use to access or control systems without explicit permission is **illegal** and **unethical**. The author is not responsible for any misuse or damage caused by this software. Ensure compliance with all applicable laws and regulations.

## 🧠 About

**PythonRAT** is a Windows-compatible Remote Access Tool written in Python. It enables remote interaction with a Windows system using Telegram bot commands. It offers features like webcam access, screenshot capture, system information retrieval, file encryption/decryption, clipboard access, remote shell, and Wi-Fi password extraction.

## ✨ Features

- 🖥️ Screen capture
- 🎥 Webcam access
- 💻 System information
- 📁 File management (list, upload, navigate)
- 🔐 File encryption/decryption with secure deletion
- 📋 Clipboard text retrieval
- 📡 Retrieve saved Wi-Fi passwords
- 🗣️ Text-to-speech
- 🔒 Lock Windows session
- 💬 Remote shell execution
- 📎 Upload any file via Telegram bot
- ⏻ System shutdown (5-second timer)

## 🛠️ Prerequisites

- Python 3.12 or higher
- Telegram Bot Token from [@BotFather](https://t.me/BotFather)
- Windows OS
- Required Libraries:

```bash
pip install mss opencv-python numpy pyttsx3 telebot pyAesCrypt secure_delete pyperclip Pillow clipboard
```

## 🚀 Installation

1. **Clone the Repository**:
```bash
git clone https://github.com/your-username/PythonRAT-Windows.git
cd PythonRAT-Windows
```

2. **Install Dependencies**:
```bash
pip install -r requirements.txt
```
Or install them manually.

3. **Configure the Telegram Bot**:
Open `PythonRAT.py` and replace:
```python
TOKEN = 'your_bot_token_here'
```
with your own bot token from BotFather.

4. **Run the Script**:
```bash
python PythonRAT.py
```

## 📱 Usage (Telegram Bot Commands)

/start – Start the bot  
/help – List available commands  
/screen – Capture and send a screenshot  
/webcam – Capture webcam image  
/sys – Get system information  
/ip – Get public IP address  
/cd [folder] – Change working directory  
/ls – List contents of the current directory  
/upload [path] – Upload a file from the victim's system  
/crypt [path] – Encrypt files in a folder  
/decrypt [path] – Decrypt files in a folder  
/lock – Lock the Windows session  
/shell – Open remote shell session (type `exit` to leave)  
/wifi – Get saved Wi-Fi SSIDs and passwords  
/speech [text] – Convert text to speech  
/clipboard – Read system clipboard  
/shutdown – Shutdown the system in 5 seconds

## 🔒 Notes on Windows Usage

- **Permissions**: Webcam and screen capture may require additional permissions.
- **Encryption**: Uses AES crypt with a hardcoded password (`softwarica`).
- **WiFi Dumping**: Requires elevated privileges to export WLAN profiles.
- **Safe File Removal**: Uses `secure_delete` to securely wipe original files.
- **Bot Polling**: `infinity_polling()` keeps the bot online indefinitely.

## 🧪 Debugging

- Add logging for more verbose output:
```python
import logging
logging.basicConfig(level=logging.DEBUG)
```

## ❗ Security & Ethical Reminder

- Do **NOT** use on unauthorized systems.
- Do **NOT** share your Telegram bot token publicly.
- The author assumes **no responsibility** for misuse.

## 🧾 License

MIT License © 2025 Your Name
