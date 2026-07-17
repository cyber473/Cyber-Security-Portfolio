# DNS (Domain Name System)

## 📌 Overview
DNS converts a domain name into an IP address. It helps users access websites using names instead of IP addresses.

---

## 🎯 What is it?

DNS is a system that translates domain names (example.com) into IP addresses.

---

## ❓ Why is it Needed?

- Easy to remember website names
- Finds the correct server
- Faster internet access

---

## ⚙️ How Does it Work?

1. User enters a domain name.
2. DNS Resolver receives the request.
3. DNS finds the IP address.
4. Browser connects to the server.
5. Website loads.

---

## 🏠 Real Life Example

A phone contact saves a person's name instead of their phone number.

---

## 🛠 Practical Demo

Find IP Address

dig google.com

nslookup google.com

---

## 💻 Kali Linux Commands

dig google.com

nslookup google.com

host google.com

---

## 🔐 VAPT Perspective

- Perform DNS Enumeration
- Find Subdomains
- Identify Name Servers
- Collect Recon Information

---

## 💡 Key Points

- DNS maps domain names to IP addresses.
- Uses Port 53.
- Works with UDP and TCP.

---

## ❓ Interview Questions

Q1. What is DNS?

A system that converts domain names into IP addresses.

Q2. Which port does DNS use?

Port 53.

---

## 📚 References

- PortSwigger
- OWASP
- RFC 1034
