# Network Configuration – Kali Linux Lab

## 1. Overview

This document describes the network configuration implemented for the cybersecurity testing lab using Oracle VirtualBox.

## 2. NAT Network Configuration

A custom NAT Network was created in Oracle VirtualBox.

| Setting | Configuration |
|---|---|
| Network Name | NatNetwork |
| IPv4 Prefix | 10.0.0.0/24 |
| DHCP | Enabled |
| Network Mode | NAT Network |

## 3. Kali Linux Network Configuration

The Kali Linux virtual machine was configured with a static IPv4 address.

| Setting | Value |
|---|---|
| IPv4 Method | Manual |
| IP Address | 10.0.0.2 |
| Netmask | 255.255.255.0 |
| Gateway | 10.0.0.1 |
| DNS | 10.0.0.1 |

## 4. Network Verification

The following commands can be used to verify the configuration:

### Check IP Address

```bash
ip addr
```

### Check Default Gateway

```bash
ip route
```

### Test Network Connectivity

```bash
ping -c 4 10.0.0.1
```

### Test DNS Resolution

```bash
ping -c 4 google.com
```

## 5. Expected Results

- Kali Linux should use the configured static IP address.
- The default gateway should be reachable.
- External network connectivity should work.
- DNS resolution should work.

## 6. Conclusion

The network configuration establishes the connectivity required for the virtual cybersecurity testing environment.
