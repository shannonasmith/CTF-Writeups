<div align="center">

# 🔒 Persistence — Maintaining Long-Term Access
## Ensuring Continued Control of Compromised Systems

![Category](https://img.shields.io/badge/Category-Persistence-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Long--Term%20Access-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors maintained **continued access** to compromised systems after initial execution.

Persistence techniques allow attackers to remain inside an environment even if the original access vector is discovered or removed.

Establishing persistence ensures that attackers can **reconnect later without repeating the initial intrusion process**.

---

## 🖥 Investigation Context

During the SkillsQuest investigation scenario, several adversary groups demonstrated different persistence mechanisms designed to survive system restarts or administrative intervention.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each adversary leveraged persistence techniques that aligned with their broader attack strategy.

---

## 🔍 Observed Persistence Techniques

| Technique | Description |
|------|------|
| Account Manipulation | Modifying existing accounts or creating new ones for continued access |
| Scheduled Tasks | Creating automated jobs that execute attacker commands |
| Web Shells | Deploying scripts on web servers that allow remote command execution |
| Account Creation | Establishing hidden or secondary accounts for long-term access |

These techniques ensure attackers retain access even after detection efforts begin.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Account Manipulation | T1098 |
| Create Account | T1136 |
| Scheduled Task / Job | T1053 |
| Web Shell | T1505.003 |

---

## 🛡 Defensive Insight

Persistence mechanisms often leave traces that can be detected through monitoring and configuration auditing.

Security teams should watch for:

- unexpected scheduled task creation  
- newly created user accounts  
- unusual account privilege changes  
- unknown scripts or web server modifications  

Regular system audits and configuration monitoring are critical for identifying unauthorized persistence mechanisms.

---

## 💡 Skills Reinforced

- Persistence mechanism identification  
- System configuration auditing concepts  
- MITRE ATT&CK persistence technique mapping  
- Understanding attacker long-term access strategies  

---

<div align="center">

🔒 Persistence keeps attackers inside  
🔎 Audit accounts and scheduled tasks  
🛡 Remove persistence to regain control  

</div>
