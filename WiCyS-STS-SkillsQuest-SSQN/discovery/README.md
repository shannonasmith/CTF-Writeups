<div align="center">

# 🧭 Discovery — Mapping the Internal Environment
## Identifying Systems, Accounts, and Resources

![Category](https://img.shields.io/badge/Category-Discovery-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Network%20Enumeration-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors performed **internal discovery** after gaining access to the target environment.

Discovery techniques allow attackers to identify valuable systems, accounts, and resources that can be leveraged for further compromise.

This stage helps attackers determine:

- which users have elevated privileges  
- which systems are connected within the network  
- where sensitive data might be stored  

Understanding discovery behavior helps defenders identify attackers **actively exploring the environment**.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups conducted reconnaissance inside the compromised environment.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each actor used discovery techniques to better understand the internal network structure.

---

## 🔍 Observed Discovery Techniques

| Technique | Description |
|------|------|
| Account Discovery | Identifying user accounts within the environment |
| Domain Discovery | Enumerating domain structures and relationships |
| Email Account Discovery | Identifying email accounts associated with the organization |
| Network Enumeration | Mapping systems and services across the network |

These techniques provide attackers with information needed to plan lateral movement and data access.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Account Discovery | T1087 |
| Domain Account Discovery | T1087.002 |
| Network Service Discovery | T1046 |
| System Information Discovery | T1082 |

---

## 🛡 Defensive Insight

Discovery activity often produces detectable patterns within system and network logs.

Indicators defenders should monitor include:

- enumeration commands executed from compromised hosts  
- large numbers of directory or account queries  
- unusual system or network scanning activity  
- internal mapping behavior from a single host

Monitoring internal enumeration behavior can reveal attackers who are actively preparing for lateral movement.

---

## 💡 Skills Reinforced

- Network enumeration analysis  
- Internal reconnaissance detection concepts  
- MITRE ATT&CK discovery technique mapping  
- Understanding attacker environment mapping strategies  

---

<div align="center">

🧭 Attackers map before they move  
🔎 Watch internal enumeration activity  
🛡 Detect exploration before expansion  

</div>
