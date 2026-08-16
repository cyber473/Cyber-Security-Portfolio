# 📂 File System Navigation

## 📌 Overview

File System Navigation means **moving between directories, checking the current location, and listing files and directories** in Linux.

## 🎯 What is it?

Linux provides commands such as `pwd`, `ls`, and `cd` to navigate through the file system from the terminal.

## ❓ Why is it Needed?

File System Navigation helps to:

* Locate files and directories.
* Move between different directories.
* Understand the current file system location.
* Work efficiently from the command line.
* Perform enumeration during security testing.

## ⚙️ How Does it Work?

Linux uses paths to identify the location of files and directories.

Example:

```text id="u7i9q1"
/home/kali/Documents
```

* `/` → Root directory
* `home` → Directory
* `kali` → User directory
* `Documents` → Current directory

## 🏠 Real Life Example

Think of the file system like a **building**:

* `pwd` → Where am I?
* `ls` → What is here?
* `cd` → Move to another room.
* `cd ..` → Go one level back.

## 🛠 Practical Demo

```bash id="7s1m8v"
# Show current directory
pwd

# List files and directories
ls

# Show hidden files
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

| Command  | Purpose                                    |
| -------- | ------------------------------------------ |
| `pwd`    | Show current directory                     |
| `ls`     | List files/directories                     |
| `ls -la` | List detailed files including hidden files |
| `cd`     | Change directory                           |
| `cd ..`  | Go to parent directory                     |
| `cd ~`   | Go to home directory                       |
| `cd /`   | Go to root directory                       |
| `cd -`   | Go to previous directory                   |

## 🔐 VAPT Perspective

File System Navigation is useful for:

* Directory Enumeration
* Sensitive File Discovery
* Configuration File Discovery
* Log Analysis
* Privilege Escalation
* Server Enumeration

## 💡 Key Points

* `pwd` → Shows where you are.
* `ls` → Shows what is inside a directory.
* `cd` → Changes directory.
* `cd ..` → Moves to the parent directory.
* `cd ~` → Goes to the user's home directory.
* `cd /` → Goes to the root directory.
* `ls -la` → Shows hidden files.

## ❓ Interview Questions

1. What is File System Navigation?
2. Which command shows the current directory?
3. Which command is used to change directories?
4. What does `cd ..` do?
5. What does `cd ~` do?
6. How do you view hidden files in Linux?
7. What is the difference between `cd /` and `cd ~`?

## 📚 References

* Linux Documentation
* GNU Coreutils Documentation
* Kali Linux Documentation
