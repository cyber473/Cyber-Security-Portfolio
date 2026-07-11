# IP Address

## 📌 Overview

**IP Address** is the process of assigning a unique numerical address to every device connected to a network. It allows devices to identify each other and exchange data over local networks and the Internet.

---

## 🎯 What is it?

An **IP (Internet Protocol) Address** is a unique identifier assigned to a device on a network. It enables devices to send and receive data by identifying the source and destination.

### Types of IP Addresses

* IPv4
* IPv6

### IPv4 Example

```
192.168.1.10
```

### IPv6 Example

```
2001:db8::1
```

---

## ❓ Why is it Needed?

IP Addressing is essential because it:

* Uniquely identifies every device on a network.
* Enables communication between devices.
* Helps routers forward packets to the correct destination.
* Supports Internet connectivity.
* Forms the foundation of networking and cybersecurity.

---

## ⚙️ How Does it Work?

When you open a website:

1. Your device has its own IP address.
2. DNS translates the domain name (e.g., google.com) into an IP address.
3. Your computer sends packets with:

   * Source IP Address
   * Destination IP Address
4. Routers forward the packets through the Internet.
5. The destination server receives the request and sends a response back to your IP address.

---

## 🏠 Real Life Example

Think of an IP address like a **home address**.

* Your home address identifies where you live.
* An IP address identifies where a device is located on a network.
* Without an address, a courier cannot deliver a package.
* Without an IP address, data cannot reach the correct device.

---

## 🛠 Practical Demo

### Display IP Address

```bash
ip addr
```

---

### Show Routing Table

```bash
ip route
```

---

### Display Network Interfaces

```bash
ip link
```

---

### Test Connectivity

```bash
ping google.com
```

---

### Trace the Network Path

```bash
traceroute google.com
```

---

### DNS Lookup

```bash
nslookup google.com
```

---

### Display ARP Table

```bash
ip neigh
```

---

## 💻 Kali Linux Commands

```bash
# Show IP addresses
ip addr

# Show routing table
ip route

# Show network interfaces
ip link

# Display ARP table
ip neigh

# Test connectivity
ping google.com

# Trace network route
traceroute google.com

# DNS lookup
nslookup google.com

# Scan a target
nmap scanme.nmap.org

# Capture packets
sudo tcpdump -i eth0

# Open Wireshark
wireshark
```

---

## 🔐 VAPT Perspective

### Why should a Pentester know IP Addressing?

Understanding IP addressing is essential for reconnaissance, scanning, exploitation, and network analysis.

### Where is it used?

* Network Reconnaissance
* Nmap Scanning
* Host Discovery
* Vulnerability Assessment
* Packet Analysis
* Firewall Testing
* Routing Analysis
* Internal Network Pentesting
* VPN Testing
* Incident Response

### Common IP-Related Attacks

* IP Spoofing
* ICMP Attacks
* Man-in-the-Middle (MITM)
* Network Scanning
* ARP Spoofing (Local Network)
* DDoS Attacks

---

## 💡 Key Points

* Every device on a network requires a unique IP address.
* IPv4 uses **32-bit** addresses, while IPv6 uses **128-bit** addresses.
* Routers use IP addresses to forward packets.
* DNS converts domain names into IP addresses.
* Public and Private IP addresses serve different purposes.

---

## ❓ Interview Questions

### 1. What is an IP address?

### 2. What is the difference between IPv4 and IPv6?

### 3. What is the difference between a Public IP and a Private IP?

### 4. What is the purpose of an IP address?

### 5. Which protocol is responsible for IP addressing?

### 6. What is the loopback IP address?

### 7. What is the difference between Static and Dynamic IP addresses?

### 8. Which command is used to display the IP address in Linux?

### 9. What is the default localhost IP address in IPv4?

### 10. Why is IP Addressing important in penetration testing?

---

## 📚 References

* **PortSwigger Web Security Academy** – Networking Fundamentals
* **OWASP Web Security Testing Guide (WSTG)**
* **RFC 791** – Internet Protocol Version 4 (IPv4)
* **RFC 8200** – Internet Protocol Version 6 (IPv6)
* **RFC 1918** – Private IPv4 Address Space
* **RFC 4291** – IPv6 Addressing Architecture

---

## 📊 IP Addressing Summary

| Feature        | IPv4         | IPv6            |
| -------------- | ------------ | --------------- |
| Address Length | 32-bit       | 128-bit         |
| Example        | 192.168.1.10 | 2001:db8::1     |
| Address Space  | ~4.3 Billion | 340 Undecillion |
| NAT Required   | Yes (Common) | Usually No      |
| Header Size    | Variable     | Fixed           |
| Security       | Optional     | IPSec Support   |

### 📍 Common Private IPv4 Ranges

| Range                         | CIDR           |
| ----------------------------- | -------------- |
| 10.0.0.0 – 10.255.255.255     | 10.0.0.0/8     |
| 172.16.0.0 – 172.31.255.255   | 172.16.0.0/12  |
| 192.168.0.0 – 192.168.255.255 | 192.168.0.0/16 |

### 📍 Common Special IP Addresses

| Address         | Purpose                                 |
| --------------- | --------------------------------------- |
| 127.0.0.1       | Loopback (Localhost)                    |
| 0.0.0.0         | Default/Unspecified Address             |
| 255.255.255.255 | Broadcast Address                       |
| 169.254.0.0/16  | APIPA (Automatic Private IP Addressing) |
