#  Linux File System Structure

## 📌 Overview

The Linux File System Structure organizes all files and directories in a hierarchical (tree-like) format. Everything in Linux starts from the **root directory (`/`)**.

---

## 🎯 What is it?

The Linux file system stores system files, user files, applications, and configuration files in different directories.

### Common Directories

* `/` → Root Directory
* `/home` → User files
* `/root` → Root user's home
* `/etc` → Configuration files
* `/bin` → Essential commands
* `/usr` → Installed applications
* `/var` → Log and variable files
* `/tmp` → Temporary files
* `/dev` → Device files
* `/proc` → Process information

---

## ❓ Why is it Needed?

* Organizes files efficiently.
* Makes system management easier.
* Separates system and user data.
* Improves security and maintenance.

---

## ⚙️ How Does it Work?

1. The Root (`/`) is the top-level directory.
2. All other directories are inside it.
3. Every file has a unique path.

Example:

```text
/home/kali/Documents/notes.txt
```

---

## 🏠 Real Life Example

Think of the file system like a **tree**.

* `/` → Tree trunk
* Folders → Branches
* Files → Leaves

---

## 🛠 Practical Demo

```bash
pwd
ls
cd /
tree -L 2
```

---

## 💻 Kali Linux Commands

```bash
# Show current directory
pwd

# List files
ls

# Go to root directory
cd /

# Show directory structure
tree -L 2

# Display mounted file systems
df -h
```

---

## 🔐 VAPT Perspective

Linux File System is used in:

* File Enumeration
* Privilege Escalation
* Configuration Review
* Log Analysis
* Sensitive File Discovery

---

## 💡 Key Points

* Everything starts from `/` (Root).
* `/home` stores user files.
* `/etc` stores configuration files.
* `/var/log` stores log files.
* `/tmp` stores temporary files.

---

## ❓ Interview Questions

1. What is the root directory in Linux?
2. What is stored in `/etc`?
3. What is the purpose of `/home`?
4. Which directory stores log files?
5. Which command shows the current directory?

---

## 📚 References

* Linux Foundation Documentation
* Filesystem Hierarchy Standard (FHS)

---

## 📊 Important Directories

| Directory | Purpose              |
| --------- | -------------------- |
| `/`       | Root directory       |
| `/home`   | User files           |
| `/root`   | Root user home       |
| `/etc`    | Configuration files  |
| `/bin`    | Essential commands   |
| `/usr`    | Installed programs   |
| `/var`    | Logs & variable data |
| `/tmp`    | Temporary files      |
| `/dev`    | Device files         |
| `/proc`   | Process information  |
