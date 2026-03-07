<div align="center">

# 🔎 searching

## Linux File Discovery & Command-Line Search Investigation

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-File%20Discovery-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-System%20Search-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux environment to locate hidden information within the filesystem using command-line search techniques.

The challenge required identifying files that were not immediately visible through simple directory inspection.

This exercise focused on **systematic file discovery using Linux search utilities**, a common investigative step during system analysis and incident response.

---

### 🖥 Environment

| Tool           | Purpose                            |
| -------------- | ---------------------------------- |
| Linux Terminal | Command-line interaction           |
| `ls`           | Directory enumeration              |
| `find`         | Locate files across the filesystem |
| `cat`          | Inspect file contents              |

---

### 📦 Step 1 — Identify Available Files

The investigation began by inspecting the current directory to determine which files and folders were available for analysis.

Command used:

```bash
ls
```

This command provided an initial understanding of the filesystem layout.

---

### 🔍 Step 2 — Search the Filesystem

Because the relevant artifact was not immediately visible, a filesystem search was performed to locate files that might contain useful information.

Command used:

```bash
find . -type f
```

📸 **Filesystem Search Results**

<img src="../images/image056_redacted.png" width="600">

The search results revealed files located deeper within the directory structure that were not visible during initial enumeration.

---

### 🔄 Step 3 — Inspect Discovered File

After identifying the relevant file through the search results, its contents were examined.

Command used:

```bash
cat filename
```

The command displayed the contents of the file within the terminal.

```
SSQ{[redacted]}
```

This confirmed that the correct artifact had been located.

---

## 🧠 Methodology Framework Applied

```
Directory inspection
      ↓
Filesystem search
      ↓
Artifact discovery
      ↓
File inspection
```

---

## 🛠 Techniques Used

Primary techniques used:

* filesystem search using `find`
* Linux directory enumeration
* artifact inspection

Key concept investigated:

```
systematic file discovery
```

---

## 🛡 Defensive Insight

Attackers often rely on search utilities to quickly locate sensitive files after gaining system access.

Administrators should minimize the exposure of sensitive information within accessible directories and ensure that proper access controls restrict unauthorized users from browsing the filesystem.

---

## 💡 Skills Reinforced

* Linux search utilities
* filesystem discovery techniques
* command-line investigation
* artifact identification

---

<div align="center">

🔎 Searching reveals hidden artifacts
🧭 Systematic discovery improves investigations
🧠 Linux tools provide powerful investigative capabilities

</div>
