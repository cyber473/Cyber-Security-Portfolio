# ARP (Address Resolution Protocol)

## 📌 Overview

ARP (Address Resolution Protocol) is used to find the **MAC Address** of a device using its **IP Address** in a Local Area Network (LAN).

---

## 🎯 What is it?

ARP is a network protocol that maps an **IP Address** to a **MAC Address**.

---

## ❓ Why is it Needed?

- Finds the destination MAC address
- Enables communication between devices in a LAN
- Connects Network Layer (IP) with Data Link Layer (MAC)

---

## ⚙️ How Does it Work?

1. A device wants to communicate with another device.
2. It knows the destination IP address.
3. It sends an **ARP Request** to the network.
4. The target device replies with its **MAC Address**.
5. The MAC address is stored in the **ARP Cache**.

---

## 🏠 Real Life Example

Imagine you know your friend's **house number (IP Address)** but not their **name (MAC Address)**.

You ask everyone, **"Who lives in House No. 25?"**

The correct person replies, **"It's me!"**

Now you know both the house number and the person's name.

---

## 🛠 Practical Demo

### View ARP Cache

```bash
ip neigh
```

### Show ARP Table

```bash
arp -a
```

### Ping a Device

```bash
ping 192.168.1.1
```

After pinging, check the ARP table again.

```bash
arp -a
```

---

## 💻 Kali Linux Commands

```bash
ip neigh

arp -a

ping 192.168.1.1

ip a
```

---

## 🔐 VAPT Perspective

A Pentester should understand ARP because it helps to:

- Discover devices in a local network
- Understand ARP Spoofing attacks
- Perform network reconnaissance
- Learn Man-in-the-Middle (MITM) attacks

---

## 💡 Key Points

- ARP maps IP Address to MAC Address.
- Works only in a Local Area Network (LAN).
- Uses ARP Request and ARP Reply.
- Stores results in the ARP Cache.
- Helps devices communicate on the same network.

---

## ❓ Interview Questions

### Q1. What is ARP?

ARP is a protocol that maps an IP Address to a MAC Address.

### Q2. Does ARP work on the Internet?

No. ARP works only inside a Local Area Network (LAN).

### Q3. What is an ARP Cache?

It is a table that stores recently learned IP-to-MAC address mappings.

### Q4. Which command shows the ARP table in Linux?

```bash
arp -a
```

or

```bash
ip neigh
```

---

## 📚 References

- PortSwigger Web Security Academy
- OWASP
- RFC 826
