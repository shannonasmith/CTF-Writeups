<div align="center">

# 🚪 Initial Access — Intrusion Entry Techniques
## Gaining the First Foothold

![Category](https://img.shields.io/badge/Category-Initial%20Access-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Attack%20Entry%20Techniques-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

# 🎯 Objective

Identify how simulated threat actors obtained their **initial foothold** within the target environment.

Initial access represents the point where attackers successfully transition from **external reconnaissance** to **internal system access**.

Understanding this phase is critical because it marks the beginning of an active compromise.

---

# 🖥 Investigation Context

Within the SkillsQuest investigation scenario, multiple adversary groups demonstrated different methods of gaining access to victim systems.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each actor leveraged different techniques depending on their operational goals and available resources.

---

# 🔍 Observed Initial Access Techniques

| Technique | Description |
|------|------|
| Valid Credentials | Using previously compromised usernames and passwords |
| Phishing Campaigns | Social engineering to capture credentials or deliver malicious payloads |
| Trusted Relationship Abuse | Leveraging relationships between organizations to gain access |
| Infrastructure-Based Access | Using attacker-controlled domains or web services as entry points |

These techniques allowed attackers to bypass traditional perimeter defenses.

---

# 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Valid Accounts | T1078 |
| Phishing | T1566 |
| Trusted Relationship | T1199 |
| External Remote Services | T1133 |

---

# 🛡 Defensive Insight

Initial access techniques frequently rely on **human error or credential compromise**.

Common indicators defenders should monitor include:

- unusual login attempts
- suspicious authentication patterns
- unexpected access from new locations
- credential usage outside normal operating hours

Preventing or detecting this phase can stop attacks before attackers begin executing commands inside the network.

---

# 💡 Skills Reinforced

- Attack lifecycle analysis  
- Authentication anomaly detection concepts  
- MITRE ATT&CK mapping  
- Understanding common enterprise intrusion entry points  

---

<div align="center">

🚪 Every intrusion begins somewhere  
🔎 Watch authentication patterns  
🛡 Stop attackers before they execute  

</div>
