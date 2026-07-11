
# MAC Address

## 📌 Overview

**MAC (Media Access Control) Address** is a method of uniquely identifying a network interface card (NIC) on a local network. Every network device has a MAC address that is used for communication within the same LAN.

---

## 🎯 What is it?

A **MAC Address** is a **48-bit (6-byte) unique hardware address** assigned to a network interface by the manufacturer. It operates at the **Data Link Layer (Layer 2)** of the OSI Model.

### Example MAC Address

```text
00:1A:2B:3C:4D:5E
```

or

```text
00-1A-2B-3C-4D-5E
```

---

## ❓ Why is it Needed?

MAC Addressing is important because it:

* Uniquely identifies devices on a Local Area Network (LAN).
* Enables communication between devices on the same network.
* Allows switches to forward frames to the correct device.
* Supports ARP (Address Resolution Protocol).
* Plays a critical role in network security and monitoring.

---

## ⚙️ How Does it Work?

When Device A wants to communicate with Device B on the same LAN:

1. Device A knows the destination IP address.
2. It uses **ARP** to find the destination MAC address.
3. The switch forwards the Ethernet frame based on the MAC address.
4. Device B receives the frame and processes the data.

If the destination is outside the LAN, the frame is first sent to the **default gateway's MAC address**.

---

## 🏠 Real Life Example

Imagine an apartment building.

* **IP Address** = Apartment address.
* **MAC Address** = The nameplate on the apartment door.

The courier first reaches the correct building using the address (IP), then identifies the correct apartment using the nameplate (MAC).

---

## 🛠 Practical Demo

### Display MAC Address

```bash
ip link
```

---

### Show Detailed Network Information

```bash
ip addr
```

---

### View ARP Cache

```bash
ip neigh
```

---

### Check Network Interface Details

```bash
ifconfig
```

---

### Capture Ethernet Frames

```bash
sudo tcpdump -e -i eth0
```

---

### Open Wireshark

```bash
wireshark
```

Apply the display filter:

```text
eth.addr
```

---

## 💻 Kali Linux Commands

```bash
# Show network interfaces
ip link

# Display IP and MAC addresses
ip addr

# Show ARP table
ip neigh

# Legacy interface information
ifconfig

# Display hardware information
sudo lshw -class network

# Capture Ethernet frames
sudo tcpdump -e -i eth0

# Launch Wireshark
wireshark
```

---

## 🔐 VAPT Perspective

### Why should a Pentester know MAC Addressing?

MAC addresses are fundamental during **internal network penetration testing**. Many Layer 2 attacks rely on understanding how MAC addresses are used.

### Where is it used?

* Internal Network Pentesting
* ARP Analysis
* Wireshark Packet Analysis
* Switch Security Testing
* MAC Filtering Assessment
* Rogue Device Detection
* Network Monitoring
* Incident Response

### Common MAC-Related Attacks

* ARP Spoofing
* MAC Flooding
* MAC Spoofing
* CAM Table Overflow
* Man-in-the-Middle (MITM)
* Rogue Device Attacks

---

## 💡 Key Points

* A MAC Address is a **48-bit hardware address**.
* It operates at **OSI Layer 2 (Data Link Layer)**.
* It is used only within the **local network (LAN)**.
* Switches forward Ethernet frames using MAC addresses.
* ARP maps an IP address to a MAC address.

---

## ❓ Interview Questions

### 1. What is a MAC Address?

### 2. What is the size of a MAC Address?

### 3. Which OSI layer uses MAC addresses?

### 4. What is the difference between an IP Address and a MAC Address?

### 5. Which protocol maps an IP address to a MAC address?

### 6. Which Linux command displays the MAC address?

### 7. Can a MAC address be changed?

### 8. What is MAC Spoofing?

### 9. What is ARP Spoofing?

### 10. Why is MAC Addressing important in penetration testing?

---

## 📚 References

* **PortSwigger Web Security Academy** – Networking Fundamentals
* **OWASP Web Security Testing Guide (WSTG)**
* **IEEE 802.3** – Ethernet Standard
* **RFC 826** – Address Resolution Protocol (ARP)
* **RFC 894** – IP over Ethernet

---

## 📊 MAC Addressing Summary

| Feature          | Description              |
| ---------------- | ------------------------ |
| Full Form        | Media Access Control     |
| OSI Layer        | Layer 2 (Data Link)      |
| Address Length   | 48-bit (6 Bytes)         |
| Format           | Hexadecimal              |
| Example          | 00:1A:2B:3C:4D:5E        |
| Used By          | Switches                 |
| Scope            | Local Area Network (LAN) |
| Related Protocol | ARP                      |

### 📍 IP Address vs MAC Address

| IP Address            | MAC Address                        |
| --------------------- | ---------------------------------- |
| Logical Address       | Physical Hardware Address          |
| Layer 3 (Network)     | Layer 2 (Data Link)                |
| Can Change            | Usually Permanent (can be spoofed) |
| Used Across Networks  | Used Within Local Network          |
| Example: 192.168.1.10 | Example: 00:1A:2B:3C:4D:5E         |
