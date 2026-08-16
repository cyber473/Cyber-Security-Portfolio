# 🔎 Viewing & Searching Files

## 📌 Overview

Viewing & Searching Files means **reading file contents and finding specific files or text** in the Linux file system.

## 🎯 What is it?

Linux provides commands such as `cat`, `less`, `head`, `tail`, `find`, `locate`, and `grep` to view and search files.

## ❓ Why is it Needed?

It helps to:

* Read file contents.
* Find specific files and directories.
* Search for specific text.
* Analyze configuration and log files.
* Find sensitive information during security testing.

## ⚙️ How Does it Work?

Example:

```text id="2z8g5w"
/var/log/
├── auth.log
├── syslog
└── apache2/
```

You can use viewing commands to read these files and searching commands to find specific files or text.

## 🏠 Real Life Example

Think of it like searching for a book in a library:

* `ls` → List the available books.
* `cat` → Read the book.
* `less` → Read page by page.
* `find` → Find a specific book.
* `grep` → Search for a specific word inside a book.

## 🛠 Practical Demo

```bash id="w5g7py"
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

| Command  | Purpose                      |
| -------- | ---------------------------- |
| `cat`    | View file contents           |
| `less`   | View contents page by page   |
| `head`   | Show the beginning of a file |
| `tail`   | Show the end of a file       |
| `find`   | Search for files/directories |
| `locate` | Quickly locate files         |
| `grep`   | Search for text or patterns  |

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

```bash id="x4t1vn"
grep -R "password" /var/www/
```

Use such searches only on **authorized systems or labs**.

## 💡 Key Points

* `cat` → View file contents.
* `less` → View files page by page.
* `head` → Show first lines.
* `tail` → Show last lines.
* `find` → Search for files.
* `locate` → Quickly locate files.
* `grep` → Search for text inside files.

## ❓ Interview Questions

1. Which command is used to view a file?
2. What is the difference between `cat` and `less`?
3. What does the `head` command do?
4. What does the `tail` command do?
5. Which command is used to search for files?
6. Which command searches for text inside files?
7. What is the difference between `find` and `grep`?

## 📚 References

* Linux Documentation
* GNU Coreutils Documentation
* Kali Linux Documentation
