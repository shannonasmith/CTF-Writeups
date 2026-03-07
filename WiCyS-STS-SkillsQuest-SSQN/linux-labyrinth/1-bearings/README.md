<div align="center">

# 🧭 bearings

## Linux Environment Enumeration & System Orientation

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-System%20Enumeration-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Command%20Line%20Discovery-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux environment to determine the system structure and identify artifacts that may contain useful information.

The challenge required using basic Linux command-line tools to explore the filesystem and locate information hidden within the environment.

This exercise focused on **initial system orientation and filesystem enumeration**, which are foundational techniques used during Linux investigations and post-compromise analysis.

---

### 🖥 Environment

| Tool           | Purpose                      |
| -------------- | ---------------------------- |
| Linux Terminal | Command-line interaction     |
| `pwd`          | Determine working directory  |
| `ls`           | Enumerate directory contents |
| `cat`          | Inspect file contents        |

---

### 📦 Step 1 — Identify Current Location

The investigation began by determining the current working directory and identifying the files available within the environment.

Commands used:

```bash
pwd
ls
```

Understanding the working directory helps analysts orient themselves within the system before beginning deeper investigation.

---

### 🔍 Step 2 — Enumerate Files in the Directory

Once the environment was identified, the contents of the directory were examined to determine whether any files contained useful information.

Command used:

```bash
ls
```

📸 **Filesystem Enumeration**

<img src="../images/image055_redacted.png" width="600">

The directory listing revealed files present within the environment that could potentially contain hidden data.

---

### 🔄 Step 3 — Inspect File Contents

After identifying a relevant file, the next step was to inspect its contents directly.

Command used:

```bash
cat filename
```

Displaying the file contents allowed the hidden information to be observed within the terminal output.

```
SSQ{[redacted]}
```

This confirmed that the file contained the information required to complete the investigation.

---

## 🧠 Methodology Framework Applied

```
Environment orientation
      ↓
Directory enumeration
      ↓
File discovery
      ↓
Artifact inspection
```

---

## 🛠 Techniques Used

Primary techniques used:

* Linux filesystem enumeration
* Command-line environment inspection
* Artifact discovery through file analysis

Key concept investigated:

```
Linux system orientation
```

---

## 🛡 Defensive Insight

System enumeration is often one of the first steps performed after gaining access to a Linux system.

Attackers may inspect directory structures and file contents to locate sensitive information, credentials, or configuration files that could enable further compromise.

Organizations should implement proper access controls and avoid storing sensitive information in locations accessible to unauthorized users.

---

## 💡 Skills Reinforced

* Linux filesystem navigation
* Command-line enumeration techniques
* Artifact discovery
* System orientation during investigations

---

<div align="center">

🧭 Understanding system structure is the first step of investigation
🔎 Enumeration reveals hidden artifacts
🧠 Structured exploration leads to discovery

</div>
