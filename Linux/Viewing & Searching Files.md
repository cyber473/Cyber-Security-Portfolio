# 🔎 Viewing & Searching Files

## 📌 Overview

Linux me **Viewing & Searching Files** ka matlab files ke content ko dekhna aur system me specific files ya text ko quickly find karna hai.

## 🎯 What is it?

Linux me file content dekhne ke liye `cat`, `less`, `head`, `tail` aur files/search ke liye `find`, `locate`, `grep` commands use hote hain.

## ❓ Why is it Needed?

* File content check karne ke liye.
* Important files locate karne ke liye.
* Configuration aur log files analyze karne ke liye.
* VAPT me sensitive information find karne ke liye.

## ⚙️ How Does it Work?

Example:

```text id="e7g0my"
/var/log/
├── auth.log
├── syslog
└── apache2/
```

Hum `cat`, `less` ya `tail` se content dekh sakte hain aur `find`/`grep` se required information search kar sakte hain.

## 🏠 Real Life Example

Isko **library me book search** karne jaisa samjho:

* `ls` → Books ki list
* `cat` → Book padhna
* `less` → Page-by-page padhna
* `find` → Specific book dhundhna
* `grep` → Book ke andar specific word dhundhna

## 🛠 Practical Demo

```bash id="8yq6i4"
# View complete file
cat notes.txt

# View file page by page
less notes.txt

# Show first 10 lines
head notes.txt

# Show last 10 lines
tail notes.txt

# Find a file
find /home -name "notes.txt"

# Search text inside a file
grep "password" notes.txt
```

## 💻 Important Commands

| Command  | Purpose                   |
| -------- | ------------------------- |
| `cat`    | View file content         |
| `less`   | View content page-by-page |
| `head`   | Show beginning of file    |
| `tail`   | Show end of file          |
| `find`   | Search files/directories  |
| `locate` | Quickly locate files      |
| `grep`   | Search text/pattern       |

## 🔐 VAPT Perspective

Viewing & Searching Files is useful for:

* Sensitive File Discovery
* Configuration Review
* Log Analysis
* Credential Discovery
* Source Code Review
* Server Enumeration
* Privilege Escalation

Example:

```bash id="7m1zqk"
grep -R "password" /var/www/
```

> Authorized systems/labs par hi sensitive information search karein.

## 💡 Key Points

* `cat` → File read
* `less` → Page-by-page viewing
* `head` → First lines
* `tail` → Last lines
* `find` → File search
* `grep` → Text search
* `locate` → Fast file location

## ❓ Interview Questions

1. Which command is used to view a file?
2. What is the difference between `cat` and `less`?
3. What does `head` command do?
4. What does `tail` command do?
5. Which command is used to search for files?
6. Which command searches text inside files?
7. What is the difference between `find` and `grep`?

## 📚 References

* Linux Documentation
* GNU Coreutils Documentation
* Kali Linux Documentation
