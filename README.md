# 🔍 Network Port Scanner

A lightweight, cross-platform TCP port scanner built with Python and a clean Tkinter GUI.
No third-party libraries required — runs on pure Python 3.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📋 Features

- Scan any IP address or hostname across a custom port range
- Real-time display of open ports as they are discovered
- Service identification for well-known ports (HTTP, SSH, FTP, MySQL, etc.)
- Live progress bar and elapsed time tracker
- Graceful stop — cancel a scan at any time
- Export results to a `.txt` file
- Multi-threaded scanning (up to 500 concurrent threads)
- Zero external dependencies — standard library only

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your system
- Tkinter (comes pre-installed with most Python distributions)

If Tkinter is missing on Linux:
```bash
sudo apt install python3-tk
```

### Run the App

```bash
# Clone the repository
git clone https://github.com/vaishaldsouza/Network_Port_Scanner.git

# Navigate into the folder
cd Network_Port_Scanner

# Run the scanner
python3 port_scanner.py
```

---

## 🛠️ How to Use

1. Enter a **Target** — IP address (e.g. `192.168.1.1`) or hostname (e.g. `scanme.nmap.org`)
2. Set the **Start Port** and **End Port** (default: 1 to 1024)
3. Click **Start Scan**
4. Open ports appear in real time in the results panel
5. Click **Save Results** to export findings to a `.txt` file

---

## 📡 Supported Services

| Port | Service |
|------|---------|
| 21   | FTP     |
| 22   | SSH     |
| 23   | Telnet  |
| 25   | SMTP    |
| 53   | DNS     |
| 80   | HTTP    |
| 110  | POP3    |
| 143  | IMAP    |
| 443  | HTTPS   |
| 3306 | MySQL   |
| 3389 | RDP     |
| 5900 | VNC     |
| 8080 | HTTP-Alt|

---

## ⚙️ Technical Details

| Detail | Value |
|--------|-------|
| Language | Python 3.x |
| GUI Framework | Tkinter / ttk |
| Concurrency | Multi-threading with Semaphore |
| Max Threads | 500 (default) |
| Timeout per Port | 0.5 seconds (default) |
| Protocol | TCP (connect_ex) |

---

## ⚠️ Legal Disclaimer

This tool is intended for use on systems **you own or have explicit permission to scan**.
Unauthorized port scanning may be **illegal** in your jurisdiction.
Use responsibly and ethically.

---

## 📁 Project Structure

```
network-port-scanner/
│
├── port_scanner.py     # Main application file
├── README.md           # Project documentation
└── .gitignore          # Git ignore rules
```
