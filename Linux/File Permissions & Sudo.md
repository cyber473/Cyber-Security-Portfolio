# 🔐 File Permissions & Sudo

## 📌 Overview

Linux **File Permissions** control who can **read, write, or execute** a file or directory.

`sudo` allows authorized users to run commands with elevated privileges.

## 🎯 What is it?

Linux permissions have three basic types:

* `r` → Read
* `w` → Write
* `x` → Execute

Permissions apply to:

* **Owner**
* **Group**
* **Others**

Example:

```text
-rwxr-xr--
```

## ❓ Why is it Needed?

File permissions help to:

* Prevent unauthorized access.
* Protect sensitive files.
* Control user access.
* Maintain system security.
* Manage privileges safely.

## ⚙️ How Does it Work?

Permission values:

```text
r = 4
w = 2
x = 1
```

Example:

```bash
chmod 755 script.sh
```

Meaning:

```text
Owner  → rwx = 7
Group  → r-x = 5
Others → r-x = 5
```

## 🏠 Real Life Example

Think of file permissions like **keys to a house**:

* `r` → Enter and view
* `w` → Modify things
* `x` → Run/use the program
* `sudo` → Authorized master access

## 🛠 Practical Demo

```bash
# Show file permissions
ls -l

# Change permissions
chmod 755 script.sh

# Change file owner
sudo chown user file.txt

# Change group
sudo chgrp group file.txt

# Run a command with elevated privileges
sudo command
```

## 💻 Important Commands

| Command | Purpose                              |
| ------- | ------------------------------------ |
| `ls -l` | Show file permissions                |
| `chmod` | Change permissions                   |
| `chown` | Change file owner                    |
| `chgrp` | Change group                         |
| `sudo`  | Run command with elevated privileges |
| `id`    | Show user and group information      |

## 🔐 VAPT Perspective

File Permissions & Sudo are important for:

* Privilege Escalation
* Sensitive File Access
* Misconfiguration Detection
* SUID/SGID Enumeration
* Access Control Testing
* Linux Server Hardening

Example:

```bash
find / -perm -4000 -type f 2>/dev/null
```

This can be used in an authorized lab to find **SUID files**.

## 💡 Key Points

* `r` = Read
* `w` = Write
* `x` = Execute
* Permissions apply to Owner, Group, and Others.
* `chmod` changes permissions.
* `chown` changes ownership.
* `sudo` provides elevated privileges.
* Weak permissions can create security risks.

## ❓ Interview Questions

1. What are Linux file permissions?
2. What do `r`, `w`, and `x` mean?
3. What are Owner, Group, and Others?
4. What does `chmod 755` mean?
5. What is `sudo`?
6. What is the difference between `chmod` and `chown`?
7. What is SUID?
8. Why are file permissions important in Linux security?

## 📚 References

* Linux Documentation
* GNU Coreutils Documentation
* Kali Linux Documentation
