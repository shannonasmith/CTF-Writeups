<div align="center">

# 🧵 strings-n-things

## Binary Inspection & Metadata Discovery Investigation

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Binary%20Analysis-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-String%20Extraction-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux system artifact to identify hidden metadata and recover embedded information.

The challenge required inspecting system paths and analyzing files to uncover hidden data within a binary artifact.

This exercise focused on **string extraction and metadata discovery techniques** commonly used during forensic analysis.

---

### 🖥 Environment

| Tool           | Purpose                                |
| -------------- | -------------------------------------- |
| Linux Terminal | Command-line interaction               |
| `echo`         | Inspect environment variables          |
| `strings`      | Extract readable strings from binaries |
| `cat`          | Inspect file contents                  |

---

### 📦 Step 1 — Inspect System Environment

The investigation began by examining the system’s executable search path.

Command used:

```bash
echo $PATH
```

This command revealed the directories used by the system to locate executable programs.

---

### 🔍 Step 2 — Inspect Binary Contents

A suspicious file was analyzed using string extraction techniques.

Command used:

```bash
strings filename
```

📸 **String Extraction Analysis**

<img src="../images/image065_redacted.png" width="600">

The extracted strings revealed hidden metadata embedded within the artifact.

---

### 🔐 Step 3 — Recover Hidden Information

Within the extracted output, a string containing the hidden message was identified.

```
SSQ{[redacted]}
```

This confirmed that the artifact contained embedded information accessible through string analysis.

---

## 🧠 Methodology Framework Applied

```
Environment inspection
      ↓
Artifact identification
      ↓
String extraction
      ↓
Metadata discovery
```

---

## 🛠 Techniques Used

Primary techniques used:

* environment variable inspection
* binary string extraction
* metadata discovery

Key concept investigated:

```
binary artifact inspection
```

---

## 🛡 Defensive Insight

Sensitive information embedded within binaries can often be discovered using simple string extraction tools.

Organizations should avoid storing confidential information within compiled binaries or application metadata.

---

## 💡 Skills Reinforced

* binary inspection
* string extraction techniques
* Linux forensic investigation
* metadata discovery

---

<div align="center">

🧵 Strings reveal hidden data
🔍 Metadata often exposes secrets
🧠 Artifact inspection uncovers hidden information

</div>
