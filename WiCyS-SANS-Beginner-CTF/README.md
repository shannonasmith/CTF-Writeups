
<div align="center">

# 🏁 WiCyS / SANS Beginner-Level CTF  
## 🧠 Structured Challenge Analysis & Methodology Portfolio

![Event](https://img.shields.io/badge/Event-WiCyS%20%2F%20SANS-6A0DAD?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-DFIR%20%7C%20Web%20%7C%20Logs-blue?style=for-the-badge)
![Documentation](https://img.shields.io/badge/Approach-Methodology%20First-success?style=for-the-badge)

</div>

---

## 🎯 Objective

This event marked the beginning of my formalized CTF documentation framework.

Rather than focusing solely on flag submission, this engagement emphasized:

- 🔁 Building repeatable investigative workflows  
- 🧭 Practicing disciplined analytical pivoting  
- 🧾 Strengthening log and artifact interpretation  
- ⏱ Improving structured documentation under time constraints  
- 📚 Identifying technical gaps for future deep-dive study  

All writeups focus strictly on **methodology, reasoning, and technique**.  
No flags or protected competition answers are included.

---

# 🛠 Technical Domains Covered

| Domain | Focus Area |
|--------|------------|
| 🔐 Encoding | Data transformation & classification |
| 🌐 Web Security | Enumeration & client-side trust analysis |
| 📄 Forensics | Document & image artifact recovery |
| 🪟 Windows Logs | Event ID 4624 & authentication tracking |
| ⚡ PowerShell | Script Block Logging & persistence |
| 📡 Network Analysis | PCAP & HTTP artifact inspection |
| 🐍 Code Review | Static Python logic auditing |

---

# 🧩 Completed Challenge Categories

---

## 🔐 Encoding & Data Transformation

### **ce01 — Encoding, Not Encryption**
- Classification of encoding type after failed initial decoding attempts  
- Pivot from common encodings to octal representation  
- Reinforced methodology: misclassification vs. execution failure  

---

## 🌐 Web Application Security

### **we01 — Hidden Web Content**
- Source inspection & enumeration mindset  
- Discovery of unlinked resources  
- Manual exploration informed by research  

### **wm01 — Arrays in JavaScript**
- Client-side logic inspection  
- Manipulation of front-end validation mechanisms  
- Demonstration of weak client-side trust model  

### **Get Admin**
- Session & cookie inspection  
- Client-side privilege escalation  
- Weak authorization model analysis  

### **race-my-robot**
- Static Python source review  
- Logic flaw identification  
- Controlled exploitation via code understanding  

---

## 📄 Digital Forensics & Artifact Recovery

### **Redacted 1 — ODT Document Analysis**
- Recovery of text not properly removed from document structure  

### **Redacted 2 — Image Transparency Analysis**
- Identification of concealed content via alpha channel behavior  

### **Redacted 3 — PDF Redaction Reversal**
- Removal of overlay-based redactions  
- Verification of underlying content persistence  

### **Redacted 4 — Embedded Diagram Metadata (.drawio.png)**
- Recognition of structured file format  
- Extraction of hidden diagram-layer content  

---

## 🪟 Windows Incident Investigation

### **Unwanted Visitor 1**
- Security.evtx analysis  
- Event ID 4624 logon validation  
- Host attribution from successful authentication events  

### **Unwanted Visitor 2**
- PowerShell Script Block Logging review  
- Detection of `Invoke-Expression (IEX)` usage  
- Scheduled task persistence mechanism identification  

### **Unwanted Visitor 3**
- Obfuscation analysis (ROT13)  
- Script block logic & comment inspection  
- Hidden account recovery methodology  

---

## 📡 Multi-Artifact Forensic Series — “New House”

Artifacts analyzed:

- 🪟 Windows event logs  
- 🐧 Linux indicators  
- 📡 Network packet capture (PCAP)  
- 📄 Supporting document artifacts  

Completed investigative areas:

- Windows group creation & membership analysis  
- Scheduled task removal & creation tracking  
- Linux OS identification  
- Tool download identification via HTTP traffic  
- Browser attribution via User-Agent analysis  

Selected questions were intentionally retained for structured follow-up research and timeline reconstruction practice.

---

# 🚧 Retained for Future Deep Dive

- Directory Traversal exploitation scenario  
- Advanced PCAP port state comparison  
- Additional artifact attribution questions  

Preserved to:

- 🔍 Revisit with stronger enumeration workflows  
- 🧪 Practice alternate traversal bypass techniques  
- 🗺 Perform structured PCAP timeline reconstruction  

---

# 🧠 Key Takeaways

- Misclassification often signals incorrect problem framing, not execution failure  
- Event ID interpretation is foundational in Windows investigations  
- Script Block Logging provides high-fidelity attacker intent  
- Client-side logic must never enforce authorization  
- File format research frequently reveals hidden metadata  
- Structured documentation improves analytical precision  

---

<div align="center">

## 👤 Shannon “Shae” Smith  
Cybersecurity | DFIR • Web • Detection Engineering  
U.S. Navy Veteran | Virginia Tech — M.S. Information Technology  

🛡️ Thinking like an analyst  
🔎 Documenting signal  
📈 Improving detection mindset  

</div>
