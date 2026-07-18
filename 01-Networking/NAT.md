# NAT (Network Address Translation)

## 📌 Overview

Network Address Translation (NAT) is a networking technique that allows multiple devices to share a single public IP address. It is commonly used in home, office, and enterprise networks.

---

## 🎯 What is it?

NAT is a process that translates a **private IP address** into a **public IP address** before sending data to the Internet.

---

## ❓ Why is it Needed?

- Saves public IP addresses
- Hides private IP addresses
- Allows multiple devices to access the Internet
- Adds a basic layer of security

---

## ⚙️ How Does it Work?

1. A device sends a request to the Internet.
2. The router replaces the private IP with its public IP.
3. The request reaches the destination server.
4. The server sends the response back.
5. The router forwards the response to the correct device.

---

## 🏠 Real Life Example

Imagine a family using one Wi-Fi router.

- Phone → 192.168.1.10
- Laptop → 192.168.1.20
- PC → 192.168.1.30

All devices access the Internet using **one public IP** provided by the ISP.

---

## 🛠 Practical Demo

### Check Your Private IP

```bash
ip a
```

### Check Your Public IP

```bash
curl ifconfig.me
```

### View Routing Table

```bash
ip route
```

---

## 💻 Kali Linux Commands

```bash
ip a

ip route

curl ifconfig.me
```

---

## 🔐 VAPT Perspective

A Pentester should understand NAT because it helps to:

- Identify private and public IP addresses
- Understand internal network architecture
- Perform network reconnaissance
- Analyze firewall and router configurations

---

## 💡 Key Points

- NAT = Private IP ➜ Public IP
- Saves IPv4 addresses
- Commonly used in routers
- Allows multiple devices to share one public IP
- Improves network security

---

## ❓ Interview Questions

### Q1. What is NAT?

NAT is a technique that translates private IP addresses into a public IP address.

### Q2. Why is NAT used?

To save public IP addresses and allow multiple devices to access the Internet.

### Q3. Where is NAT commonly used?

Home routers, office networks, and enterprise networks.

---

## 📚 References

- PortSwigger Web Security Academy
- OWASP
- RFC 3022
