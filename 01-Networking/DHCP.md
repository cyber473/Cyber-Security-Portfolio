# DHCP (Dynamic Host Configuration Protocol)

## 📌 Overview

DHCP automatically assigns IP addresses to devices on a network.

---

## 🎯 What is it?

DHCP is a protocol that provides IP configuration automatically.

---

## ❓ Why is it Needed?

- Automatic IP assignment
- Saves time
- Reduces configuration errors

---

## ⚙️ How Does it Work?

1. Device requests an IP.
2. DHCP Server offers an IP.
3. Device accepts the offer.
4. Server confirms the assignment.

---

## 🏠 Real Life Example

A hotel automatically gives a room number when you check in.

---

## 🛠 Practical Demo

Check IP Address

ip a

View Routing Table

ip route

---

## 💻 Kali Linux Commands

ip a

ip route

nmcli device show

---

## 🔐 VAPT Perspective

- Identify DHCP Server
- Analyze Network Configuration
- Gather Network Information

---

## 💡 Key Points

- Assigns IP automatically.
- Reduces manual work.
- Uses UDP Ports 67 and 68.

---

## ❓ Interview Questions

Q1. What is DHCP?

A protocol that automatically assigns IP addresses.

Q2. Which ports does DHCP use?

UDP 67 and UDP 68.

---

## 📚 References

- PortSwigger
- OWASP
- RFC 2131
