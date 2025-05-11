# **Mac Master - Network Stealth Tool**

**Mac Master** is a powerful tool for network manipulation, designed for advanced users. It allows you to perform **MAC Spoofing**, **IP Spoofing**, **ARP Spoofing**, and even more complex operations like **Evil Twin Attacks** and **Deauthentication Attacks** designed for network security researchers.

---

### 🚀 **Features**:
- **MAC Spoofing:** Change your MAC address for complete anonymity.
- **IP Spoofing:** Spoof your IP address to mimic another device on the network.
- **ARP Spoofing:** Perform ARP poisoning to intercept network traffic.
- **Evil Twin Attack:** Clone a target Wi-Fi network and capture user credentials.
- **Deauthentication Attack:** Kick users off the network to temporarily disconnect them.

---

### ⚙️ **Setup Instructions**:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/mac-master.git
    cd mac-master
    ```

2. **Install dependencies**:
    - Ensure you have Python 3.x installed.
    - Install required libraries with:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the script**:
    - Run the script with root privileges:
    ```bash
    sudo python mac_master.py
    ```

    - The script will prompt you for specific actions:
        - Choose between **MAC Spoofing**, **IP Spoofing**, or **Advanced Attacks**.
        - For **MAC Spoofing**, you will be prompted to enter the MAC address you want to spoof.
        - For **Advanced Attacks**, the script will guide you through setting up Evil Twin and Deauthentication attacks.

---

### 🛠️ **Usage Example**:

1. **MAC Spoofing**:
    - Spoof your MAC address by entering:
    ```bash
    sudo python mac_master.py --spoof-mac
    ```

2. **IP Spoofing**:
    - Spoof your IP address to connect to a specific network:
    ```bash
    sudo python mac_master.py --spoof-ip
    ```

3. **Advanced Attacks**:
    - Use Evil Twin or Deauthentication attacks to intercept or disconnect users:
    ```bash
    sudo python mac_master.py --attack evil-twin
    ```

---

### 🔐 **Security Disclaimer**:
This tool is meant for **ethical hacking** and **learning purposes** only. **Mac Master** should only be used on networks and devices where you have explicit permission to test and manipulate.

**Misuse can lead to legal consequences. Use responsibly.**

---





# **Aircrack-ng** suite for advanced attacks




## Features

### 1. **MAC Spoofing**
- **Description:** Change your MAC address for anonymity and bypass MAC filters.
- **Key Features:**
  - Random MAC generation and custom MAC input.
  - Cycle through multiple MAC addresses.
  - Works on both wired and wireless interfaces.
- **Dependencies:** `macchanger`, `ifconfig`, `ip`, Python `subprocess`.

### 2. **IP Spoofing**
- **Description:** Spoof your IP address to mimic another device on the network.
- **Key Features:**
  - Source IP manipulation for custom packets.
  - Supports both UDP and TCP spoofing.
  - Random IP generation from a subnet.
- **Dependencies:** `scapy`, `socket`, `iproute2`.

### 3. **ARP Spoofing (ARP Poisoning)**
- **Description:** Poison the ARP cache of devices and intercept network traffic.
- **Key Features:**
  - ARP cache poisoning for traffic interception.
  - Man-in-the-Middle (MITM) attack support.
  - Target specific devices with IP addresses.
- **Dependencies:** `arpspoof`, `ettercap`, Python `scapy`, `tcpdump`, `wireshark`.

### 4. **Evil Twin Attack**
- **Description:** Clone a target Wi-Fi network and capture user credentials.
- **Key Features:**
  - Clone SSID, encryption, and settings from the target network.
  - Use deauthentication flooding to force clients to connect to your fake AP.
  - Capture user credentials using a captive portal.
- **Dependencies:** `hostapd`, `airmon-ng`, `mdk3`, `dnsmasq`, Python `subprocess`.

### 5. **Deauthentication Attack (DoS Attack)**
- **Description:** Disconnect devices from the network by flooding it with deauthentication packets.
- **Key Features:**
  - Flood the network with deauth packets to disconnect all clients.
  - Target specific devices by MAC address.
  - Perform attacks with stealth mode to hide presence.
- **Dependencies:** `aireplay-ng`, `mdk3`, Python `subprocess`.

### 6. **WPA/WPA2 Cracking**
- **Description:** Crack WPA/WPA2 passwords using a captured 4-way handshake.
- **Key Features:**
  - Capture WPA handshakes for offline cracking.
  - Supports dictionary and brute-force attacks.
  - GPU-based cracking for faster performance.
- **Dependencies:** `aircrack-ng`, `hashcat`, Python `subprocess`, `os`.

### 7. **User Interface & Documentation**
- **Description:** A GUI for easy control and interaction with the modules.
- **Key Features:**
  - A clean and intuitive graphical interface.
  - Real-time attack feedback and results.
  - Built-in documentation for module usage.
- **Dependencies:** `tkinter`, `pyqt5`, `markdown`, `sphinx`.

## Installation

To install the necessary dependencies, run the following commands:

```bash
# For Mac Spoofing
sudo apt-get install macchanger

# For ARP Spoofing and MITM
sudo apt-get install arpspoof ettercap

# For Evil Twin Attack
sudo apt-get install hostapd aircrack-ng mdk3 dnsmasq

# For WPA Cracking
sudo apt-get install aircrack-ng hashcat

# For IP Spoofing and Packet Crafting
sudo apt-get install python3-pip
pip install scapy

# For Deauthentication Attacks
sudo apt-get install aireplay-ng mdk3

# GUI Dependencies
pip install tkinter pyqt5

# General Dependencies
pip install -r requirements.txt

