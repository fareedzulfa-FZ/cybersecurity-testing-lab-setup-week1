# Troubleshooting – Cybersecurity Lab Setup

## 1. Kali Linux Internet Connectivity Issues

If Kali Linux cannot access the internet:

- Verify that the NAT Network is configured correctly.
- Check that the Kali VM is connected to NatNetwork.
- Verify the IP address, gateway, and DNS configuration.
- Ensure that no other VM is using the same static IP address.

## 2. Network Connection Restart

For the relevant NetworkManager configuration, the following commands can be used when troubleshooting the connectivity issue described in the lab guide:

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0

sudo nmcli connection down "Wired connection 1"

sudo nmcli connection up "Wired connection 1"
```

## 3. Network Verification Commands

```bash
ip addr
ip route
ping -c 4 10.0.0.1
ping -c 4 google.com
```

## 4. Conclusion

Systematic troubleshooting helps identify network configuration problems and maintain a functional virtual lab environment.
