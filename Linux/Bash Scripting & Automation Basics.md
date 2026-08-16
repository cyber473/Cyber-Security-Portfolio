# 🐚 Bash Scripting & Automation Basics

## 📌 Overview

Bash Scripting is used to **automate repetitive tasks** in Linux by writing multiple commands in a script file.

## 🎯 What is it?

**Bash** is a command-line shell commonly used in Linux.

A Bash script is a file containing commands that are executed in sequence.

Example:

```bash id="5v7q2m"
#!/bin/bash
echo "Hello, Cyber Security"
```

## ❓ Why is it Needed?

Bash scripting helps to:

* Automate repetitive tasks.
* Run multiple commands quickly.
* Automate system administration.
* Automate security and enumeration tasks.
* Save time and reduce manual work.

## ⚙️ How Does it Work?

Basic workflow:

```text id="5pj1lc"
Write Script
     ↓
Give Execute Permission
     ↓
Run Script
     ↓
Commands Execute Automatically
```

Example:

```bash id="9b6n2k"
#!/bin/bash

echo "System Information"
uname -a

echo "Current User"
whoami

echo "IP Address"
ip addr
```

## 🏠 Real Life Example

Think of Bash scripting like creating a **shortcut**.

Instead of performing 5 tasks manually, you write them once in a script and run the script whenever needed.

## 🛠 Practical Demo

### Create a Script

```bash id="9c7x1m"
nano info.sh
```

Add:

```bash id="z5p4k2"
#!/bin/bash
echo "Current User:"
whoami

echo "Hostname:"
hostname

echo "IP Address:"
ip addr
```

### Make it Executable

```bash id="f3s8n1"
chmod +x info.sh
```

### Run the Script

```bash id="p6w2r9"
./info.sh
```

## 💻 Important Bash Concepts

| Concept        | Example           |
| -------------- | ----------------- |
| Shebang        | `#!/bin/bash`     |
| Variable       | `name="Golu"`     |
| Output         | `echo "Hello"`    |
| Input          | `read name`       |
| Condition      | `if ... then`     |
| Loop           | `for ... do`      |
| Function       | `function_name()` |
| Execute Script | `./script.sh`     |

## 🔐 VAPT Perspective

Bash scripting is useful for:

* Reconnaissance Automation
* Host Enumeration
* Network Information Gathering
* Log Analysis
* Security Testing
* Repetitive VAPT Tasks
* Automating Security Scripts

Example:

```bash id="m4k8z2"
#!/bin/bash

echo "Hostname:"
hostname

echo "IP Address:"
ip addr

echo "Open Connections:"
ss -tuln
```

Use automation only on **authorized systems and labs**.

## 💡 Key Points

* Bash scripts contain Linux commands.
* `#!/bin/bash` defines the Bash interpreter.
* `chmod +x` gives execute permission.
* `./script.sh` runs a script.
* Variables store values.
* Conditions make decisions.
* Loops repeat tasks.
* Automation saves time and reduces manual work.

## ❓ Interview Questions

1. What is Bash?
2. What is Bash scripting?
3. What is the purpose of `#!/bin/bash`?
4. How do you make a Bash script executable?
5. How do you run a Bash script?
6. What is a variable in Bash?
7. What are loops used for?
8. How is Bash scripting useful in cybersecurity?

## 📚 References

* GNU Bash Documentation
* Linux Documentation
* Kali Linux Documentation
