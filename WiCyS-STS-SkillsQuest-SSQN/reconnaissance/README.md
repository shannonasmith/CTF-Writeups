<div align="center">

# 🔎 Reconnaissance — Threat Intelligence Analysis
## Adversary Information Gathering

![Category](https://img.shields.io/badge/Category-Reconnaissance-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Threat%20Actor%20Behavior-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Identify how different simulated threat actors conduct **reconnaissance activities** before launching attacks.

Reconnaissance represents the **information gathering phase** of an intrusion where attackers collect data about:

- target infrastructure
- user identities
- exposed services
- organizational structure

Understanding these behaviors allows defenders to detect **early indicators of compromise**.

---

## 🖥 Investigation Context

The SkillsQuest scenario provided several simulated adversary groups whose behaviors had to be compared and classified.

Threat actors analyzed included:

- Ethereal Treasure
- Nuclear Tangerine
- Black Lotus
- Moriarty
- Reichenbach

Each group demonstrated different reconnaissance techniques.

---

## 🔍 Observed Reconnaissance Techniques

| Technique | Description |
|------|------|
| Active Scanning | Probing network services to identify exposed systems |
| Wordlist Scanning | Automated discovery of hidden web resources |
| Victim Organization Research | Collecting company or infrastructure information |
| Victim Identity Research | Identifying users and credentials associated with the target |

These activities align with early-stage intrusion behavior.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Active Scanning | T1595 |
| Gather Victim Identity Information | T1589 |
| Gather Victim Organization Information | T1591 |

---

## 🛡 Defensive Insight

Reconnaissance activity often appears **benign at first**, making detection difficult.

However, early indicators such as:

- unusual scanning activity
- repeated enumeration attempts
- automated wordlist probing

can signal **pre-attack reconnaissance**.

Detecting this stage provides defenders with an opportunity to disrupt attacks **before initial access occurs**.

---

## 💡 Skills Reinforced

- Threat actor behavioral analysis  
- MITRE ATT&CK technique mapping  
- Attack lifecycle understanding  
- Early-stage intrusion detection concepts  

---

<div align="center">

🔎 Detect reconnaissance early  
🧠 Understand attacker preparation  
🛡 Stop attacks before they start

</div>
