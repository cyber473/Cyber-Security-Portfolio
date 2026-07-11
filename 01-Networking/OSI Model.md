
# OSI Model

## 📌 Overview

The **OSI (Open Systems Interconnection) Model** is a conceptual framework that explains how data travels from one device to another over a network. It divides the communication process into **seven layers**, making networking easier to understand, design, and troubleshoot.

---

## 🎯 What is it?

The **OSI Model** is a **7-layer networking reference model** developed by ISO. Each layer has a specific responsibility and works together to enable reliable communication between devices.

### The 7 Layers

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

---

## ❓ Why is it Needed?

The OSI Model is important because it:

* Standardizes network communication.
* Simplifies troubleshooting by separating functions into layers.
* Allows devices from different vendors to communicate.
* Helps engineers understand where problems occur.
* Provides a structured approach for network design and security.

---

## ⚙️ How Does it Work?

When you open a website in your browser:

1. **Application Layer** creates an HTTP request.
2. **Presentation Layer** formats or encrypts the data.
3. **Session Layer** establishes and manages the connection.
4. **Transport Layer** divides data into segments using TCP or UDP.
5. **Network Layer** determines the best route using IP addresses.
6. **Data Link Layer** adds MAC addresses and prepares the frame.
7. **Physical Layer** transmits the data as electrical, optical, or wireless signals.

The receiving device processes the data in the reverse order, from Layer 1 back to Layer 7.

---

## 🏠 Real Life Example

Imagine ordering a product online.

* **Application:** You place the order.
* **Presentation:** The package is wrapped and labeled.
* **Session:** The delivery tracking is maintained.
* **Transport:** The package is divided into shipments if necessary.
* **Network:** The courier selects the delivery route.
* **Data Link:** The local delivery center receives the package.
* **Physical:** The delivery person brings it to your home.

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

### Display Active TCP/UDP Connections

```bash
ss -tuln
```

### Send an HTTP Request

```bash
curl https://example.com
```

### Capture Network Packets

```bash
sudo tcpdump -i eth0
```

For Wi-Fi:

```bash
sudo tcpdump -i wlan0
```

### Launch Wireshark

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

# Show ARP neighbors
ip neigh

# DNS lookup
nslookup google.com

# Test connectivity
ping google.com

# Trace packet route
traceroute google.com

# View listening ports
ss -tuln

# Capture packets
sudo tcpdump -i eth0

# Open Wireshark
wireshark
```

---

## 🔐 VAPT Perspective

### Why should a Pentester know the OSI Model?

Understanding the OSI Model helps identify where an attack occurs and which protocols are involved.

### Common Attacks by Layer

**Layer 2 (Data Link)**

* ARP Spoofing
* MAC Flooding

**Layer 3 (Network)**

* IP Spoofing
* Routing Attacks

**Layer 4 (Transport)**

* Port Scanning
* SYN Scan
* SYN Flood

**Layer 7 (Application)**

* SQL Injection
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Server-Side Request Forgery (SSRF)
* File Upload Vulnerabilities
* Authentication Bypass

### Where is it used?

* Network Penetration Testing
* Web Application Testing
* Packet Analysis
* Firewall Testing
* Wireshark Analysis
* Burp Suite Traffic Analysis
* Incident Response

---

## 💡 Key Points

* The OSI Model consists of **7 layers**.
* Each layer performs a specific networking function.
* Data is **encapsulated** while sending and **decapsulated** while receiving.
* It is widely used for troubleshooting, learning networking, and penetration testing.
* Many cyber attacks target specific OSI layers.

---

## ❓ Interview Questions

### 1. What is the OSI Model?

### 2. How many layers are there in the OSI Model?

### 3. Which layer is responsible for IP addressing?

### 4. Which layer uses MAC addresses?

### 5. What is the difference between TCP and UDP?

### 6. Which OSI layer does HTTP operate on?

### 7. Which attacks target Layer 2?

### 8. Which OSI layer is commonly targeted by SQL Injection and XSS attacks?

---

## 📚 References

* **PortSwigger Web Security Academy** – Web Security & HTTP Fundamentals
* **OWASP Web Security Testing Guide (WSTG)**
* **OWASP Top 10**
* **RFC 791** – Internet Protocol (IPv4)
* **RFC 793** – Transmission Control Protocol (TCP)
* **RFC 768** – User Datagram Protocol (UDP)
* **ISO/IEC 7498-1** – Open Systems Interconnection (OSI) Reference Model

---

## 📊 OSI Model Summary

| Layer | Name         | Common Protocols                           |
| ----: | ------------ | ------------------------------------------ |
|     7 | Application  | HTTP, HTTPS, FTP, DNS                      |
|     6 | Presentation | SSL/TLS, JPEG, ASCII                       |
|     5 | Session      | RPC, NetBIOS                               |
|     4 | Transport    | TCP, UDP                                   |
|     3 | Network      | IP, ICMP, IPSec                            |
|     2 | Data Link    | Ethernet, ARP, PPP                         |
|     1 | Physical     | Ethernet Cable, Fiber Optic, Wi-Fi Signals |
