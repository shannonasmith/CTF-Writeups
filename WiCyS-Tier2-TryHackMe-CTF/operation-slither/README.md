<div align="center">

# 🐍 Operation Slither 1  
## Linux Command-Line Investigation & Hidden File Discovery

![Category](https://img.shields.io/badge/Category-Linux-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-File%20Discovery-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Command%20Line%20Investigation-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux system to locate hidden information within the filesystem.

The challenge required using Linux command-line tools to search for files and identify data that had been intentionally hidden.

The objective was to perform **filesystem reconnaissance** and recover the hidden information.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Kali Linux AttackBox | Investigation environment |
| Linux terminal | Command execution |
| `ls` | Directory inspection |
| `find` | File discovery |
| `cat` | File content inspection |

---

### 📦 Step 1 — Begin Filesystem Investigation

The investigation began by examining the working directory to determine what files were present.

```bash
ls
```

Initial inspection showed a minimal set of visible files.

Because challenges like this often hide information in unexpected locations, deeper exploration of the filesystem was required.

---

### 🔍 Step 2 — Search for Hidden Files

Hidden files in Linux typically begin with a dot (`.`) and may not appear in standard directory listings.

To reveal hidden files, the following command was used:

```bash
ls -la
```

This command displays all files, including hidden entries and directory metadata.

However, further investigation suggested that the target file might be located deeper within the filesystem.

---

### 🧪 Step 3 — Locate the Target File

To search for files across the system, the `find` command was used.

```bash
find / -type f 2>/dev/null
```

This command recursively searches the filesystem for files while suppressing permission errors.

📸 **Filesystem Search Results**

<img src="../images/image047.png" width="600">

The search results revealed a file of interest that appeared to contain the hidden information.

---

#### 🔎 Analytical Observation

Linux systems provide powerful command-line utilities that allow investigators to search large filesystems efficiently.

Commands such as `find`, `grep`, and `ls` are frequently used in forensic investigations to locate hidden or suspicious files.

These tools allow analysts to quickly identify artifacts that may otherwise remain unnoticed.

---

### 🔄 Step 4 — Inspect the File Contents

After identifying the suspicious file, the next step was to inspect its contents.

```bash
cat filename
```

This command prints the contents of the file directly to the terminal, allowing investigators to determine whether it contains relevant information.

---

### 🔐 Step 5 — Confirm Successful Recovery

Opening the discovered file revealed the information required to complete the challenge.

📸 **Recovered Hidden Data**

<img src="../images/image048_redacted.png" width="600">

This confirmed that the hidden information had been successfully located through command-line filesystem investigation.

---

## 🧠 Methodology Framework Applied

```
Filesystem inspected
      ↓
Hidden files revealed
      ↓
Recursive file search performed
      ↓
Suspicious file identified
      ↓
File contents inspected
      ↓
Hidden information recovered
```

---

## 🛠 Techniques Used

Primary techniques used:

- filesystem reconnaissance  
- hidden file discovery  
- recursive file search  
- command-line file inspection  

Key concept investigated:

```
Linux filesystem investigation
```

---

## 🛡 Defensive Insight

Attackers and administrators alike may hide files within a system’s filesystem.

Linux provides powerful command-line tools that can uncover hidden files and artifacts.

Security teams should regularly audit systems using tools that can:

- identify hidden files  
- locate suspicious artifacts  
- monitor unauthorized filesystem changes  

Routine filesystem monitoring can help detect unauthorized activity.

---

## 💡 Skills Reinforced

- Linux command-line investigation  
- Filesystem enumeration  
- Hidden file discovery  
- Command-line forensic analysis  

---

<div align="center">

🐍 Hidden files often contain valuable clues  
🔍 Linux command-line tools enable deep system inspection  
🧠 Filesystem analysis is essential for forensic investigations  

</div>
