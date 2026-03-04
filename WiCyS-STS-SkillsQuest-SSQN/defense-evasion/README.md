<div align="center">

# 🕶 Defense Evasion — Hiding Malicious Activity
## Avoiding Detection and Security Controls

![Category](https://img.shields.io/badge/Category-Defense%20Evasion-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Stealth%20Techniques-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors avoided detection while operating inside compromised environments.

Defense evasion techniques allow attackers to **hide their presence**, disable security monitoring, or obscure malicious activity to remain undetected for as long as possible.

This phase is critical because attackers who successfully evade detection can continue operating without interruption.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated different techniques to evade defensive monitoring.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each adversary applied methods designed to obscure activity or bypass security controls.

---

## 🔍 Observed Defense Evasion Techniques

| Technique | Description |
|------|------|
| Token Impersonation | Using stolen authentication tokens to impersonate legitimate users |
| File Permission Manipulation | Altering permissions to restrict visibility or access to malicious files |
| Log Manipulation | Deleting or modifying logs to remove evidence of attacker activity |
| Indicator Removal | Removing files, artifacts, or traces left during intrusion activity |
| Timestomping | Modifying file timestamps to hide the true timeline of attacker actions |

These techniques help attackers maintain stealth while continuing other stages of the intrusion.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Impair Defenses | T1562 |
| Indicator Removal on Host | T1070 |
| Timestomp | T1070.006 |
| Token Impersonation/Theft | T1134 |
| File and Directory Permissions Modification | T1222 |

---

## 🛡 Defensive Insight

Defense evasion techniques are designed to obscure evidence of compromise, making detection more difficult.

Security teams can detect these behaviors by monitoring:

- unexpected log deletion or modification  
- unusual file permission changes  
- abnormal authentication token usage  
- discrepancies between event timelines and system artifacts  

Maintaining centralized logging and monitoring can reduce the effectiveness of attacker evasion attempts.

---

## 💡 Skills Reinforced

- Detection evasion pattern recognition  
- Log integrity monitoring concepts  
- Artifact timeline analysis  
- MITRE ATT&CK defense evasion mapping  

---

<div align="center">

🕶 Attackers hide to survive  
🔎 Protect and monitor system logs  
🛡 Visibility defeats stealth  

</div>
