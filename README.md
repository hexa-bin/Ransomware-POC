# 🛡️ Ransomware-POC

**⚠️ For Educational Use Only — Ethical Ransomware Simulation Project**  
A  ransomware proof-of-concept tool designed for **cybersecurity research**, **red-team simulation**, and **academic demonstration**.

---

## ✨ Overview

This project is a two-part educational ransomware simulation:

- 🐍 A **Python GUI** that mimics ransomware behavior — encrypts files and simulates a victim-facing interface.
- 🌐 A **PHP-based Command & Control (C2) dashboard** that logs encryption keys, manages signals, and acts as the attacker interface.

🔐 **Fully safe** – No real destruction or propagation. Built to educate, not harm.

---

## 📂 Folder Structure

```
Ransomware-POC/
├── simulator_gui/
│   ├── rans.py
│   ├── gui.py
│   ├── Simple-Encryption.py
│   ├── Simple-Decryption.py
│   ├── logo.ico
│   └── img/
├── control_panel/
│   ├── public/
│   ├── includes/
│   ├── uploads/
│   └── assets/
├── README.md
├── .gitignore
```

---

## ✅ Features

| Module              | Key Features                                          |
|---------------------|-------------------------------------------------------|
| 🐍 Python Simulator | AES-256 encryption, victim wallpaper, GUI lock screen |
| 🌐 PHP C2 Panel     | Secure login, view keys, receive victim metadata      |
| 🔒 Reversible Logic | Safe for labs; no real-world harm or file loss        |
| 📡 Signal Handling  | Check/stop signals, kill logic, fake command API      |

---

## 🛠️ How to Run

### 🐍 Victim-Side Python GUI

1. Install Python 3.x  
2. Open terminal:
   ```bash
   cd simulator_gui
   python rans.py
   ```
3. This will:
   - Simulate ransomware GUI
   - Encrypt files
   - Send encrypted key (image) to C2 panel

---

### 🌐 Attacker-Side Command Panel

1. Copy `control_panel/` into your `htdocs/` directory (XAMPP/WAMP)
2. Start Apache server
3. Visit:
   ```
   http://localhost/control_panel/public/login.php
   ```
4. Login or register → View logs and key uploads

---

## ⚙️ Tech Stack

| Component      | Technologies Used           |
|----------------|-----------------------------|
| GUI & Crypto   | Python, Tkinter, AES (PyCrypto) |
| Backend        | PHP, HTML, CSS, JavaScript   |
| Server         | Apache (XAMPP/WAMP)          |
| Optional DB    | SQLite or MySQL              |

---

## 📸 Screenshots

> Once you upload screenshots into a `/screenshots` folder, reference them like below:

| Victim GUI                | Attacker Dashboard         |
|---------------------------|----------------------------|
| ![](screenshots/gui.png)  | ![](screenshots/dashboard.png) |

---

## ⚠️ Disclaimer: Educational Use Only

This project is created solely for:

- ✅ Cybersecurity education
- ✅ Red-team demonstrations
- ✅ Ethical hacking practice
- ✅ Security awareness training

🚫 Do **NOT** use this for:
- Real-world attacks or malware creation
- Unauthorized systems
- Any activity outside isolated lab environments

> The authors take **no responsibility** for misuse or abuse of this tool.

---

## 📜 License

Licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 📈 Use Cases

- 🎓 University-level red-team simulations
- 🧠 Ethical hacking workshops
- 🔍 Safe malware behavior emulation
- 📡 Ransomware incident response training

---

## 🚧 Future Enhancements

- [ ] Live victim tracking
- [ ] WebSocket-based control channels
- [ ] Geolocation and dummy IP mapping
- [ ] Email/SMTP signal triggers

---

## 🙌 Credits

Created by [@hexa-bin](https://github.com/hexa-bin)  
Special thanks to cybersecurity educators, researchers, and red-teamers who inspire safe, ethical hacking.

---

**Built for Labs 🧪 | Powered by Python 🐍 | Secured by Ethics 🛡️**
