<div align="center">

# 🕵️ Redacted Artifacts  
## Document Forensics & Improper Redaction Analysis

![Category](https://img.shields.io/badge/Category-Digital%20Forensics-darkred?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Document%20Analysis-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Artifact%20Inspection-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Analyze a set of documents that appear to have sensitive information removed through redaction.

The challenge title suggested that the redactions may have been applied incorrectly, meaning the hidden information might still exist within the file structure.

This challenge focused on **digital artifact inspection and improper redaction discovery**.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Kali / Ubuntu Linux VM | Investigation environment |
| Document viewers | File inspection |
| Manual artifact inspection | Identifying hidden document structure |
| Text selection testing | Determining whether underlying data remained |

---

### 📦 Step 1 — Obtain the Artifacts

The challenge provided several documents containing redacted sections.

At first glance, the files displayed blacked-out text intended to conceal sensitive information.

Initial hypothesis:

The redactions may have been applied **visually rather than structurally**, meaning the original data could still exist within the file.

---

### 🔍 Step 2 — Inspect the Redacted Documents

Each document was opened and inspected visually.

📸 **Redacted Document Example**

<img src="../images/image26.png" width="800">

The redacted sections appeared as black rectangles covering text.

However, visual redactions do not always remove the underlying content.

---

### 🧪 Step 3 — Examine Additional Redacted Artifacts

Multiple documents were provided, each showing similar redaction behavior.

📸 **Additional Redacted Document**

<img src="../images/image27.png" width="800">

The consistent redaction style suggested that the same method had been used across multiple files.

This increased the likelihood that the redaction process had been applied incorrectly.

---

### 🔄 Step 4 — Analyze Redaction Technique

Improper redaction often occurs when:

- black shapes are placed over text
- the original text layer remains underneath
- the document is exported without removing the underlying data

📸 **Redacted Artifact Structure**

<img src="../images/image28.png" width="800">

This indicated that the sensitive content may still exist in the document structure despite being visually hidden.

---

### 🔐 Step 5 — Identify Improper Redaction

Through artifact inspection and testing, it became clear that the redactions had not permanently removed the sensitive information.

Instead, the redacted areas were likely implemented as **visual overlays**, meaning the underlying content could potentially be recovered through further analysis.

---

## 🧠 Methodology Framework Applied

```
Artifact acquisition
      ↓
Visual document inspection
      ↓
Redaction pattern analysis
      ↓
Overlay identification
      ↓
Improper redaction discovery
```

---

## 🛠 Techniques Used

Primary techniques used:

- document artifact inspection
- visual redaction analysis
- layered document behavior analysis
- information disclosure investigation

Key concept investigated:

```
Improper document redaction
```

---

## 🛡 Defensive Insight

Improper redaction is a common data protection failure.

Simply covering text with shapes or black boxes does not remove the original content from the document.

If the text layer remains intact, attackers may recover the hidden information.

Proper redaction requires:

- permanently removing sensitive text
- flattening document layers
- verifying that underlying content cannot be extracted

Organizations that rely on visual redaction alone risk exposing sensitive information.

---

## 💡 Skills Reinforced

- Digital artifact inspection  
- Document structure analysis  
- Redaction bypass investigation  
- Information disclosure analysis  
- Secure document handling awareness  

---

<div align="center">

🕵️ Visual redaction does not remove data  
🔍 Inspect artifacts beyond the visible layer  
🧠 Hidden information often remains recoverable  

</div>
