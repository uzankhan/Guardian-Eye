# Guardian-Eye# 🛡️ Guardian Eye

### *The Immortal Shield Of Your System.*

**See The Unseen & Stop The Unknown. Hunt. Isolate. Destroy.**

---

## 📌 Overview

**Guardian Eye** is an enterprise-grade, multi-layered cybersecurity suite designed for Blue Teams and security professionals. It combines **16 integrated security phases** into one powerful engine, providing real-time threat detection, ML-powered anomaly detection, automated incident response, and forensic evidence collection.

Unlike traditional antivirus solutions that rely on signature-based detection, Guardian Eye uses **behavioral analysis, machine learning, and zero-trust verification** to detect and block known and unknown threats — including zero-day attacks, ransomware, APTs, and even quantum-based threats.

---

## 🚀 Key Features

### 🔍 Real-Time Monitoring
- **WMI & ETW Integration** – Monitors every process, file, and network connection in real-time.
- **Sysmon Support** – Kernel-level logging for deep visibility.

### 🧠 Multi-Layer Detection Engine
- **Trusted Database** – Whitelist for Microsoft, Google, Mozilla, and other trusted vendors.
- **Digital Signature Verification** – Validates Authenticode signatures.
- **Reputation Scoring (0–100)** – Combines signature, path, parent process, and file age.
- **Machine Learning (Isolation Forest)** – Trained on system behavior to detect anomalies.
- **Behavioral Analysis** – Detects suspicious patterns like rapid file creation or C2 connections.

### ⚡ Automated Response
- **Instant Termination** – Kills malicious processes on detection.
- **Secure Quarantine** – Copies malicious files to a safe vault with metadata.
- **Forensic Evidence Collection** – Saves process dumps, network logs, and file hashes.
- **One-Click Restore** – Restore quarantined files using `--restore`.

### 🔐 Advanced Security Shields
| Shield | Domain | Key Capabilities |
|--------|--------|------------------|
| **Shield 1** | Endpoint & Network | DPI, DDoS Protection, DNS Tunneling Detection, USB Blocking |
| **Shield 2** | Cloud & AI | VirusTotal Integration, Ensemble ML, Zero-Day Detection |
| **Shield 3** | API, Mobile & 5G | REST/GraphQL Scanning, JWT Validation, 5G Slice Security |
| **Shield 4** | Containers & Zero-Trust | Docker/K8s Security, Micro-Segmentation |
| **Shield 5** | Quantum & Edge | Post-Quantum Cryptography (Kyber, Dilithium), QKD Simulation |
| **Shield 6** | Bio, DNA & Space | Biometric Spoof Detection, DNA Data Encryption, Satellite Monitoring |

### 🛡️ Safety First
- **System File Protection** – Never quarantines critical Windows system files.
- **Trusted Vendor Protection** – Never blocks files signed by Microsoft, Google, or Mozilla.
- **Dry Run Mode** – Test without taking any action.
- **Auto-Cleanup** – Automatically removes files older than 30 days.

---

## 📋 Requirements

### System Requirements
- **Windows 10/11** (64-bit) – Windows 7/8 with limitations
- **Python 3.8+** (3.11 recommended)
- **Administrator Rights** – Required for full protection
- **Internet Connection** – For VirusTotal & threat intelligence updates
- **At Least 5 GB Free Disk Space**

### Python Dependencies
```bash
pip install psutil wmi numpy scikit-learn pypiwin32 pywin32 scapy colorama cryptography pyyaml joblib
```

### Optional (For Advanced Features)
- **Sysmon** – Kernel-level logging  
  Download from Microsoft, then run: `Sysmon.exe -accepteula -i`
- **Npcap** – Packet capture  
  Download from [npcap.com](https://npcap.com), install with WinPcap API mode.
- **PyUSB** – USB device monitoring  
  `pip install pyusb`

---

## 🚀 Installation & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/guardian-eye.git
cd guardian-eye
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run Guardian Eye
```bash
python guardian_eye_final.py
```

### 4. Commands
| Command | Description |
|---------|-------------|
| `python guardian_eye_final.py` | Run in default mode (DRY_RUN=True – test only) |
| `--test-mode` | Force test mode (no actions) |
| `--install-service` | Install as Windows boot service |
| `--uninstall-service` | Remove the service |
| `--list-quarantine` | Show all quarantined files |
| `--restore <filename>` | Restore a specific quarantined file |
| `--update-threat-intel` | Pull latest threat intelligence feeds |
| `--train-model` | Manually retrain ML model |
| `--quantum-test` | Test quantum security modules |
| `--bio-test` | Test biometric/dna/space modules |

---

## 📁 Folder Structure

```
D:\GuardianEye_Vault\
   ├── Evidence\        (attack evidence)
   ├── Forensics\       (pre‑scan reports)
   ├── Logs\            (daily logs)
   ├── Quarantine\      (quarantined files – can restore)
   ├── PCAP\            (packet captures)
   ├── Models\          (trained ML models)
   ├── ThreatIntel\     (IOC database)
   └── ... (other phase folders)
```

---

## 🧪 Testing

To test Guardian Eye without taking any action:
```bash
python guardian_eye_final.py --test-mode
```

To enable live protection, edit the config in the code:
```python
DRY_RUN: bool = False  # Set to False for live protection
```

---

## 🛡️ Why "The Immortal Shield"?

Guardian Eye is designed to be **immortal** – it never sleeps, never crashes, and never misses a threat. With:
- **Graceful Shutdown** – `Ctrl+C` safely stops all threads.
- **Auto-Cleanup** – Old logs are automatically removed.
- **Future-Proof** – Protects against quantum decryption, AI-generated malware, and neuro-attacks.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

**Project Link:** [https://github.com/YOUR_USERNAME/guardian-eye](https://github.com/YOUR_USERNAME/guardian-eye)

---

## ⭐ Show Your Support

If this project helped you, please give it a ⭐ on GitHub!

---

**Guardian Eye – The Immortal Shield Of Your System.**  
*See The Unseen & Stop The Unknown. Hunt. Isolate. Destroy.*
