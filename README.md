
```markdown
<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=30&duration=3000&pause=500&color=00FF00&center=true&vCenter=true&width=500&lines=ERROR+MASK+PRO;Android+Pentesting+Toolkit;Fully+Automated+%26+Real" alt="Typing SVG" />
</p>

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Stars-⭐-yellow?style=flat-square" alt="Stars"></a>
  <a href="#"><img src="https://img.shields.io/badge/Forks-🍴-orange?style=flat-square" alt="Forks"></a>
  <a href="#"><img src="https://img.shields.io/badge/License-MIT-blue?style=flat-square" alt="License"></a>
  <a href="#"><img src="https://img.shields.io/badge/Python-3.8%2B-brightgreen?style=flat-square&logo=python&logoColor=white" alt="Python"></a>
  <a href="#"><img src="https://img.shields.io/badge/Metasploit-Required-red?style=flat-square&logo=metasploit" alt="Metasploit"></a>
  <a href="#"><img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20macOS-lightgrey?style=flat-square" alt="Platform"></a>
</p>

---

## 🚀 Overview

**ERROR MASK PRO** is a **100% real, fully automated** terminal-based penetration testing toolkit designed for **Android security assessments**. It streamlines the entire red-team workflow:

- Binds a Metasploit payload to any legitimate APK (`msfvenom -x`)
- Applies military-grade **AES-256 encryption** for AV evasion
- Automatically spins up an `msfconsole` listener
- Guides you through **post-exploitation** with 10+ Meterpreter commands

> **⚠️ Disclaimer:** This tool is intended for **authorized security testing, educational research, and CTF challenges only**. The authors are not responsible for any misuse. Always obtain explicit permission before testing any device.

---

## ✨ Features

| Category | Feature | Status |
| :--- | :--- | :---: |
| **🤖 Automation** | One-command "Full Auto Attack" (Bind + Encrypt + Listen) | ✅ |
| **📱 Payload Binding** | Real APK binding using `msfvenom -x` | ✅ |
| **🔐 Cryptography** | AES-256-CBC real encryption & decryption (PyCryptodome) | ✅ |
| **📦 APK Signing** | Auto-sign with `jarsigner` (Debug keystore) | ✅ |
| **📡 Listener** | Auto-start `msfconsole` handler in a separate terminal | ✅ |
| **🎯 Post-Exploit** | 10+ interactive Meterpreter command guides (Geo, SMS, Call, Mic, etc.) | ✅ |
| **📂 Session Manager** | Save/load previous sessions with timestamps | ✅ |
| **📜 Logging** | Complete activity logging in JSON format | ✅ |
| **🛡️ Fallback Mode** | Pure Python reverse shell (No Metasploit required) | ✅ |
| **⚡ Self-Managed** | Auto-installs Python packages & system dependencies (Metasploit, Java) | ✅ |
| **🎨 UI/UX** | Beautiful Terminal UI with Rich, PyFiglet, and Colorama | ✅ |
| **🌍 Cross-Platform** | Works on Linux, Windows, and macOS | ✅ |

---

## 📸 Screenshots

<p align="center">
  <img src="https://via.placeholder.com/800x400?text=Main+Menu+Preview" alt="Main Menu" width="80%">
  <br>
  <em>🔹 The stunning terminal interface with ASCII art banner.</em>
</p>

<p align="center">
  <img src="https://via.placeholder.com/800x400?text=Full+Auto+Attack+in+Progress" alt="Auto Attack" width="80%">
  <br>
  <em>🔹 Fully automated bind + encrypt + listener sequence.</em>
</p>

> *Replace the placeholder links with actual screenshots from your terminal!*

---

## 🛠️ Prerequisites

The tool is designed to manage dependencies itself. However, to run smoothly, ensure you have:

- **Python 3.8+** installed.
- **Internet Connection** (for auto-installing packages and Metasploit).
- **Root/Sudo privileges** (required on Linux for installing system packages).

---

## 📥 Installation & Usage

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/error-mask-pro.git
cd error-mask-pro
```

### Step 2: Run the Tool
You only need **one command**. The script will automatically handle everything else.
```bash
sudo python3 final_error_mask.py
```

**What happens next?**
1. Script checks for `msfvenom`, `jarsigner`, and `keytool`.
2. If missing, it runs `sudo apt update && sudo apt install -y metasploit-framework openjdk-17-jdk`.
3. It installs all Python libraries (`rich`, `pycryptodome`, `psutil`, etc.).
4. The beautiful main menu appears.

### Step 3: Choose Your Attack

- Press **[1]** for the **Full Auto Attack** (Recommended).
- Follow the prompts:
  - **LHOST**: Your local IP address (e.g., `192.168.1.100`).
  - **LPORT**: The port to listen on (e.g., `4444`).
  - **Path to APK**: Provide a legitimate Android APK file to bind the payload with (e.g., `~/Downloads/game.apk`).

---

## 🔧 How It Works (Technical Breakdown)

1. **Binding (`msfvenom -x`)**
   The tool takes your legitimate APK and injects the `android/meterpreter/reverse_tcp` payload using the `-x` (embed) flag. This creates a hybrid APK that retains the original app's functionality while running a backdoor in the background.

2. **Signing (`jarsigner`)**
   Android devices refuse to install unsigned APKs. The script automatically generates a debug keystore and signs the hybrid APK, bypassing installation barriers (as long as "Unknown Sources" is enabled).

3. **AES-256 Encryption**
   To bypass antivirus scanners (AV Evasion), the bound APK is encrypted using AES-256-CBC with a hardcoded password (`ErrorMask2025`). The encrypted file is saved with a `.enc` extension.

4. **Listener (`msfconsole`)**
   A resource file (`.rc`) is generated to launch `msfconsole` with the exact payload settings (`LHOST`, `LPORT`). It automatically opens in a new terminal window (or runs in the background) and waits for the victim device to connect.

5. **Post-Exploitation**
   Once a session is established, the tool provides a guide to run critical Meterpreter commands like `geolocate`, `dump_sms`, `webcam_snap`, `keyscan_start`, and more.

---

## 🚨 Fallback Mode (No Metasploit!)

If your system does not have Metasploit installed and the auto-installer fails, **ERROR MASK PRO** falls back to a **Pure Python Reverse Shell**.

- Generates a lightweight `payload.py` that uses Python's `socket` and `subprocess` modules.
- Creates a Python-based listener (`listener.py`).
- Perfect for environments where installing the full Metasploit framework is overkill or restricted.

---

## ⚙️ Commands & Options

Run `sudo python3 final_error_mask.py` and navigate the interactive menu:

| Option | Description |
| :--- | :--- |
| `1` | **Full Auto Attack**: Bind + Encrypt + Listener + Post-Exploit Menu. |
| `2` | **Bind APK Only**: Just inject the payload (no encryption). |
| `3` | **Encrypt APK Only**: Encrypt an existing APK with AES-256. |
| `4` | **Decrypt APK**: Decrypt a previously encrypted `.enc` file. |
| `5` | **Start Listener**: Manually start `msfconsole` with custom IP/Port. |
| `6` | **Kill All Listeners**: Forcefully terminate all running `msfconsole` processes. |
| `7` | **Sessions Manager**: View saved attack sessions. |
| `8` | **View Logs**: Check recent activity logs. |
| `9` | **Fallback Mode**: Generate pure Python payload/listener. |
| `0` | **Exit**: Clean shutdown & cleanup. |

---

## 📂 File Structure

```
error-mask-pro/
├── final_error_mask.py   # Main script
├── debug.keystore        # Auto-generated signing keystore
├── error_mask_config.json # Session history
├── error_mask_log.json   # Activity logs
├── bound_*.apk           # Generated bound APKs
├── *.apk.enc             # Encrypted APKs
└── listener_*.rc         # msfconsole resource files
```

---

## 📝 Legal & Ethical Notice

```
###################################################
#  THIS SOFTWARE IS PROVIDED FOR EDUCATIONAL USE  #
#  AND AUTHORIZED PENETRATION TESTING ONLY.        #
#                                                  #
#  Unauthorized access to systems or devices is   #
#  a criminal offense. The user assumes full      #
#  responsibility for any misuse.                 #
###################################################
```

- You must have **written authorization** to test any device.
- Use this exclusively on your own devices or in a lab environment.
- The developers are **not liable** for any illegal activity performed with this tool.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

- [Metasploit Framework](https://www.metasploit.com/)
- [Rich](https://github.com/Textualize/rich) for the beautiful TUI.
- [PyCryptodome](https://www.pycryptodome.org/) for AES encryption.
- All security researchers who push the boundaries of ethical hacking.

---

<p align="center">
  <b>Made with 💻 & ❤️ for the cybersecurity community.</b><br>
  <i>Stay Ethical, Stay Legal, Stay Safe.</i>
</p>
```

---
