<div align="center">

# 🧠 CTF Writeups — Cybersecurity Investigation Portfolio

Hands-on cybersecurity investigations across **web exploitation, DFIR, cryptography, network analysis, threat hunting, and system forensics**.

<br>

<img src="https://img.icons8.com/color/96/anonymous-mask.png" width="60"/>
<img src="https://img.icons8.com/color/96/network.png" width="60"/>
<img src="https://img.icons8.com/color/96/lock.png" width="60"/>
<img src="https://img.icons8.com/color/96/cyber-security.png" width="60"/>

<br><br>

![CTFs](https://img.shields.io/badge/CTFs_Documented-3-purple?style=for-the-badge)
![Challenges](https://img.shields.io/badge/Challenges_Investigated-50+-blue?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Security%20Investigation-success?style=for-the-badge)

</div>

---

# 🎯 Purpose

This repository documents structured investigations from multiple **Capture-the-Flag (CTF) competitions** completed through the **WiCyS Security Training Scholarship program**.

🔗 https://www.wicys.org/benefits/security-training-scholarship/

Rather than publishing challenge answers, this repository focuses on documenting the **investigation methodology used to solve security problems.**

Each writeup demonstrates:

• investigative reasoning
• hypothesis testing
• artifact and system analysis
• structured problem solving
• repeatable investigation workflows

The goal is to show **how a security analyst approaches an unknown problem**, not just the final solution.

---

# 🔍 Investigation Approach

Each challenge in this repository was approached as a **security investigation rather than a puzzle.**

The workflow used across the writeups follows a repeatable analytical process similar to those used by **security analysts, incident responders, and threat hunters**.

### Investigation Workflow

<div align="center">

```
🔎 Initial Observation
↓
🧭 Environment Exploration
↓
💡 Hypothesis Development
↓
🛠 Tool-Based Investigation
↓
📂 Artifact Analysis
↓
🔁 Iterative Testing
↓
✅ Evidence Confirmation
```

</div>

Rather than jumping directly to a solution, the investigation process emphasizes:

• understanding system behavior
• identifying anomalies
• validating hypotheses with evidence
• documenting investigative steps

This mirrors how analysts investigate **real-world security incidents**, where answers must be uncovered through structured analysis.

---

# 🧠 Analyst Skillsets Demonstrated

Across the documented competitions, this portfolio demonstrates **three complementary cybersecurity analyst roles.**

| Competition                  | Analyst Role                         | Focus                                                      |
| ---------------------------- | ------------------------------------ | ---------------------------------------------------------- |
| WiCyS / SANS Beginner CTF    | **SOC / DFIR Analyst**               | artifact analysis, Windows logs, event correlation         |
| WiCyS Tier 2 TryHackMe CTF   | **Security Testing & Exploitation**  | web vulnerabilities, command injection, enumeration        |
| WiCyS STS Tier 2 SkillsQuest | **Threat Investigation & Detection** | SIEM analysis, persistence detection, binary investigation |

Together these investigations demonstrate the ability to:

• investigate attacker behavior across systems
• analyze artifacts and logs to reconstruct attack timelines
• identify persistence mechanisms and escalation paths
• document investigation methodology for repeatable workflows

---

# 🧩 CTFs Documented

| Competition                                                        | Description                                                |
| ------------------------------------------------------------------ | ---------------------------------------------------------- |
| 🏁 **[WiCyS / SANS Beginner CTF](WiCyS-SANS-Beginner-CTF)**        | First structured CTF investigation and documentation       |
| 🧠 **[WiCyS Tier 2 TryHackMe CTF](WiCyS-Tier2-TryHackMe-CTF)**     | Web exploitation, cryptography, OSINT, and enumeration     |
| 🛰 **[WiCyS STS Tier 2 SkillsQuest](WiCyS-STS-Tier2-SkillsQuest)** | Threat investigation, SIEM analysis, persistence detection |
| 🌐 **[WiCyS NCL CyberSkyline 2026](WiCyS-NCL-CyberSkyline-2026)**  | Upcoming competition (documentation in progress)           |

Each competition includes:

• event overview README
• individual challenge folders
• structured investigation writeups
• supporting screenshots and artifacts

---

## 📊 Security Skills Practiced

These categories represent **hands-on investigations documented across 50+ CTF challenges in this repository.**

| Domain                          | Investigation Exposure  |
| ------------------------------- | ----------------------- |
| 🌐 **Web Exploitation**         | ███████ (18 challenges) |
| 🔎 **DFIR / Artifact Analysis** | ██████ (15 challenges)  |
| 🔐 **Cryptography**             | █████ (11 challenges)   |
| 📡 **Network Analysis**         | ████ (9 challenges)     |
| 🕵️ **OSINT**                   | ███ (5 challenges)      |
| 🐧 **Linux Investigation**      | ███ (6 challenges)      |
| 🧬 **Reverse Engineering**      | ██ (3 challenges)       |

These counts represent **practical investigation experience**, not proficiency ratings.

---

# 🛠 Tools & Technologies Used

Across the documented investigations, the following tools and technologies were used.

---

## 🔧 Investigation Tool Stack

<div align="center">

![Kali](https://img.shields.io/badge/Kali_Linux-Operating_System-black?style=flat-square\&logo=kalilinux)
![Ubuntu](https://img.shields.io/badge/Ubuntu-Linux-E95420?style=flat-square\&logo=ubuntu)
![Windows](https://img.shields.io/badge/Windows-Environment-0078D6?style=flat-square\&logo=windows)

![Wireshark](https://img.shields.io/badge/Wireshark-PCAP_Analysis-1679A7?style=flat-square\&logo=wireshark)
![Nmap](https://img.shields.io/badge/Nmap-Network_Scanner-blue?style=flat-square)
![CyberChef](https://img.shields.io/badge/CyberChef-Data_Transformation-orange?style=flat-square)

![ELK](https://img.shields.io/badge/ELK-Log_Analysis-yellow?style=flat-square\&logo=elastic)
![Python](https://img.shields.io/badge/Python-Scripting-3776AB?style=flat-square\&logo=python)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat-square\&logo=powershell)

</div>

---

## 🌐 Network & Enumeration

* nmap
* netcat
* curl
* tcpdump
* Wireshark

---

## 🔎 Web Security Investigation

* Browser Developer Tools
* HTTP request inspection
* session cookie analysis
* client-side JavaScript inspection
* command injection testing

---

## 🔐 Cryptography & Encoding

* CyberChef
* hash analysis
* base encoding analysis
* hex decoding

---

## 🐧 Linux Investigation & Terminal Analysis

Common commands used during investigations:

```bash
find • grep • cat • less • strings • chmod • ps • lsof • tar • gzip
gunzip • unzip • xz • dd • file • xxd • wget • curl • mv • cp • ls

```

Investigation techniques included:

• file system enumeration
• metadata inspection
• archive extraction
• binary interaction

---

## 🪟 Windows Investigation

PowerShell investigation commands:

```powershell
Get-Service
Get-Process
Get-ItemProperty
Get-NetTCPConnection
Get-ChildItem
```

Additional analysis included:

• Windows event log investigation
• registry inspection
• service enumeration

---

## 📊 SIEM & Log Analysis

* ELK Stack (Elasticsearch / Logstash / Kibana)
* event log correlation
* log filtering and query analysis
* timeline reconstruction
* threat hunting queries

---

## 🧬 Malware & Binary Investigation

* process inspection
* binary interaction
* memory artifact extraction
* network connection monitoring

---

# 🛰 MITRE ATT&CK Techniques Practiced

| Technique | Description                         |
| --------- | ----------------------------------- |
| T1595     | Active Scanning                     |
| T1583     | Acquire Infrastructure              |
| T1078     | Valid Accounts                      |
| T1059     | Command & Scripting Interpreter     |
| T1053     | Scheduled Task Persistence          |
| T1110     | Brute Force                         |
| T1046     | Network Service Discovery           |
| T1040     | Network Sniffing                    |
| T1041     | Exfiltration Over Command & Control |

---

# 🔒 Flag & Content Policy

To respect competition rules and maintain integrity:

❌ Flags are not published
❌ Protected answers are not disclosed
❌ Copyrighted materials are not redistributed

Writeups focus strictly on **analysis, investigation methodology, and technical reasoning.**

---

# 📚 Continuing Development

Additional cybersecurity investigations and competitions will continue to be documented in this repository as part of ongoing professional development.

Future areas of focus include:

• threat hunting investigations
• detection engineering
• adversary emulation
• malware analysis

---

<div align="center">

## 👤 Shannon Smith

Cybersecurity | DFIR • Threat Investigation • Security Analysis

U.S. Navy Veteran
Virginia Tech — M.S. Information Technology

GIAC **GFACT** | CEH | Security+ | Linux+ | Splunk CCPU

🛡 Thinking like an analyst
🔎 Documenting investigations
📈 Building repeatable security workflows

</div>
