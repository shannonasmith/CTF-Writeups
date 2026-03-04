<div align="center">

# 🔁 Lateral Movement — Expanding Across the Network
## Moving Between Systems After Initial Compromise

![Category](https://img.shields.io/badge/Category-Lateral%20Movement-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Network%20Propagation-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors moved laterally across systems after establishing a foothold in the environment.

Lateral movement techniques allow attackers to expand access from a single compromised system to additional hosts across the network.  
This enables them to reach sensitive systems, escalate privileges, and maintain operational control of the environment.

Understanding lateral movement is critical for detecting **attack propagation within internal networks**.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, adversary groups demonstrated methods for spreading access between systems and users.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each adversary leveraged internal relationships and authentication mechanisms to move across the environment.

---

## 🔍 Observed Lateral Movement Techniques

| Technique | Description |
|------|------|
| Internal Spearphishing | Sending malicious emails within the organization to compromise additional users |
| Credential Reuse | Using harvested credentials to authenticate to other systems |
| Remote Access Tools | Leveraging remote access protocols or administrative tools |
| Service-Based Movement | Accessing network services that allow remote execution |

These techniques allow attackers to transition from one compromised system to many others.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Internal Spearphishing | T1534 |
| Remote Services | T1021 |
| Lateral Tool Transfer | T1570 |
| Valid Accounts | T1078 |

---

## 🛡 Defensive Insight

Lateral movement activity often appears as **unusual authentication patterns across systems**.

Security teams should monitor for:

- authentication attempts from unusual hosts  
- logins between systems that rarely communicate  
- repeated credential usage across multiple machines  
- abnormal internal email activity

Detecting lateral movement early can significantly reduce the impact of an intrusion.

---

## 💡 Skills Reinforced

- Network propagation analysis  
- Authentication pattern monitoring concepts  
- MITRE ATT&CK lateral movement mapping  
- Understanding attacker network expansion strategies  

---

<div align="center">

🔁 Attackers move to gain control  
🔎 Monitor internal authentication activity  
🛡 Stop propagation before escalation  

</div>
