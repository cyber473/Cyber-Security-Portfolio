# 📁 File & Directory Management

## 📌 Overview

File & Directory Management means Linux me **files aur folders ko create, copy, move, rename aur delete karna**.

## 🎯 What is it?

Linux terminal me files aur directories manage karne ke liye commands jaise `touch`, `mkdir`, `cp`, `mv`, aur `rm` use hote hain.

## ❓ Why is it Needed?

File & Directory Management important hai because it:

* Files aur folders organize karne me help karta hai.
* Data ko copy aur move karne deta hai.
* Unnecessary files remove karne deta hai.
* Linux administration aur VAPT me frequently use hota hai.

## ⚙️ How Does it Work?

Example:

```text id="t3r8qs"
Cyber-Security/
├── Notes/
│   └── linux.txt
└── Labs/
```

Commands ke through hum is structure ko create aur modify kar sakte hain.

## 🏠 Real Life Example

Computer ke folders ko **almirah** ki tarah samjho:

* `mkdir` → Naya folder banana
* `touch` → Nayi file banana
* `cp` → Copy banana
* `mv` → Move/Rename karna
* `rm` → Delete karna

## 🛠 Practical Demo

```bash id="k2zv5p"
# Create a file
touch notes.txt

# Create a directory
mkdir CyberSecurity

# Copy a file
cp notes.txt CyberSecurity/

# Move a file
mv notes.txt CyberSecurity/

# Rename a file
mv old.txt new.txt

# Remove a file
rm new.txt

# Remove an empty directory
rmdir CyberSecurity
```

## 💻 Important Commands

| Command | Purpose                |
| ------- | ---------------------- |
| `touch` | Create a file          |
| `mkdir` | Create a directory     |
| `cp`    | Copy files/directories |
| `mv`    | Move or rename         |
| `rm`    | Delete files           |
| `rmdir` | Delete empty directory |
| `ls`    | List files/directories |

### ⚠️ Important

`rm -r` directories ko recursively delete kar sakta hai, isliye use karne se pehle path carefully check karo.

## 🔐 VAPT Perspective

File & Directory Management is useful for:

* Creating Payload/Test Files
* Organizing Recon Data
* Saving Scan Results
* Managing Scripts
* Moving Evidence/Reports
* Preparing Exploitation Labs

## 💡 Key Points

* `touch` → File create
* `mkdir` → Directory create
* `cp` → Copy
* `mv` → Move/Rename
* `rm` → Delete
* `rmdir` → Empty directory delete
* Linux me file management command line se efficiently kiya ja sakta hai.

## ❓ Interview Questions

1. How do you create a file in Linux?
2. How do you create a directory?
3. What is the difference between `cp` and `mv`?
4. How do you rename a file?
5. How do you delete a file?
6. What is the purpose of `rmdir`?
7. What is the difference between `rm` and `rmdir`?

## 📚 References

* Linux Documentation
* GNU Coreutils Documentation
* Kali Linux Documentation
