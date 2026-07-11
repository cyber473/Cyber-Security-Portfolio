# TCP/IP Model

## 📌 Overview

The **TCP/IP (Transmission Control Protocol/Internet Protocol) Model** is the standard networking model used on the Internet. It defines how data is transmitted between devices using a suite of communication protocols.

---

## 🎯 What is it?

The **TCP/IP Model** is a **4-layer networking model** that provides the rules and protocols for communication over the Internet. It is the practical model used in modern computer networks.

### The 4 Layers

1. Application
2. Transport
3. Internet
4. Network Access (Link)

---

## ❓ Why is it Needed?

The TCP/IP Model is important because it:

* Powers the Internet and modern computer networks.
* Defines how devices communicate across different networks.
* Ensures reliable and efficient data transmission.
* Supports interoperability between different operating systems and hardware.
* Forms the foundation of network security and penetration testing.

---

## ⚙️ How Does it Work?

When you visit a website:

1. **Application Layer** creates an HTTP request.
2. **Transport Layer** uses TCP or UDP to segment the data.
3. **Internet Layer** assigns source and destination IP addresses and determines routing.
4. **Network Access Layer** converts the data into frames and transmits it over Ethernet or Wi-Fi.

The receiving device processes the data in reverse order until it reaches the application.

---

## 🏠 Real Life Example

Imagine sending a parcel to a friend.

* **Application Layer:** You write the message.
* **Transport Layer:** The parcel is packed securely.
* **Internet Layer:** The courier chooses the delivery route.
* **Network Access Layer:** The delivery vehicle transports the parcel to its destination.

---

## 🛠 Practical Demo

### View Network Interfaces

```bash
ip addr
```

### View Routing Table

```bash
ip route
```

### Check Active Connections

```bash
ss -tuln
```

### Send an HTTP Request

```bash
curl https://example.com
```

### Test Connectivity

```bash
ping google.com
```

### Capture Packets

```bash
sudo tcpdump -i eth0
```

### Open Wireshark

```bash
wireshark
```

---

## 💻 Kali Linux Commands

```bash
# Show network interfaces
ip addr

# Display routing table
ip route

# View ARP table
ip neigh

# DNS lookup
nslookup google.com

# Test network connectivity
ping google.com

# Trace packet route
traceroute google.com

# Display TCP/UDP sockets
ss -tuln

# Capture packets
sudo tcpdump -i eth0

# Launch Wireshark
wireshark

# Scan a host
nmap scanme.nmap.org
```

---

## 🔐 VAPT Perspective

### Why should a Pentester know the TCP/IP Model?

A pentester analyzes network traffic, identifies vulnerabilities, and understands how protocols work. Almost every network attack targets one or more TCP/IP layers.

### Common Attacks by Layer

**Application Layer**

* SQL Injection
* Cross-Site Scripting (XSS)
* CSRF
* SSRF
* Authentication Bypass

**Transport Layer**

* SYN Flood
* TCP Session Hijacking
* UDP Flood
* Port Scanning

**Internet Layer**

* IP Spoofing
* ICMP Attacks
* Routing Attacks

**Network Access Layer**

* ARP Spoofing
* MAC Flooding
* DHCP Starvation
* VLAN Hopping

### Where is it used?

* Network Penetration Testing
* Web Application Security Testing
* Packet Analysis
* Wireshark
* Burp Suite
* Nmap
* Firewall Testing
* Incident Response

---

## 💡 Key Points

* The TCP/IP Model has **4 layers**.
* It is the **standard model used on the Internet**.
* It focuses on practical implementation rather than theory.
* Every Internet communication uses TCP/IP protocols.
* It is essential for networking and penetration testing.

---

## ❓ Interview Questions

### 1. What is the TCP/IP Model?

### 2. How many layers are in the TCP/IP Model?

### 3. Which protocol is responsible for routing packets?

### 4. What is the difference between TCP and UDP?

### 5. Which layer is responsible for IP addressing?

### 6. Which layer handles Ethernet and Wi-Fi communication?

### 7. Why is the TCP/IP Model preferred over the OSI Model in real-world networking?

### 8. Which TCP/IP layer is commonly targeted by SQL Injection attacks?

---

## 📚 References

* **PortSwigger Web Security Academy** – HTTP & Networking Fundamentals
* **OWASP Web Security Testing Guide (WSTG)**
* **RFC 791** – Internet Protocol (IPv4)
* **RFC 793** – Transmission Control Protocol (TCP)
* **RFC 768** – User Datagram Protocol (UDP)
* **RFC 826** – Address Resolution Protocol (ARP)
* **RFC 1122** – Requirements for Internet Hosts

---

## 📊 TCP/IP Model Summary

| Layer | Name                  | Common Protocols                 |
| ----: | --------------------- | -------------------------------- |
|     4 | Application           | HTTP, HTTPS, FTP, DNS, SMTP, SSH |
|     3 | Transport             | TCP, UDP                         |
|     2 | Internet              | IP, ICMP, ARP, IPSec             |
|     1 | Network Access (Link) | Ethernet, Wi-Fi, PPP             |

### 🔄 OSI vs TCP/IP Mapping

| OSI Model    | TCP/IP Model   |
| ------------ | -------------- |
| Application  | Application    |
| Presentation | Application    |
| Session      | Application    |
| Transport    | Transport      |
| Network      | Internet       |
| Data Link    | Network Access |
| Physical     | Network Access |
