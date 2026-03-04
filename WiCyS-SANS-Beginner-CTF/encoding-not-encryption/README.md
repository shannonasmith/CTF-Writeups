<div align="center">

# 🔐 Encoding, Not Encryption  
## Data Classification & Transformation Analysis

![Category](https://img.shields.io/badge/Category-Encoding-yellow?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Artifact%20Classification-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Structured%20Pivot-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Download and analyze a provided artifact to determine the hidden value contained within it.

The challenge title emphasized **encoding rather than encryption**, signaling that the solution required identifying and reversing a data transformation — not breaking cryptography.

This was fundamentally a **classification problem**.

---

## 🖥 Environment

| Tool | Purpose |
|-----|------|
| Kali / Ubuntu Linux VM | Investigation environment |
| Terminal utilities (`wget`, `unzip`, `ls`) | Artifact acquisition and inspection |
| CyberChef | Data decoding and transformation |
| Encoding reference materials | Format identification |

---

## 📦 Step 1 — Acquire the Artifact

The challenge provided a downloadable ZIP archive containing the encoded artifact.

The file was retrieved via terminal:

```bash
wget https://2-files.bootupctf.net/ce01.zip
```

Example output:

```bash
--2024-XX-XX--  https://2-files.bootupctf.net/ce01.zip
Resolving 2-files.bootupctf.net...
Connecting...
Saving to: 'ce01.zip'

100%[==========================>] 1.2K
```

📸 **Artifact Download**

![Artifact Download](images/image01.png)

Successful retrieval confirmed that the artifact was intact and ready for inspection.

---

## 🔍 Step 2 — Extract & Inspect

The archive was extracted and the contents inspected.

```bash
unzip ce01.zip -d ce01
cd ce01
ls -l
```

Example directory output:

```bash
encoded.txt
```

📸 **Extracted File Structure**

![Extracted Files](images/image02.png)

Opening the file revealed a sequence of numeric values that were not immediately human-readable.

```bash
cat encoded.txt
```

Example data excerpt:

```
157 143 164 146 173 ...
```

📸 **Encoded Artifact**

![Encoded Data](images/image03.png)

Initial hypothesis:

The values likely represented **encoded ASCII text** rather than encrypted data.

---

## 🧪 Step 3 — Initial Classification Attempts

Common encoding formats were tested first.

### Base64

Attempted decoding via CyberChef.

Result: ❌ Invalid format.

### Hexadecimal

Hex decoding also failed to produce meaningful output.

### Binary

Binary decoding attempts did not match the numeric structure of the data.

---

### 🔎 Analytical Observation

Repeated decoding failures suggested:

- the decoding tools were functioning correctly  
- the **encoding classification was incorrect**

At this point the investigation pivoted toward **pattern analysis of the numeric values themselves**.

---

## 🔄 Step 4 — Strategic Pivot

Instead of continuing to retry common encoding methods, the investigation shifted toward identifying **numeric base patterns**.

Observation:

All numbers fell within the range typical for **octal representations**.

Example values:

```
157
143
164
```

These align with **ASCII octal encoding**, which represents characters using base-8 values.

Guiding principle:

> Persistent decoding failure often indicates incorrect encoding classification, not tool misuse.

---

## 🔢 Step 5 — Identify Octal Representation

The numeric values were interpreted as **octal ASCII codes**.

Using CyberChef:

```
From Octal → Text
```

📸 **CyberChef Transformation**

![CyberChef Decode](images/image04.png)

The decoded output produced readable text, confirming the correct encoding classification.

---

# 🧠 Methodology Framework Applied

```
Artifact acquisition
      ↓
Archive extraction
      ↓
Data inspection
      ↓
Common encoding testing
      ↓
Pattern recognition
      ↓
Octal classification
      ↓
Successful decoding
```

---

# 🛠 Commands Used

```bash
wget https://2-files.bootupctf.net/ce01.zip
unzip ce01.zip -d ce01
cd ce01
ls -l
cat encoded.txt
```

Primary analysis tool:

- **CyberChef** for octal-to-text conversion

---

# 🛡 Defensive Insight

Encoding misclassification is common in early-stage investigations.

This challenge reinforced several investigation principles:

- Encoding ≠ encryption  
- Data classification must precede transformation  
- Tool repetition without pivoting wastes time  
- Research-backed pivots accelerate resolution  

Recognizing numeric patterns and base representations can significantly reduce investigation time.

---

# 💡 Skills Reinforced

- Terminal-based artifact handling  
- Encoding pattern recognition  
- Analytical pivoting  
- Systematic troubleshooting  
- Data classification under ambiguity  
- CyberChef data transformation workflows  

---

<div align="center">

🔐 Classify before decoding  
🔄 Pivot when patterns fail  
🧠 Think in encoding families, not formats  

</div>
