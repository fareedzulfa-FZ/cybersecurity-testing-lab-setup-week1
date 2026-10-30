# Cybersecurity Testing Lab Environment Setup

## 1. Project Overview

This project focuses on setting up a virtual cybersecurity testing lab environment using Oracle VirtualBox and Kali Linux.

The objective is to create an isolated virtual networking environment that can be used for learning cybersecurity concepts, ethical hacking, network configuration, and penetration testing.

## 2. Tools and Technologies

- Oracle VirtualBox
- Kali Linux
- 7-Zip
- Virtual NAT Network
- NetworkManager

## 3. Lab Environment Configuration

| Component | Configuration |
|---|---|
| Virtualization Platform | Oracle VirtualBox |
| Operating System | Kali Linux |
| Network Type | NAT Network |
| Network Subnet | 10.0.0.0/24 |
| Kali Linux IP Address | 10.0.0.2 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 10.0.0.1 |
| DNS Server | 8.8.8.8 |

## 4. Implementation Steps

### Step 1 – Download and Install 7-Zip

Downloaded and installed 7-Zip to extract the required virtual machine files.

### Step 2 – Download and Install Oracle VirtualBox

Downloaded and installed Oracle VirtualBox to create and manage virtual machines.

### Step 3 – Configure VirtualBox NAT Network

Created a custom NAT Network in VirtualBox with the following configuration:

- Network Name: NatNetwork
- IPv4 Network: 10.0.0.0/24
- DHCP: Enabled

### Step 4 – Download and Import Kali Linux

Downloaded the Kali Linux virtual machine and imported it into Oracle VirtualBox.

### Step 5 – Configure Kali Linux IP Address

Configured the Kali Linux network interface with a static IPv4 address.

- IP Address: 10.0.0.2
- Subnet Mask: 255.255.255.0
- Gateway: 10.0.0.1
- DNS: 10.0.0.1

### Step 6 – Create a Virtual Machine Snapshot

Created a snapshot of the configured Kali Linux virtual machine to preserve the working environment and provide a recovery point.

## 5. Additional Virtual Machine Configurations

The lab requirements also include:

- Enabling shared clipboard.
- Enabling drag and drop.
- Configuring a shared folder between the host machine and Kali Linux.
- Providing internet connectivity to Kali Linux.

## 6. Testing and Verification

The following checks are used to verify the lab environment:

- Verify the Kali Linux IP address.
- Check connectivity to the default gateway.
- Test internet connectivity.
- Verify DNS resolution.

## 7. Learning Outcomes

Through this hands-on project, I gained practical knowledge of:

- Virtualization and virtual machine management.
- NAT networking and subnet configuration.
- IPv4 static IP configuration.
- Network connectivity and DNS troubleshooting.
- Virtual machine snapshots and recovery.

## 8. Screenshots

Screenshots of the installation, network configuration, Kali Linux setup, and testing results are included in the `screenshots` directory.

## 9. Disclaimer

This lab environment is intended for educational purposes and authorized cybersecurity testing only.

## Author

Zulfa Fareed

Cybersecurity Program – Networkwalks (Batch B084)

