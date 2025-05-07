# **Mac Master - Network Stealth Tool**

**Mac Master** is a powerful tool for network manipulation, designed for advanced users. It allows you to perform **MAC Spoofing**, **IP Spoofing**, **ARP Spoofing**, and even more complex operations like **Evil Twin Attacks** and **Deauthentication Attacks**.

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
