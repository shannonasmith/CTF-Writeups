<div align="center">

# 🛰 WiCyS STS Tier 2 — SkillsQuest CTF
## Threat Actor Investigation & MITRE ATT&CK Analysis

![Event](https://img.shields.io/badge/Event-WiCyS%20STS%20Tier%202-purple?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Threat%20Hunting-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

The **SkillsQuest CTF** focused on analyzing attacker behavior through a threat-intelligence scenario.

Participants were tasked with identifying attacker techniques, understanding adversary behavior patterns, and mapping activity to the **MITRE ATT&CK framework**.

The exercise simulated real-world incident investigation where defenders must determine:

- attacker objectives
- tactics used
- infrastructure leveraged
- methods of persistence and exfiltration

Rather than isolated puzzles, this competition emphasized **holistic threat analysis**.

---

## 🧠 Skills Practiced

| Skill | Description |
|------|------|
| Threat Actor Profiling | Identifying adversary groups based on behavioral patterns |
| MITRE ATT&CK Mapping | Mapping activity to known adversary tactics |
| Incident Investigation | Following attacker activity through multiple phases |
| Log Analysis | Identifying suspicious activity within system artifacts |
| Attack Lifecycle Analysis | Understanding how attacks progress across stages |

---

## 🧭 Threat Actor Analysis

The investigation compared several simulated adversary groups including:

- **Ethereal Treasure**
- **Nuclear Tangerine**
- **Black Lotus**
- **Moriarty**
- **Reichenbach**

Each group demonstrated different tactics across the attack lifecycle.

Analysis required identifying which techniques aligned with specific attacker behavior.

---

## 🧩 Attack Lifecycle Observed

The investigation followed the typical cyber intrusion lifecycle:

| Phase | Example Techniques |
|------|------|
| Reconnaissance | active scanning, victim organization research |
| Resource Development | infrastructure acquisition, domain creation |
| Initial Access | phishing campaigns, valid credential abuse |
| Execution | PowerShell, command interpreter usage |
| Persistence | scheduled tasks, account manipulation |
| Privilege Escalation | credential theft and abuse |
| Defense Evasion | log deletion, timestomping |
| Credential Access | password spraying and cracking |
| Discovery | account and network enumeration |
| Lateral Movement | internal spearphishing |
| Command & Control | web protocols and remote access |
| Exfiltration | data transfer over alternative channels |

---

## 🛠 Tools & Techniques Used

<img src="https://img.icons8.com/color/48/windows-10.png" width="25"/> Windows Event Logs  
<img src="https://img.icons8.com/color/48/linux.png" width="25"/> Linux systems  
<img src="https://img.icons8.com/color/48/python.png" width="25"/> Python scripting  
<img src="https://img.icons8.com/color/48/network.png" width="25"/> network traffic analysis  

</div>


Additional techniques included:

- event log investigation
- attacker behavioral comparison
- attack lifecycle reconstruction
- adversary technique attribution

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
| T1041 | Exfiltration Over C2 Channel |

---

## 💡 Key Lessons Learned

- Attackers rarely rely on a single technique
- Attribution requires pattern recognition across multiple tactics
- Understanding the attack lifecycle is critical for defenders
- MITRE ATT&CK provides a useful framework for organizing investigations
- Threat hunting requires both technical analysis and behavioral reasoning

---

<div align="center">

🛰 Investigating attacker behavior  
🧠 Mapping adversary tactics  
🛡 Strengthening defensive analysis

</div>
