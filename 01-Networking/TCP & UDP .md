# TCP vs UDP

## 📌 Overview

TCP and UDP are two transport layer protocols. TCP is reliable and connection-based, while UDP is fast and connectionless.

---

## 🎯 What is it?

### TCP (Transmission Control Protocol)

TCP provides reliable and secure data delivery.

### UDP (User Datagram Protocol)

UDP sends data quickly without checking delivery.

---

## ❓ Why is it Needed?

### TCP

* Reliable communication
* Error checking
* Ordered data delivery

### UDP

* Fast communication
* Low delay
* Real-time applications

---

## ⚙️ How Does it Work?

### TCP

1. Establishes a connection.
2. Sends data.
3. Confirms delivery (ACK).
4. Closes the connection.

### UDP

1. Sends data.
2. No connection.
3. No acknowledgment.
4. Faster transmission.

---

## 🏠 Real Life Example

**TCP:** Sending a bank transaction. Every packet must reach safely.

**UDP:** Watching a live cricket match. Speed is more important than perfect delivery.

---

## 🛠 Practical Demo

Check TCP Ports

```bash
ss -t
```

Check UDP Ports

```bash
ss -u
```

Scan TCP Ports

```bash
nmap -sT <IP>
```

Scan UDP Ports

```bash
nmap -sU <IP>
```

---

## 💻 Kali Linux Commands

```bash
ss -t
ss -u
nmap -sT <IP>
nmap -sU <IP>
```

---

## 🔐 VAPT Perspective

* Identify TCP and UDP services
* Scan open ports
* Find running services
* Start enumeration

---

## 💡 Key Points

| TCP                 | UDP               |
| ------------------- | ----------------- |
| Reliable            | Fast              |
| Connection-Oriented | Connectionless    |
| Uses ACK            | No ACK            |
| Error Checking      | No Error Recovery |
| Slower              | Faster            |

---

## ❓ Interview Questions

**Q1. What is TCP?**
A reliable, connection-oriented protocol.

**Q2. What is UDP?**
A fast, connectionless protocol.

**Q3. Which protocol is faster?**
UDP.

**Q4. Which protocol is more reliable?**
TCP.

---

## 📚 References

* PortSwigger Web Security Academy
* OWASP
* RFC 793 (TCP)
* RFC 768 (UDP)
