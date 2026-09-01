
<div align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=32&duration=3000&pause=500&color=00FF66&center=true&vCenter=true&width=650&lines=ERROR+MASK+PRO;Android+Pentesting+Toolkit;Fully+Automated+%26+Advanced+Red-Ops" alt="Typing SVG" />

  <p>
    <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=500&size=16&duration=4000&pause=1000&color=3399FF&center=true&vCenter=true&width=500&lines=Secure+The+Future+Through+Penetration+Testing;Automate+Your+Red-Teaming+Workflow" alt="Typing SVG"></a>
  </p>

</div>

---

<p align="center">
  <img src="https://img.shields.io/badge/Version-3.0.0-blueviolet?style=for-the-badge&logo=rocket&logoColor=white" alt="Version">
  <img src="https://img.shields.io/badge/Stars-⭐%20Trending-yellow?style=for-the-badge" alt="Stars">
  <img src="https://img.shields.io/badge/Forks-🍴%20Active-orange?style=for-the-badge" alt="Forks">
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="License">
  <img src="https://img.shields.io/badge/Python-3.8%2B-brightgreen?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Metasploit-Framework-red?style=for-the-badge&logo=metasploit&logoColor=white" alt="Metasploit">
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20macOS-lightgrey?style=for-the-badge&logo=linux&logoColor=white" alt="Platform">
</p>

---

## ⚡ Overview

<div align="center">

> **ERROR MASK** is an elite, terminal-based automated penetration testing framework built specifically for **Android security assessments**. Designed to supercharge red-team workflows with surgical precision.

</div>

- 🔥 **Dynamic Payload Integration:** Binds custom payloads seamlessly using `msfvenom -x`.
- 🛡️ **Military-Grade Obfuscation:** Applies AES-256 encryption to outsmart modern AV heuristics.
- 🚀 **Zero-Touch Automation:** Spins up handlers, signs packages, and tracks sessions autonomously.

> **⚠️ DISCLAIMER:** This software is intended strictly for **authorized security auditing, educational research, and isolated CTF environments**. The author assumes zero liability for unauthorized exploitation or misuse.

---

## ✨ Core Features & Matrix

| Module | Capability | Status |
| :--- | :--- | :---: |
| **🤖 Full-Auto Core** | One-command Bind + Encrypt + Listener deployment | `🟢 ACTIVE` |
| **📱 APK Hybridizer** | Native embedding via `msfvenom -x` | `🟢 ACTIVE` |
| **🔐 PyCryptodome** | Real AES-256-CBC encryption/decryption layers | `🟢 ACTIVE` |
| **📦 KeySigner** | Auto-signing via internal debug keystores & `jarsigner` | `🟢 ACTIVE` |
| **📡 Auto-Handler** | Independent `msfconsole` resource file generation | `🟢 ACTIVE` |
| **🎯 Post-Exploitation**| 10+ interactive Meterpreter command shortcuts | `🟢 ACTIVE` |
| **📂 Session Vault** | Timestamped session management & state preservation | `🟢 ACTIVE` |
| **📜 Audit Trails** | Comprehensive activity logging in structural JSON | `🟢 ACTIVE` |
| **🛡️ Fallback Engine**| Pure Python socket reverse-shell (No dependencies needed) | `🟢 ACTIVE` |
| **🎨 Advanced TUI** | High-performance interactive UI driven by Rich & PyFiglet | `🟢 ACTIVE` |

---

## 🛠️ System Prerequisites

Ensure your environment satisfies the baseline requirements before initializing:
- **Python 3.8+** runtime environment.
- **Active Network Access** (for dynamic package and framework fetching).
- **Sudo / Root Privileges** (mandatory for system-level dependency resolution on Linux distributions).

---

## 📥 Installation & Quick Start

### Step 1: Clone the Repository
```bash
git clone [https://github.com/ErrorMask101/Android.git](https://github.com/ErrorMask101/Android.git)
cd Android

```

### Step 2: Initialize Framework

Execute the master controller with administrative privileges:

```bash
sudo python3 android.py

```

### Step 3: Launch Attack Sequence

1. Choose option **[1]** for **Full Auto Attack**.
2. Input target network identifiers:
* **LHOST:** `192.168.x.x` (Your local bind address)
* **LPORT:** `4444` (Listening port)
* **APK Path:** Path to target APK (`/path/to/target.apk`)



---

## 🔧 Technical Architecture Breakdown

```
Target APK + Payload ──> [ msfvenom -x ] ──> Hybrid APK
                                                  │
Session Listener <── [ msfconsole .rc ] <── [ AES-256 Obfuscation ] <── [ Jarsigner ]

```

1. **Payload Embedding:** Injects reverse TCP logic into legitimate app architecture without breaking original runtime behavior.
2. **Cryptographic Wrapping:** Encrypts outputs using robust block ciphers (`ErrorMask2025` key standard) to bypass automated signature checks.
3. **Automated Handlers:** Automatically constructs configuration scripts (.rc files) to streamline listener management.

---

## ⚙️ Interactive Command Menu

```bash
sudo python3 final_error_mask.py

```

| Option | Command Reference | Action Execution |
| --- | --- | --- |
| **1** | Full Auto Attack | Bind + Encrypt + Listener + Post-Exploitation Suite |
| **2** | Bind APK Only | Inject payload core without cryptographic encryption |
| **3** | Encrypt Module | Secure standalone targets via AES-256 wrappers |
| **4** | Decrypt Module | Reverse `.enc` wrappers back to clean packages |
| **5** | Manual Listener | Standalone `msfconsole` process instantiator |
| **6** | Purge Listeners | Force-terminate active background socket listeners |
| **7** | Session Manager | Inspect historical payloads and active logs |
| **8** | Audit Logs | Review recent operations and system responses |
| **9** | Fallback Mode | Deploy lightweight pure Python reverse shell framework |
| **0** | Terminate | Safe exit and temporary cache cleanup |

---

## 📂 Project Directory Structure

```text
error-mask-pro/
├── 📄 final_error_mask.py     # Core application engine
├── 🔑 debug.keystore          # Built-in signing certificate
├── 📊 error_mask_config.json  # Persistent session storage
├── 📜 error_mask_log.json     # Execution & error logs
├── 📱 bound_*.apk             # Compiled payload-injected apps
├── 🔒 *.apk.enc               # Cryptographically secured builds
└── ⚙️ listener_*.rc           # Metasploit automated resource files

```

---

## 📝 Legal & Compliance Notice

```text
╔════════════════════════════════════════════════════════════════╗
║       [!] RESTRICTED ACCESS & EDUCATIONAL TOOLING [!]          ║
║                                                                ║
║   This framework is built strictly for authorized security     ║
║   testing, penetration assessments, and academic research.     ║
║   Unauthorized deployment against external devices is illegal. ║
╚════════════════════════════════════════════════════════════════╝

```

---

## 🤝 Community Contributions

Contributions, feature requests, and bug reports are open!

1. **Fork** the Project repository.
2. Create your Feature Branch (`git checkout -b feature/EliteModule`).
3. Commit your Changes (`git commit -m 'Add EliteModule capability'`).
4. Push to the Branch (`git push origin feature/EliteModule`).
5. Open a **Pull Request**.

---

## 📜 License & Acknowledgments

Distributed under the **MIT License**. See `LICENSE` for details.

* Special credits to the **Metasploit Framework**, **Rich TUI**, and **PyCryptodome** ecosystems.

---আপনার গিটহাবের README ফাইলটিকে আরও বেশি আই-ক্যাচিং, হাই-টেক অ্যানিমেশন সমৃদ্ধ এবং প্রো-লেভেল ডেভেলপার ভাইব দিতে এটি পুরোপুরি রি-ডিজাইন করা হয়েছে।

নিচের **`Copy Code`** বাটনে ক্লিক করে পুরো কোডটি এক ক্লিকেই কপি করে আপনার গিটহাবের ফাইলের ভেতর পেস্ট করে সেভ করে নিন! 🚀

```markdown
<div align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=32&duration=3000&pause=500&color=00FF66&center=true&vCenter=true&width=650&lines=ERROR+MASK+PRO;Android+Pentesting+Toolkit;Fully+Automated+%26+Advanced+Red-Ops" alt="Typing SVG" />

  <p>
    <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=500&size=16&duration=4000&pause=1000&color=3399FF&center=true&vCenter=true&width=500&lines=Secure+The+Future+Through+Penetration+Testing;Automate+Your+Red-Teaming+Workflow" alt="Typing SVG"></a>
  </p>

</div>

---

<p align="center">
  <img src="https://img.shields.io/badge/Version-3.0.0-blueviolet?style=for-the-badge&logo=rocket&logoColor=white" alt="Version">
  <img src="https://img.shields.io/badge/Stars-⭐%20Trending-yellow?style=for-the-badge" alt="Stars">
  <img src="https://img.shields.io/badge/Forks-🍴%20Active-orange?style=for-the-badge" alt="Forks">
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="License">
  <img src="https://img.shields.io/badge/Python-3.8%2B-brightgreen?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Metasploit-Framework-red?style=for-the-badge&logo=metasploit&logoColor=white" alt="Metasploit">
  <img src="https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20macOS-lightgrey?style=for-the-badge&logo=linux&logoColor=white" alt="Platform">
</p>

---

## ⚡ Overview

<div align="center">

> **ERROR MASK PRO** is an elite, terminal-based automated penetration testing framework built specifically for **Android security assessments**. Designed to supercharge red-team workflows with surgical precision.

</div>

- 🔥 **Dynamic Payload Integration:** Binds custom payloads seamlessly using `msfvenom -x`.
- 🛡️ **Military-Grade Obfuscation:** Applies AES-256 encryption to outsmart modern AV heuristics.
- 🚀 **Zero-Touch Automation:** Spins up handlers, signs packages, and tracks sessions autonomously.

> **⚠️ DISCLAIMER:** This software is intended strictly for **authorized security auditing, educational research, and isolated CTF environments**. The author assumes zero liability for unauthorized exploitation or misuse.

---

## ✨ Core Features & Matrix

| Module | Capability | Status |
| :--- | :--- | :---: |
| **🤖 Full-Auto Core** | One-command Bind + Encrypt + Listener deployment | `🟢 ACTIVE` |
| **📱 APK Hybridizer** | Native embedding via `msfvenom -x` | `🟢 ACTIVE` |
| **🔐 PyCryptodome** | Real AES-256-CBC encryption/decryption layers | `🟢 ACTIVE` |
| **📦 KeySigner** | Auto-signing via internal debug keystores & `jarsigner` | `🟢 ACTIVE` |
| **📡 Auto-Handler** | Independent `msfconsole` resource file generation | `🟢 ACTIVE` |
| **🎯 Post-Exploitation**| 10+ interactive Meterpreter command shortcuts | `🟢 ACTIVE` |
| **📂 Session Vault** | Timestamped session management & state preservation | `🟢 ACTIVE` |
| **📜 Audit Trails** | Comprehensive activity logging in structural JSON | `🟢 ACTIVE` |
| **🛡️ Fallback Engine**| Pure Python socket reverse-shell (No dependencies needed) | `🟢 ACTIVE` |
| **🎨 Advanced TUI** | High-performance interactive UI driven by Rich & PyFiglet | `🟢 ACTIVE` |

---

## 🛠️ System Prerequisites

Ensure your environment satisfies the baseline requirements before initializing:
- **Python 3.8+** runtime environment.
- **Active Network Access** (for dynamic package and framework fetching).
- **Sudo / Root Privileges** (mandatory for system-level dependency resolution on Linux distributions).

---

## 📥 Installation & Quick Start

### Step 1: Clone the Repository
```bash
git clone https://github.com/ErrorMask101/Android.git
cd Android

```

### Step 2: Initialize Framework

Execute the master controller with administrative privileges:

```bash
sudo python3 android.py

```

### Step 3: Launch Attack Sequence

1. Choose option **[1]** for **Full Auto Attack**.
2. Input target network identifiers:
* **LHOST:** `192.168.x.x` (Your local bind address)
* **LPORT:** `4444` (Listening port)
* **APK Path:** Path to target APK (`/path/to/target.apk`)



---

## 🔧 Technical Architecture Breakdown

```
Target APK + Payload ──> [ msfvenom -x ] ──> Hybrid APK
                                                  │
Session Listener <── [ msfconsole .rc ] <── [ AES-256 Obfuscation ] <── [ Jarsigner ]

```

1. **Payload Embedding:** Injects reverse TCP logic into legitimate app architecture without breaking original runtime behavior.
2. **Cryptographic Wrapping:** Encrypts outputs using robust block ciphers (`ErrorMask2025` key standard) to bypass automated signature checks.
3. **Automated Handlers:** Automatically constructs configuration scripts (.rc files) to streamline listener management.

---

## ⚙️ Interactive Command Menu

```bash
sudo python3 final_error_mask.py

```

| Option | Command Reference | Action Execution |
| --- | --- | --- |
| **1** | Full Auto Attack | Bind + Encrypt + Listener + Post-Exploitation Suite |
| **2** | Bind APK Only | Inject payload core without cryptographic encryption |
| **3** | Encrypt Module | Secure standalone targets via AES-256 wrappers |
| **4** | Decrypt Module | Reverse `.enc` wrappers back to clean packages |
| **5** | Manual Listener | Standalone `msfconsole` process instantiator |
| **6** | Purge Listeners | Force-terminate active background socket listeners |
| **7** | Session Manager | Inspect historical payloads and active logs |
| **8** | Audit Logs | Review recent operations and system responses |
| **9** | Fallback Mode | Deploy lightweight pure Python reverse shell framework |
| **0** | Terminate | Safe exit and temporary cache cleanup |

---

## 📂 Project Directory Structure

```text
error-mask-pro/
├── 📄 final_error_mask.py     # Core application engine
├── 🔑 debug.keystore          # Built-in signing certificate
├── 📊 error_mask_config.json  # Persistent session storage
├── 📜 error_mask_log.json     # Execution & error logs
├── 📱 bound_*.apk             # Compiled payload-injected apps
├── 🔒 *.apk.enc               # Cryptographically secured builds
└── ⚙️ listener_*.rc           # Metasploit automated resource files

```

---

## 📝 Legal & Compliance Notice

```text
╔════════════════════════════════════════════════════════════════╗
║       [!] RESTRICTED ACCESS & EDUCATIONAL TOOLING [!]          ║
║                                                                ║
║   This framework is built strictly for authorized security     ║
║   testing, penetration assessments, and academic research.     ║
║   Unauthorized deployment against external devices is illegal. ║
╚════════════════════════════════════════════════════════════════╝

```

---

## 🤝 Community Contributions

Contributions, feature requests, and bug reports are open!

1. **Fork** the Project repository.
2. Create your Feature Branch (`git checkout -b feature/EliteModule`).
3. Commit your Changes (`git commit -m 'Add EliteModule capability'`).
4. Push to the Branch (`git push origin feature/EliteModule`).
5. Open a **Pull Request**.

---

## 📜 License & Acknowledgments

Distributed under the **MIT License**. See `LICENSE` for details.

* Special credits to the **Metasploit Framework**, **Rich TUI**, and **PyCryptodome** ecosystems.

---
