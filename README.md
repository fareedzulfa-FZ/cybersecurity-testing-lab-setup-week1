# 🔐 Cybersecurity Testing Lab Environment Setup

<p align="center">
  <strong>A Virtual Cybersecurity Lab using Oracle VirtualBox and Kali Linux</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-VirtualBox-blue?style=for-the-badge&logo=virtualbox" />
  <img src="https://img.shields.io/badge/OS-Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux" />
  <img src="https://img.shields.io/badge/Network-NAT%20Network-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Project-Completed-success?style=for-the-badge" />
</p>

---

## 📌 1. Project Overview

This project focuses on establishing a virtual cybersecurity testing lab environment on a personal computer using Oracle VirtualBox and Kali Linux.

The primary objective is to create an isolated virtual environment that can be used for learning cybersecurity concepts, understanding network configurations, and performing authorized ethical hacking and penetration testing exercises.

The lab uses a custom NAT Network with the `10.0.0.0/24` subnet and a statically configured Kali Linux virtual machine.

## 🎯 2. Project Objectives

- Install and configure Oracle VirtualBox.
- Create a custom NAT Network using the `10.0.0.0/24` subnet.
- Download and import Kali Linux into VirtualBox.
- Configure a static IPv4 address for Kali Linux.
- Establish internet connectivity.
- Enable clipboard sharing and drag-and-drop functionality.
- Configure a shared Downloads folder between the host and virtual machine.
- Create a virtual machine snapshot for recovery.

## 🛠️ 3. Tools and Technologies

| Tool | Purpose |
|---|---|
| Oracle VirtualBox | Virtualization platform |
| Kali Linux | Cybersecurity testing operating system |
| NAT Network | Virtual network configuration |
| NetworkManager | Linux network management |
| GitHub | Project documentation and version control |

## 🌐 4. Network Architecture

The lab environment consists of a host operating system running Oracle VirtualBox, with Kali Linux operating as a virtual machine.

### Network Configuration

| Configuration | Value |
|---|---|
| Network Mode | NAT Network |
| Network Name | NatNetwork |
| Network Address | 10.0.0.0/24 |
| Kali Linux IP Address | 10.0.0.2 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 10.0.0.1 |
| DNS Server | 10.0.0.1 |

### Network Architecture Diagram

```text
             Host Computer
               (Windows)
                    |
                    |
             Oracle VirtualBox
                    |
                    |
             Custom NAT Network
               10.0.0.0/24
                    |
                    |
              Kali Linux VM
               10.0.0.2/24
                    |
                    |
              Internet Access
```

## ⚙️ 5. Implementation Process


### Step 1 – Install Oracle VirtualBox

Downloaded and installed Oracle VirtualBox to create and manage virtual machines.

### Step 2 – Configure NAT Network

Created a custom NAT Network in VirtualBox.

- Network Name: NatNetwork
- IPv4 Network: 10.0.0.0/24
- DHCP: Enabled

### Step 3 – Download and Import Kali Linux

Downloaded the Kali Linux VirtualBox image from the official Kali Linux website and imported it into Oracle VirtualBox.

### Step 4 – Configure Kali Linux IP Address

Configured the Kali Linux network interface with a static IPv4 address.

- IP Address: 10.0.0.2
- Subnet Mask: 255.255.255.0
- Gateway: 10.0.0.1
- DNS: 10.0.0.1

### Step 5 – Configure Virtual Machine Settings

Configured additional VirtualBox settings:

- Enabled shared clipboard.
- Enabled drag-and-drop functionality.
- Configured a shared Downloads folder from the host machine.
- Connected Kali Linux to the custom NAT Network.

### Step 7 – Create a Virtual Machine Snapshot

Created a snapshot of the configured Kali Linux virtual machine to preserve the initial lab environment and provide a recovery point.

## 🧪 6. Testing and Verification

The following checks were performed to verify the lab configuration:

| Test | Expected Result |
|---|---|
| IP configuration | 10.0.0.2/24 |
| Gateway configuration | 10.0.0.1 |
| Network connectivity | Successful |
| DNS resolution | Successful |
| Internet connectivity | Available |
| VM snapshot | Created |

## 📸 7. Project Screenshots

Screenshots documenting the installation, configuration, and verification stages are available in the `screenshots/` directory.

| Screenshot | Description |
|---|---|
| VirtualBox Installation | VirtualBox installation |
| NAT Network Configuration | Custom NAT Network setup |
| Kali VM Configuration | Kali Linux VM settings |
| IP Configuration | Static IP configuration |
| Connectivity Testing | Network and DNS testing |
| VM Snapshot | Snapshot creation |

## 📚 8. Key Learning Outcomes

Through this hands-on project, I gained practical knowledge and experience in:

- Virtualization and virtual machine management.
- Configuring NAT-based virtual networks.
- IPv4 addressing and subnet configuration.
- Static IP configuration in Kali Linux.
- Network connectivity and DNS troubleshooting.
- Virtual machine snapshots and recovery.
- Technical documentation and lab setup.

## 🚀 9. Future Improvements

Potential future enhancements to this lab include:

- Adding Windows virtual machines as testing targets.
- Practising network scanning using Nmap.
- Analysing network traffic using Wireshark.
- Performing vulnerability assessments in authorized lab environments.
- Exploring penetration testing tools available in Kali Linux.

## ⚠️ 10. Disclaimer

This project is intended strictly for educational purposes and authorized cybersecurity testing. Any security testing should only be conducted in environments where permission has been granted.

## 👨‍💻 Author

**Zulfa Fareed**

Cybersecurity Student


LinkedIn: https://www.linkedin.com/in/zulfa-fareed-0a0085441/

---

⭐ If you find this project useful, feel free to explore the repository and follow my cybersecurity learning journey.
