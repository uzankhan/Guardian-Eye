# 🛡️ Guardian Eye – Installation Guide

### *The Immortal Shield Of Your System.*

---

## 📋 System Requirements

| Requirement | Details |
|-------------|---------|
| **Operating System** | Windows 10 / 11 (64-bit) – Windows 7/8 with limitations |
| **Python Version** | Python 3.8 or higher (3.11 recommended) |
| **Administrator Rights** | Required for full protection and monitoring |
| **Internet Connection** | Required for VirusTotal API and threat intelligence updates |
| **Disk Space** | At least 5 GB free space |
| **RAM** | 4 GB minimum (8 GB recommended) |

---

## 🔧 Step 1: Install Python

1. Download Python from [python.org](https://www.python.org/downloads/)
2. During installation, **check** ✅ **"Add Python to PATH"**
3. Verify installation:
   ```bash
   python --version
   ```

---

## 📦 Step 2: Clone the Repository

```bash
git clone https://github.com/uzankhan/Guardian-Eye.git
cd Guardian-Eye
```

> **OR** download ZIP from GitHub and extract.

---

## 🧩 Step 3: Install Python Dependencies

Open **Command Prompt as Administrator** and run:

```bash
pip install -r requirements.txt
```

### Manual Installation (if requirements.txt fails):

```bash
pip install psutil wmi numpy scikit-learn pypiwin32 pywin32 scapy colorama cryptography pyyaml joblib
```

---

## 🔌 Step 4: Install Optional Tools (For Advanced Features)

### 🔹 Sysmon (Kernel-Level Logging)

1. Download Sysmon from [Microsoft Sysinternals](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon)
2. Extract and install:
   ```bash
   Sysmon.exe -accepteula -i
   ```

### 🔹 Npcap (Packet Capture)

1. Download Npcap from [npcap.com](https://npcap.com)
2. Install with **WinPcap API-compatible Mode** selected.

### 🔹 PyUSB (USB Device Monitoring)

```bash
pip install pyusb
```

---

## 🚀 Step 5: Run Guardian Eye

### 🔸 Test Mode (Safe – No Actions Taken)

```bash
python guardian_eye.py
```

### 🔸 Live Protection Mode

Edit the `guardian_eye.py` file and change:

```python
DRY_RUN: bool = False  # Set to False for live protection
```

Then run:

```bash
python guardian_eye.py
```

### 🔸 Install as Windows Service (Boot-Time Protection)

```bash
python guardian_eye.py --install-service
```

---

## 📁 Step 6: Folder Structure (Auto-Created)

Guardian Eye automatically creates this structure:

```
D:\GuardianEye_Vault\
   ├── Evidence\        (Attack evidence and logs)
   ├── Forensics\       (Pre‑scan reports)
   ├── Logs\            (Daily operational logs)
   ├── Quarantine\      (Quarantined files – can restore)
   ├── PCAP\            (Network packet captures)
   ├── Models\          (Trained ML models)
   └── ThreatIntel\     (IOC database)
```

---

## 🛠️ Step 7: Common Commands

| Command | Description |
|---------|-------------|
| `python guardian_eye.py --test-mode` | Run in test mode (no actions) |
| `python guardian_eye.py --list-quarantine` | Show all quarantined files |
| `python guardian_eye.py --restore chrome.exe` | Restore a quarantined file |
| `python guardian_eye.py --install-service` | Install as Windows service |
| `python guardian_eye.py --uninstall-service` | Remove the service |

---

## ❓ Troubleshooting

### ❌ ModuleNotFoundError
```bash
pip install missing_package_name
```

### ❌ WMI Error
- Run **Command Prompt as Administrator**.

### ❌ Scapy / Npcap Error
- Install Npcap and restart.

### ❌ Permission Denied
- Ensure you are running as Administrator.

### ❌ Process Not Found Error
- Ignore these – they are normal for short-lived processes.

---

## 📞 Support

- **GitHub Issues:** [https://github.com/uzankhan/Guardian-Eye/issues](https://github.com/uzankhan/Guardian-Eye/issues)
- **Project Link:** [https://github.com/uzankhan/Guardian-Eye](https://github.com/uzankhan/Guardian-Eye)

---

**Guardian Eye – The Immortal Shield Of Your System.** 🛡️  
*See The Unseen & Stop The Unknown. Hunt. Isolate. Destroy.*
