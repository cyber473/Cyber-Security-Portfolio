# Ports and Protocols

## 📌 Overview

Ports and Protocols are the foundation of networking. A **Protocol** defines how devices communicate, and a **Port** identifies which service or application receives the data.

---

## 🎯 What is it?

### Protocol

A **Protocol** is a set of rules used for communication over a network.

**Examples:** HTTP, HTTPS, FTP, SSH, DNS

### Port

A **Port** is a logical number that identifies a specific service or application.

**Examples:**

* HTTP → 80
* HTTPS → 443
* SSH → 22
* DNS → 53

---

## ❓ Why is it Needed?

* To communicate between devices
* To identify network services
* To send data to the correct application
* To manage network traffic

---

## ⚙️ How Does it Work?

1. Client sends a request.
2. The request uses a protocol (HTTP, HTTPS, etc.).
3. It goes to a specific port.
4. The server processes the request.
5. The server sends a response back.

---

## 🏠 Real Life Example

* House = Computer
* Door Number = Port
* Rules = Protocol
* Delivery Boy = Data

The delivery reaches the correct house only if the door number is correct.

---

## 🛠 Practical Demo

Scan Open Ports

```bash
nmap <IP>
```

Detect Service Version

```bash
nmap -sV <IP>
```

View Open Ports

```bash
ss -tuln
```

---

## 💻 Kali Linux Commands

```bash
nmap <IP>
nmap -sV <IP>
ss -tuln
netstat -tuln
```

---

## 🔐 VAPT Perspective

* Find open ports
* Identify running services
* Detect service versions
* Discover attack surface
* Start enumeration

---

## 💡 Key Points

* Protocol = Communication Rules
* Port = Service Number
* HTTP = 80
* HTTPS = 443
* SSH = 22
* DNS = 53

---

## ❓ Interview Questions

**Q1. What is a Protocol?**
A set of rules for network communication.

**Q2. What is a Port?**
A logical number that identifies a service.

**Q3. What is the default port of HTTP?**
80

**Q4. What is the default port of HTTPS?**
443

---

## 📚 References

* PortSwigger Web Security Academy
* OWASP
* IANA Port Registry
