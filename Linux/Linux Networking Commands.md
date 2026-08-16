# 🌐 Linux Networking Commands

## 📌 Overview

Linux Networking Commands are used to **view network configuration, test connectivity, inspect routes, and troubleshoot network-related issues**.

## 🎯 What is it?

Linux provides commands such as `ip`, `ping`, `ss`, `traceroute`, `nslookup`, and `curl` to work with and analyze network connections.

## ❓ Why is it Needed?

Networking commands help to:

* Check IP addresses and interfaces.
* Test network connectivity.
* View routing information.
* Check open ports and connections.
* Troubleshoot network problems.
* Perform basic network enumeration.

## ⚙️ How Does it Work?

Basic workflow:

```text id="gq9f6n"
Check Interface
      ↓
Check IP Address
      ↓
Test Connectivity
      ↓
Check Routes
      ↓
Inspect Connections
      ↓
Analyze Network
```

## 🛠 Practical Demo

```bash id="8u5m2x"
# Show IP addresses
ip addr

# Show network interfaces
ip link

# Show routing table
ip route

# Test connectivity
ping 8.8.8.8

# Check DNS resolution
nslookup google.com

# Trace network path
traceroute google.com

# Show listening ports
ss -tuln

# Test HTTP connection
curl -I https://example.com

# Show ARP/neighbor table
ip neigh
```

## 💻 Important Commands

| Command      | Purpose                        |
| ------------ | ------------------------------ |
| `ip addr`    | Show IP addresses              |
| `ip link`    | Show network interfaces        |
| `ip route`   | Show routing table             |
| `ping`       | Test connectivity              |
| `ss`         | Show network connections/ports |
| `traceroute` | Trace network path             |
| `nslookup`   | DNS lookup                     |
| `curl`       | Test HTTP/HTTPS requests       |
| `ip neigh`   | Show ARP/neighbor information  |
| `hostname`   | Show system hostname           |

## 🔐 VAPT Perspective

Networking commands are useful for:

* Network Enumeration
* Host Discovery
* Service Enumeration
* Connectivity Testing
* Route Analysis
* DNS Enumeration
* Troubleshooting
* Security Assessment

Example:

```bash id="2q5y7d"
ip addr
ip route
ss -tuln
```

These commands can provide useful network information during an **authorized security assessment**.

## 💡 Key Points

* `ip addr` → IP information.
* `ip link` → Network interfaces.
* `ip route` → Routing table.
* `ping` → Connectivity test.
* `ss` → Network connections and listening ports.
* `traceroute` → Network path.
* `nslookup` → DNS information.
* `curl` → HTTP/HTTPS testing.
* `ip neigh` → Neighbor/ARP information.

## ❓ Interview Questions

1. Which command displays IP addresses in Linux?
2. What is the purpose of `ip route`?
3. Which command tests network connectivity?
4. What does `ss -tuln` show?
5. What is the purpose of `traceroute`?
6. Which command is used for DNS lookup?
7. What is the purpose of `curl`?
8. Which command displays the ARP/neighbor table?

## 📚 References

* Linux Documentation
* iproute2 Documentation
* Kali Linux Documentation
* GNU Inetutils Documentation
