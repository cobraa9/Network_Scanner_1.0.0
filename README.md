# Network Scanner Tool (Nmap)💻

## Overview 🛡️🔎

The **Network Scanner Tool** is a Python-based cybersecurity tool designed to scan networks, detect open ports, identify running services, and assess potential vulnerabilities. This tool is ideal for network pen testers, cybersecurity researchers, and network administrators who want to analyze and secure their networks. 🖥️🔌

## Features 🎯

- **Device Discovery:** Identify all devices connected to a given network.
- **Port Scanning:** Scan open ports on discovered devices.
- **Service Detection:** Identify services running on the open ports.
- **Vulnerability Detection:** Identify known vulnerabilities based on detected services.
- **Reporting:** Generate a summary report of the scanned network.

## Technologies and Libraries Used 📚

- **Python:** Core programming language. LINK --> https://www.python.org/downloads/
- **Scapy:** Scapy is used by the scanner to give users strong capabilities for packet creation, sending, sniffing, and dissecting, giving them a thorough understanding of network traffic and device activity. For further information visit --> https://github.com/secdev/scapy .
- **socket:** Built-in Python module for network communications.
- **nmap (python-nmap):** To enhance port scanning and service detection. LINK --> https://nmap.org/download.html
- **argparse:** For handling command-line arguments.
- **subprocess:** To execute system commands for additional functionalities.
- **pcap/json:** For structured reporting.
- **pcapviewer** To analyze the network PCAP/PCAPNG (Packet Capture) files. LINK --> https://marketplace.visualstudio.com/items?itemName=sankooc.pcapviewer

## Installation ⚙️📥📌

### Prerequisites ✅📦

Ensure you have Python 3.x (any updated version) installed on your system. 📂⚙️

### Clone the Repository 🖥️🔗

```bash
git clone https://github.com/cobraa9/Network_Scanner_Tool.git
cd Network_Scanner_Tool
```

### Install Required Libraries 📦🛠️

```bash
pip install scapy python-nmap argparse
```

## Usage 🖥️

Run the tool with the following command:

```bash
python scan.py --target 192.168.1.0/24
```

### Command-Line Arguments 🖥️

| Argument   | Description                                        |
| ---------- | -------------------------------------------------- |
| `--target` | The target IP address or subnet to scan.           |
| `--ports`  | Specific ports to scan (default: common ports).    |
| `--output` | Save the scan results to a file (PCAP/JSON/CSV format). |

### Example Commands 📡🖥️

- Scan a specific IP:
  ```bash
  python scan.py --target 192.168.1.100
  ```
- Scan a subnet and save results to PCAP/JSON:
  ```bash
  python scan.py --target 192.168.1.0/24 --output results.pcap
  ```

## How It Works ⚙️🛠️

1. **Device Discovery:** Uses ARP requests to detect active devices on the network. 🖥️📡🔍
2. **Port Scanning:** Uses TCP SYN scans to identify open ports. 🔌🔎
3. **Service Detection:** Uses Nmap integration to identify running services. 🔍📡
4. **Vulnerability Detection:** Cross-references detected services with a known vulnerability database. 🔥
5. **Report Generation:** Outputs findings in a structured format. 📜📂

## Disclaimer ⚠️

This tool is intended for **educational and ethical** purposes only. While port scanning itself isn't always illegal,but unauthorized scanning of networks that you do not own or have permission to scan is illegal and punishable by law. 🚨❌⚖️

## Contribution 🔧🤝
It was my first project as a complete beginner in penetration Testing, and i know that this tiny project needs a lot of improvemnets.
So, contributions are welcome! Feel free to fork the repository and submit pull requests. 📝



## Author ✍️🌍

Anirban

For Suggestions & inquiries, feel free to contact me via GitHub. 📩

