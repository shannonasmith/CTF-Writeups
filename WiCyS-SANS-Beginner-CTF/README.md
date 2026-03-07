<div align="center">

# 🏁 WiCyS / SANS Beginner-Level CTF  
## 🧠 Structured Security Investigation Portfolio

![Event](https://img.shields.io/badge/Event-WiCyS%20%2F%20SANS-6A0DAD?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-DFIR%20%7C%20Web%20Security%20%7C%20Artifact%20Analysis-blue?style=for-the-badge)
![Approach](https://img.shields.io/badge/Approach-Investigation%20First-success?style=for-the-badge)

</div>

---

## 🎯 Objective

This event marked the beginning of my structured CTF investigation documentation process.

Rather than focusing only on flag submission, this CTF was approached as a **hands-on security investigation exercise**.

The primary goals were to:

- 🔁 Develop repeatable investigation workflows  
- 🧭 Practice analytical pivoting when initial hypotheses fail  
- 🧾 Strengthen artifact and log interpretation skills  
- 🔍 Explore how attackers hide information within systems and files  
- 📚 Document investigative techniques for future reference  

All writeups focus on **methodology, reasoning, and investigation workflow**.

To respect competition integrity:

- ❌ Flags are not published  
- ❌ Protected answers are not disclosed  
- ✔ Only investigative techniques and analysis are documented

---

# 🛠 Technical Domains Practiced

| Domain | Focus Area |
|------|------|
| 🔐 Encoding Analysis | Data transformation & classification |
| 🌐 Web Security | Enumeration, source inspection, session manipulation |
| 📄 Artifact Forensics | Document redaction failures & metadata extraction |
| 🪟 Windows Log Analysis | Authentication tracking and event investigation |
| ⚡ PowerShell Investigation | Script block logging & attacker persistence |
| 📡 Network Investigation | Traffic analysis and artifact reconstruction |
| 🐍 Code Review | Static Python logic analysis |

---

# 🧩 Documented Challenges

---

## 🔐 Encoding & Data Transformation

### **Encoding, Not Encryption**  
🔎 [View Writeup](./encoding-not-encryption)

- Identified encoded data within a downloaded artifact  
- Tested multiple decoding strategies before identifying octal encoding  
- Demonstrated the importance of **correct classification before decoding**

---

## 🌐 Web Application Security

### **Hidden Web Content**  
🔎 [View Writeup](./hidden-web-content)

- Manual web application enumeration  
- Source code inspection revealed hidden content not visible in the UI  
- Demonstrated risks of storing sensitive information in client-side code

---

### **Arrays in JavaScript**  
🔎 [View Writeup](./arrays-in-javascript)

- JavaScript source analysis to understand client-side validation logic  
- Identified values stored within arrays controlling application behavior  
- Demonstrated weaknesses in **client-side security enforcement**

---

### **Get Admin**  
🔎 [View Writeup](./get-admin)

- Browser session and cookie inspection  
- Identified client-side role storage within session data  
- Privilege escalation achieved through **cookie manipulation**

---

## 🐍 Code Review

### **Race My Robot**  
🔎 [View Writeup](./race-my-robot)

- Static Python code inspection  
- Identified logic flaws affecting program behavior  
- Demonstrated the value of code review during security testing

---

## 📄 Digital Forensics & Artifact Analysis

### **Redacted Artifacts**  
🔎 [View Writeup](./redacted-artifacts)

- Investigated improperly redacted documents  
- Identified hidden information within layered artifacts  
- Demonstrated risks of **visual redaction without removing underlying data**

---

### **Hidden Diagram Metadata (.drawio)**  
🔎 [View Writeup](./hidden-diagram-data)

- Investigated a `.drawio.png` network diagram artifact  
- Identified embedded diagram metadata within the image file  
- Recovered hidden data by opening the file in **draw.io**

---

## 🪟 Windows Incident Investigation

### **Unwanted Visitor**  
🔎 [View Writeup](./unwanted-visitor)

- Investigated authentication activity using **Security.evtx logs**  
- Identified attacker workstation via **Event ID 4624 logon records**  
- Analyzed PowerShell activity through **Script Block Logging (Event ID 4104)**

---

### **Hidden Backdoor User (ROT13)**  
🔎 [View Writeup](./hidden-backdoor-user)

- Investigated PowerShell script block logs  
- Identified attacker persistence via scheduled task creation  
- Decoded ROT13-obfuscated username used to create a **hidden administrator account**

---

# 🧠 Key Takeaways

- Misclassification often signals incorrect problem framing rather than execution failure  
- Windows Event IDs provide valuable authentication forensic evidence  
- PowerShell Script Block Logging reveals attacker intent and persistence mechanisms  
- Client-side logic must never enforce authorization  
- File format research frequently reveals hidden metadata  
- Structured documentation significantly improves investigative clarity

---

<div align="center">

## 👤 Shannon Smith  
Cybersecurity | DFIR • Web Security • Threat Analysis  
U.S. Navy Veteran | Virginia Tech — M.S. Information Technology  

🛡️ Thinking like an analyst  
🔎 Documenting investigations  
📈 Building repeatable security workflows  

</div>
