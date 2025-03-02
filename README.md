🚀 Network Sniffer

📌 Overview

A network sniffer is a tool used to capture and analyze network traffic. This Python-based sniffer leverages Scapy to monitor data packets flowing through a network interface. It helps in understanding packet structures, identifying network patterns, and troubleshooting potential security issues.

🔍 How It Works

The script captures live network packets and extracts key details such as:

Source and Destination IP Addresses

Protocol Type (TCP, UDP, ICMP, etc.)

Packet Length and Payload Information

By analyzing captured packets, users can gain insights into network behavior, detect anomalies, and enhance cybersecurity knowledge.

🛠 Installation

Install dependencies:

pip install -r requirements.txt

▶️ Usage

Run the script with administrator privileges:

sudo python network_sniffer.py

✨ Features

✅ Captures live network traffic in real time✅ Displays key packet details (source, destination, protocol)✅ Automatically installs Scapy if missing✅ Simple and lightweight✅ Helps in network monitoring and troubleshooting

🚀 Future Enhancements

🔹 Add protocol filtering (TCP, UDP, HTTP)🔹 Save captured packets to a log file🔹 Implement a user-friendly GUI for analysis🔹 Advanced packet analysis for cybersecurity research
