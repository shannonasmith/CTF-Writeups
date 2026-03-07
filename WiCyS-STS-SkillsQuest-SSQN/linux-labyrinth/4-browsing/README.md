<div align="center">

# 📂 browsing

## Linux File Inspection & Artifact Review

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Artifact%20Inspection-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-File%20Analysis-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux environment by reviewing files discovered during filesystem exploration.

The challenge required analysts to inspect files and analyze their contents to identify hidden information.

This exercise focused on **artifact inspection and file content analysis**.

---

### 🖥 Environment

| Tool           | Purpose                  |
| -------------- | ------------------------ |
| Linux Terminal | Command-line interaction |
| `ls`           | Directory enumeration    |
| `cat`          | File content inspection  |

---

### 📦 Step 1 — Review Available Files

The investigation began by examining the files available in the directory.

Command used:

```bash
ls
```

This provided visibility into files that could be inspected further.

---

### 🔍 Step 2 — Inspect File Contents

After identifying a potential artifact, its contents were examined.

Command used:

```bash
cat filename
```

📸 **Artifact Inspection**

<img src="../images/image058_redacted.png" width="600">

The command revealed the hidden information stored within the file.

```
SSQ{[redacted]}
```

---

## 🧠 Methodology Framework Applied

```
Directory enumeration
      ↓
Artifact discovery
      ↓
File inspection
      ↓
Information recovery
```

---

## 🛠 Techniques Used

Primary techniques used:

* file inspection
* command-line artifact analysis

Key concept investigated:

```
artifact analysis
```

---

## 🛡 Defensive Insight

Sensitive information stored in accessible files can be easily discovered by attackers using basic command-line tools.

Organizations should avoid storing sensitive data in publicly accessible directories and implement strict access control policies.

---

## 💡 Skills Reinforced

* artifact inspection
* Linux command-line investigation
* file content analysis

---

<div align="center">

📂 File inspection reveals hidden data
🔎 Artifact analysis uncovers system secrets
🧠 Investigation requires careful review

</div>
