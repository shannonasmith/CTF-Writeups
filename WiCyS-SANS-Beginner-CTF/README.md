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

# 🧩 Documented Challenges

---

## 🔐 Encoding & Data Transformation

### **ce01 — Encoding, Not Encryption**  
🔎 [View Writeup](./ce01-encoding-not-encryption)

- Classification of encoding type after failed initial decoding attempts  
- Pivot from common encodings to octal representation  
- Reinforced methodology: misclassification vs. execution failure  

---

## 🌐 Web Application Security

### **we01 — Hidden Web Content**  
🔎 [View Writeup](./we01-hidden-web-content)

- Source inspection & enumeration mindset  
- Discovery of unlinked resources  
- Manual exploration informed by research  

### **wm01 — Arrays in JavaScript**  
🔎 [View Writeup](./wm01-arrays-in-javascript)

- Client-side logic inspection  
- Manipulation of front-end validation mechanisms  
- Demonstration of weak client-side trust model  

### **we02 — Get Admin**  
🔎 [View Writeup](./we02-get-admin)

- Session & cookie inspection  
- Client-side privilege escalation  
- Weak authorization model analysis  

---

## 🐍 Code Review

### **cr01 — Race My Robot**  
🔎 [View Writeup](./cr01-race-my-robot)

- Static Python source review  
- Logic flaw identification  
- Controlled exploitation via code understanding  

---

## 📄 Digital Forensics & Artifact Recovery

### **df01 — Redacted Artifacts**  
🔎 [View Writeup](./df01-redacted-artifacts)

- Recovery of text not properly removed from document structure  
- Identification of concealed content in layered artifacts  
- Detection of improper redaction techniques across file formats  

---

## 🪟 Windows Incident Investigation

### **df02 — Unwanted Visitor**  
🔎 [View Writeup](./df02-unwanted-visitor)

- Security.evtx analysis  
- Event ID 4624 logon validation  
- Host attribution from successful authentication events  
- PowerShell Script Block Logging review  
- Detection of suspicious command execution & persistence  

---

## 📡 Multi-Artifact Forensic Series

### **df03 — New House Investigation**  
🔎 [View Writeup](./df03-new-house-investigation)

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
