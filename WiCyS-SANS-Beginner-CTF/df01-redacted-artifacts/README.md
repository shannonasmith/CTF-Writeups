<div align="center">

# 🕵️ df01 — Redacted Artifacts  
## Document & Media Forensics Analysis

![Category](https://img.shields.io/badge/Category-Digital%20Forensics-darkred?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Artifact%20Inspection-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Metadata%20%26%20Content%20Recovery-orange?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze several files that appeared to have sensitive information removed through redaction.

The goal was to determine whether the redactions were properly implemented or if the underlying data could still be recovered through artifact inspection.

This challenge focused on identifying **improper redaction techniques** and recovering hidden information from various document and media formats.

---

## 🖥 Environment

- Document viewers  
- Text extraction tools  
- File inspection utilities  
- Image viewers with transparency support  

---

## 🔎 Step 1 — Initial Artifact Inspection

Each file appeared to contain content that had been visually redacted.

Common formats included:

- Office documents  
- PDFs  
- image-based artifacts  
- diagram exports  

Initial inspection confirmed that the files were accessible and could be opened normally.

The key investigative question became:

> Was the sensitive data actually removed, or simply hidden visually?

---

## 🔍 Step 2 — Evaluate Redaction Technique

In many real-world scenarios, redaction is performed incorrectly.

Common mistakes include:

- covering text with black rectangles  
- layering shapes over content  
- hiding elements in document layers  
- leaving metadata intact  

These methods often **conceal information visually without removing it from the underlying file structure**.

The artifacts were examined with this possibility in mind.

---

## 🧪 Step 3 — Inspect Document Structure

Files were inspected to determine how the redactions were applied.

Investigation methods included:

- highlighting and copying text  
- selecting layered elements  
- reviewing embedded object structures  
- inspecting diagram or document metadata  

This revealed that in several cases, the redactions were only **visual overlays rather than true content removal**.

---

## 🔄 Step 4 — Recover Underlying Information

Because the original content was still embedded in the files, it was possible to reveal the hidden information by interacting with the document elements.

Examples of recoverable data included:

- text hidden beneath shapes  
- elements embedded within layered images  
- content preserved within diagram metadata  
- text recoverable through selection and copying  

This confirmed that the redaction techniques used were ineffective.

---

## 🧠 Methodology Framework Applied

1. Acquire artifacts  
2. Inspect file types  
3. Identify visual redaction techniques  
4. Examine document structure  
5. Test text selection and metadata inspection  
6. Recover underlying content  
7. Validate artifact integrity  

---

## 🛡 Defensive Insight

Improper redaction is a common operational security failure.

Simply hiding information visually does **not** remove it from a document.

Secure redaction requires:

- removing underlying text objects  
- flattening document layers  
- sanitizing metadata  
- exporting sanitized versions of files  

Failure to properly redact sensitive data can result in unintended information disclosure.

---

## 💡 Skills Reinforced

- Document artifact inspection  
- Understanding layered document structures  
- Metadata awareness  
- Digital evidence recovery techniques  
- Evaluating redaction security practices  

---

<div align="center">

🔎 Inspect the artifact  
🧠 Understand the file structure  
🛡 Visual redaction is not secure  

</div>
