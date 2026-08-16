# 📂 File System Navigation

## 📌 Overview

File System Navigation means Linux me **directories ke andar move karna, current location check karna, aur files/directories ko list karna**.

## 🎯 What is it?

Linux terminal me navigation ke liye mainly `pwd`, `ls`, aur `cd` commands use kiye jate hain.

## ❓ Why is it Needed?

File System Navigation important hai because it:

* Files aur directories locate karne me help karta hai.
* Different directories ke beech move karne deta hai.
* Command-line work ko easy banata hai.
* VAPT aur Linux enumeration me frequently use hota hai.

## ⚙️ How Does it Work?

Linux me current location ek **path** se identify hoti hai.

Example:

```text
/home/kali/Documents
```

* `/` → Root
* `home` → Directory
* `kali` → User directory
* `Documents` → Current directory

## 🏠 Real Life Example

File System ko ek **building** samjho.

* `pwd` → Tum abhi kis room me ho?
* `ls` → Room ke andar kya hai?
* `cd` → Dusre room me jana
* `cd ..` → Ek level peeche jana

## 🛠 Practical Demo

```bash
# Current directory
pwd

# List files
ls

# Detailed listing
ls -la

# Enter a directory
cd Documents

# Go one level back
cd ..

# Go to home directory
cd ~

# Go to root directory
cd /

# Go to previous directory
cd -
```

## 💻 Important Commands

| Command  | Purpose                                 |
| -------- | --------------------------------------- |
| `pwd`    | Current directory                       |
| `ls`     | List files/directories                  |
| `ls -la` | Detailed listing including hidden files |
| `cd`     | Change directory                        |
| `cd ..`  | Parent directory                        |
| `cd ~`   | Home directory                          |
| `cd /`   | Root directory                          |
| `cd -`   | Previous directory                      |

## 🔐 VAPT Perspective

File System Navigation is useful for:

* Directory Enumeration
* Finding Configuration Files
* Finding Sensitive Files
* Log Analysis
* Privilege Escalation
* Server Enumeration

## 💡 Key Points

* `pwd` → Where am I?
* `ls` → What is here?
* `cd` → Move to another directory.
* `cd ..` → Move to parent directory.
* `cd ~` → Go to home directory.
* `cd /` → Go to root directory.
* `ls -la` → Show hidden files too.

## ❓ Interview Questions

1. What is File System Navigation?
2. Which command shows the current directory?
3. Which command is used to change directories?
4. What does `cd ..` do?
5. What does `cd ~` do?
6. How can you view hidden files in Linux?
7. What is the difference between `cd /` and `cd ~`?

## 📚 References

* Linux Documentation
* Kali Linux Documentation
* GNU Coreutils Documentation
