# 🚀 Network Sniffer

## 📌 Overview

A network sniffer is a tool used to capture and analyze network traffic. This Python-based sniffer leverages Scapy to monitor data packets flowing through a network interface. It helps in understanding packet structures, identifying network patterns, and troubleshooting potential security issues.

## 🔍 How It Works

The script captures live network packets and extracts key details such as:

- **Source and Destination IP Addresses**
- **Protocol Type (TCP, UDP, ICMP, etc.)**
- **Packet Length and Payload Information**

By analyzing captured packets, users can gain insights into network behavior, detect anomalies, and enhance cybersecurity knowledge.

## 🛠 Installation

1. Clone the repository:
   ```bash
   https://github.com/meghh06/CodeAlpha_Network-Sniffer.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## ▶️ Usage

Run the script with administrator privileges:

```bash
sudo python network_sniffer.py
```

## ✨ Features

✅ Captures live network traffic in real time\
✅ Displays key packet details (source, destination, protocol)\
✅ Automatically installs Scapy if missing\
✅ Simple and lightweight\
✅ Helps in network monitoring and troubleshooting

## 📜 Code

```python
import sys
import subprocess

try:
    from scapy.all import sniff
except ModuleNotFoundError:
    print("Scapy module not found. Installing...")
    subprocess.check_call([sys.executable, "-m", "pip", "install", "scapy"])
    from scapy.all import sniff

def packet_callback(packet):
    print(packet.summary())  # Display packet details

# Capture packets (adjust count and interface as needed)
print("Sniffing network traffic... Press Ctrl+C to stop.")
sniff(prn=packet_callback, count=10)  # Capture 10 packets
```

## 🚀 Future Enhancements

🔹 Add protocol filtering (TCP, UDP, HTTP)\
🔹 Save captured packets to a log file\
🔹 Implement a user-friendly GUI for analysis\
🔹 Advanced packet analysis for cybersecurity research

---



