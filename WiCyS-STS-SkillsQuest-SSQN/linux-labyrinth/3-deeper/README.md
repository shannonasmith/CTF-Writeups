<div align="center">

# 🕳 deeper

## Linux Directory Exploration & Nested Artifact Discovery

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Directory%20Exploration-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Filesystem%20Traversal-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux filesystem by navigating deeper into the directory structure to locate hidden artifacts.

The challenge required analysts to explore nested directories and identify files that were not visible from the top-level directory.

This exercise focused on **filesystem traversal and structured directory exploration**.

---

### 🖥 Environment

| Tool           | Purpose                  |
| -------------- | ------------------------ |
| Linux Terminal | Command-line interaction |
| `cd`           | Directory navigation     |
| `ls`           | Directory enumeration    |
| `cat`          | File inspection          |

---

### 📦 Step 1 — Begin Directory Navigation

After identifying directories in the environment, the investigation moved deeper into the filesystem to locate potential artifacts.

Command used:

```bash
cd directory_name
```

Navigating into subdirectories allows analysts to explore additional areas of the filesystem.

---

### 🔍 Step 2 — Enumerate Nested Directories

Once inside the directory, its contents were examined.

Command used:

```bash
ls
```

📸 **Nested Directory Enumeration**

<img src="../images/image057_redacted.png" width="600">

This revealed additional files located within the deeper directory structure.

---

### 🔄 Step 3 — Inspect File Contents

After identifying a relevant file, its contents were displayed using the `cat` command.

Command used:

```bash
cat filename
```

```
SSQ{[redacted]}
```

The file contained the information required to complete the investigation.

---

## 🧠 Methodology Framework Applied

```
Directory discovery
      ↓
Filesystem traversal
      ↓
Artifact identification
      ↓
File inspection
```

---

## 🛠 Techniques Used

Primary techniques used:

* directory traversal
* filesystem enumeration
* artifact inspection

Key concept investigated:

```
nested filesystem exploration
```

---

## 🛡 Defensive Insight

Attackers frequently explore directory structures after gaining system access to locate sensitive information or configuration files.

Organizations should implement proper file permissions and limit access to sensitive directories to reduce exposure.

---

## 💡 Skills Reinforced

* Linux directory traversal
* command-line investigation
* nested filesystem exploration
* artifact discovery

---

<div align="center">

🕳 Deeper exploration reveals hidden artifacts
🔎 Directory traversal exposes system structure
🧠 Investigation requires systematic exploration

</div>
