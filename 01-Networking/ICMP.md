# ICMP (Internet Control Message Protocol)

## 📌 Overview

ICMP (Internet Control Message Protocol) is used to send error messages and network status information. It helps diagnose and troubleshoot network problems.

---

## 🎯 What is it?

ICMP is a network protocol used for network testing, error reporting, and diagnostics.

---

## ❓ Why is it Needed?

- Tests network connectivity
- Reports network errors
- Helps troubleshoot network issues
- Used by Ping and Traceroute

---

## ⚙️ How Does it Work?

1. A device sends an ICMP Echo Request.
2. The destination device receives the request.
3. It sends an ICMP Echo Reply.
4. The sender confirms that the device is reachable.

---

## 🏠 Real Life Example

You call your friend and ask, **"Are you there?"**

If your friend replies, **"Yes, I'm here!"**, you know the connection is working.

---

## 🛠 Practical Demo

### Check Network Connectivity

```bash
ping google.com
```

### Send 4 Ping Requests

```bash
ping -c 4 google.com
```

### Trace the Network Path

```bash
traceroute google.com
```

---

## 💻 Kali Linux Commands

```bash
ping google.com

ping -c 4 google.com

traceroute google.com

tracepath google.com
```

---

## 🔐 VAPT Perspective

A Pentester should understand ICMP because it helps to:

- Check if a host is alive
- Discover active devices
- Perform network reconnaissance
- Troubleshoot network connectivity

---

## 💡 Key Points

- ICMP is used for network diagnostics.
- Ping uses ICMP.
- Traceroute uses ICMP (or UDP, depending on the OS).
- ICMP does not transfer application data.
- Helps identify network problems.

---

## ❓ Interview Questions

### Q1. What is ICMP?

ICMP is a protocol used for network diagnostics and error reporting.

### Q2. Which command uses ICMP?

```bash
ping
```

### Q3. Why is ICMP important?

It helps test connectivity and troubleshoot network issues.

### Q4. Does ICMP use TCP or UDP?

No. ICMP is a separate network protocol and does not use TCP or UDP.

---

## 📚 References

- PortSwigger Web Security Academy
- OWASP
- RFC 792
