# 🔐 File Permissions & Sudo

## 📌 Overview

Linux me **File Permissions** decide karti hain ki kaun kisi file ya directory ko **read, write, ya execute** kar sakta hai.

`sudo` users ko required permission ke saath commands execute karne deta hai.

## 🎯 What is it?

Linux permissions mainly 3 types ki hoti hain:

* `r` → Read
* `w` → Write
* `x` → Execute

Permissions 3 users/groups ke liye hoti hain:

* **Owner**
* **Group**
* **Others**

Example:

```text
-rwxr-xr--
```

## ❓ Why is it Needed?

* Unauthorized access prevent karta hai.
* Sensitive files protect karta hai.
* Users ke access ko control karta hai.
* Privilege management me help karta hai.
* Server security ke liye important hai.

## ⚙️ How Does it Work?

Example:

```text
-rwxr-xr--
 │││ │││ │││
 │││ │││ └── Others
 │││ └────── Group
 └────────── Owner
```

Common permission values:

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

File permissions ko **ghar ki keys** ki tarah samjho:

* `r` → Ghar ke andar dekhna
* `w` → Cheezein change karna
* `x` → File/program run karna

`sudo` → Special permission wali master key jaisa hai.

## 🛠 Practical Demo

```bash
# Show permissions
ls -l

# Change permissions
chmod 755 script.sh

# Change owner
sudo chown user file.txt

# Run command with elevated privileges
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
| `id`    | Show user/group information          |

## 🔐 VAPT Perspective

File Permissions & Sudo are important for:

* Privilege Escalation
* Sensitive File Access
* Misconfiguration Detection
* SUID/SGID Enumeration
* Linux Server Hardening
* Access Control Testing

Example:

```bash
# Find SUID files
find / -perm -4000 -type f 2>/dev/null
```

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
