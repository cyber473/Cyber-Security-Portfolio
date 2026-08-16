# ⚙️ Package Management & System Processes

## 📌 Overview

**Package Management** is used to install, update, and remove software in Linux.

**System Processes** are running programs and services that can be monitored and managed.

## 🎯 What is it?

### Package Management

Linux uses **package managers** to manage software packages.

Kali Linux and Debian-based systems mainly use **APT**.

### System Processes

A **process** is a running instance of a program. Each process has a unique **PID (Process ID)**.

## ❓ Why is it Needed?

It helps to:

* Install and update software.
* Apply security updates.
* Monitor running processes.
* Identify unnecessary or suspicious processes.
* Maintain system security and performance.

## ⚙️ How Does it Work?

### Package Management

```text id="7tq3xc"
Repository
    ↓
Package Manager (APT)
    ↓
Download Package
    ↓
Install / Update
```

### Process Management

```text id="m6y9ra"
Program Starts
      ↓
Process Created
      ↓
PID Assigned
      ↓
Process Runs
      ↓
Process Stops
```

## 🏠 Real Life Example

Think of a **package manager like an app store**.

A **process** is like an application that is currently running.

* Install → Install an app
* Update → Update an app
* Remove → Uninstall an app
* Process → Running application

## 🛠 Practical Demo

```bash id="6z5h9a"
# Update package list
sudo apt update

# Upgrade installed packages
sudo apt upgrade

# Install a package
sudo apt install nmap

# Remove a package
sudo apt remove nmap

# Show running processes
ps aux

# Monitor processes
top

# Find a process
pgrep ssh

# Stop a process
kill PID
```

## 💻 Important Commands

| Command       | Purpose                    |
| ------------- | -------------------------- |
| `apt update`  | Update package list        |
| `apt upgrade` | Upgrade installed packages |
| `apt install` | Install a package          |
| `apt remove`  | Remove a package           |
| `apt search`  | Search for packages        |
| `ps aux`      | Show running processes     |
| `top`         | Monitor processes          |
| `pgrep`       | Find a process             |
| `kill`        | Terminate a process        |

## 🔐 VAPT Perspective

Package & Process Management is useful for:

* Vulnerable Software Identification
* Security Patch Checking
* Service Enumeration
* Process Enumeration
* Privilege Escalation
* Suspicious Process Detection
* Linux Server Hardening

Example:

```bash id="j8v4kp"
ps aux
```

This can help identify unusual or unnecessary running processes during an authorized security assessment.

## 💡 Key Points

* **APT** is commonly used in Kali/Debian-based systems.
* `apt update` updates the package list.
* `apt upgrade` upgrades installed packages.
* A process is a running program.
* Every process has a **PID**.
* `ps` shows process information.
* `top` provides live process monitoring.
* `kill` terminates a process.

## ❓ Interview Questions

1. What is Package Management?
2. What is APT?
3. What is the difference between `apt update` and `apt upgrade`?
4. What is a process?
5. What is a PID?
6. Which command shows running processes?
7. What is the purpose of `top`?
8. What is the purpose of the `kill` command?

## 📚 References

* Debian Documentation
* Kali Linux Documentation
* Linux Documentation
* APT Documentation
