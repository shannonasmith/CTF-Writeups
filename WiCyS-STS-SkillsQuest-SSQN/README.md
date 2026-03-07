<div align="center">

# 🛰 WiCyS STS Tier 2 — SkillsQuest CTF
## Threat Investigation, System Analysis & MITRE ATT&CK Mapping

![Event](https://img.shields.io/badge/Event-WiCyS%20STS%20Tier%202-purple?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Threat%20Investigation-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

The **WiCyS Security Training Scholarship (STS) Tier 2 SkillsQuest CTF** focused on developing practical skills in **system investigation, threat analysis, and incident response techniques**.

Participants analyzed multiple simulated environments including:

- Linux systems
- Windows hosts
- enterprise log environments
- running malware processes

Rather than isolated puzzles, the competition emphasized **realistic investigative workflows** similar to those used by security analysts and threat hunters.

The challenges required identifying attacker activity, investigating suspicious artifacts, and understanding how attacks progress across systems.

---

## 🧠 Skills Practiced

| Skill | Description |
|------|------|
| System Investigation | Investigating Linux and Windows hosts for suspicious activity |
| Threat Hunting | Searching logs and system artifacts for indicators of compromise |
| SIEM Analysis | Investigating attack activity through ELK log analysis |
| Persistence Detection | Identifying attacker footholds within operating systems |
| Binary & Process Analysis | Investigating suspicious processes and malware behavior |
| Privilege Escalation Analysis | Understanding system misconfigurations enabling escalation |
| MITRE ATT&CK Mapping | Relating attacker actions to known adversary techniques |

---

## 🧩 Challenge Environments

The SkillsQuest competition included several investigative environments.

### 🐧 Linux Labyrinth

Focused on **Linux command-line investigation and system enumeration**.

Skills practiced:

- file system navigation
- command-line searching
- HTTP interaction from the terminal
- process and service inspection
- metadata extraction

---

### 🪟 Windows Basics

Focused on **Windows host investigation using PowerShell and system utilities**.

Skills practiced:

- service inspection
- registry analysis
- user directory investigation
- process enumeration
- network port discovery

---

### 📊 ELK SIEM Log Analysis

Simulated a **network intrusion investigation** using the ELK stack.

Participants analyzed logs to:

- identify phishing activity
- trace attacker behavior across hosts
- investigate process creation events
- identify persistence and lateral movement
- reconstruct an attack timeline

---

### 🧩 Windows Persistence

Focused on identifying **multiple persistence mechanisms used by malware**.

Investigated techniques included:

- registry run keys
- scheduled tasks
- Windows services
- startup folder execution
- WMI persistence

---

### 🧬 Linux Binary Analysis

Focused on analyzing a **suspicious binary running on a Linux system**.

Skills practiced:

- process enumeration
- memory artifact extraction
- binary interaction
- network connection monitoring
- malware behavior investigation

---

### 🧠 Privilege Escalation & Lateral Movement

A multi-user Linux environment simulating **privilege escalation and lateral movement scenarios**.

Skills practiced:

- credential discovery
- command injection exploitation
- file permission analysis
- environment manipulation
- user account pivoting

---

## 🧭 Attack Lifecycle Analysis

Across the challenges, investigations followed common phases of a cyber intrusion lifecycle:

| Phase | Example Techniques |
|------|------|
| Reconnaissance | system enumeration |
| Initial Access | phishing and credential discovery |
| Execution | command interpreter activity |
| Persistence | scheduled tasks and service manipulation |
| Privilege Escalation | abuse of system permissions |
| Discovery | host and network enumeration |
| Lateral Movement | account pivoting across systems |
| Command & Control | network connections from malware |
| Exfiltration | attacker data transfer |

---

## 🛠 Tools & Techniques Used

<img src="https://img.icons8.com/color/48/linux.png" width="25"/> Linux command line  
<img src="https://img.icons8.com/color/48/windows-10.png" width="25"/> Windows PowerShell  
<img src="https://img.icons8.com/color/48/network.png" width="25"/> network investigation  
<img src="https://img.icons8.com/color/48/database.png" width="25"/> ELK SIEM log analysis  

Additional investigative techniques included:

- event log investigation
- system artifact analysis
- process inspection
- network connection monitoring
- privilege escalation analysis

---

## 🧠 MITRE ATT&CK Techniques Observed

| Technique | Description |
|------|------|
| T1595 | Active Scanning |
| T1583 | Acquire Infrastructure |
| T1078 | Valid Accounts |
| T1059 | Command and Scripting Interpreter |
| T1053 | Scheduled Task |
| T1110 | Brute Force |
| T1046 | Network Service Discovery |
| T1040 | Network Sniffing |
| T1041 | Exfiltration Over Command & Control |

---

## 💡 Key Lessons Learned

- System artifacts provide valuable insight into attacker activity  
- Log correlation enables reconstruction of complex intrusion timelines  
- Persistence mechanisms often hide within legitimate system components  
- Binary processes can reveal forensic artifacts even after deletion  
- Threat investigations require both technical analysis and behavioral reasoning  

---

<div align="center">

🛰 Investigating attacker behavior  
🧠 Mapping adversary techniques  
🛡 Strengthening defensive analysis

</div>
