<div align="center">

# 🏗 Resource Development — Threat Infrastructure Analysis
## Adversary Preparation & Infrastructure Acquisition

![Category](https://img.shields.io/badge/Category-Resource%20Development-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Adversary%20Infrastructure-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

# 🎯 Objective

Analyze how simulated adversary groups establish the infrastructure and resources required to support their attacks.

Resource development occurs **before initial access** and often includes acquiring systems, domains, or accounts that enable attackers to conduct operations without exposing their true identity.

Understanding this phase helps defenders identify attacker preparation activity and infrastructure staging.

---

# 🖥 Investigation Context

Within the SkillsQuest scenario, multiple simulated threat actors demonstrated different approaches to preparing attack infrastructure.

Threat actors examined included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each group used distinct methods to establish resources needed for later stages of intrusion.

---

# 🔍 Observed Resource Development Techniques

| Technique | Description |
|------|------|
| Infrastructure Acquisition | Registering domains or provisioning servers used for malicious operations |
| Account Creation | Establishing accounts that can later be used for authentication or phishing |
| Botnet Infrastructure | Leveraging compromised systems to expand attacker-controlled resources |
| Malware Development | Creating tools used during later execution stages |

These preparations allow attackers to operate indirectly and maintain operational security.

---

# 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Acquire Infrastructure | T1583 |
| Establish Accounts | T1585 |
| Develop Capabilities (Malware / Tools) | T1587 |

---

# 🛡 Defensive Insight

Resource development activities frequently occur **outside the target environment**, making detection difficult.

However, defenders can sometimes identify early warning signs through:

- suspicious domain registrations
- unusual infrastructure connections
- newly created accounts associated with phishing campaigns

Threat intelligence monitoring can help organizations detect attacker infrastructure before it is used in active attacks.

---

# 💡 Skills Reinforced

- Threat actor lifecycle analysis  
- Infrastructure staging recognition  
- MITRE ATT&CK technique classification  
- Adversary preparation phase understanding  

---

<div align="center">

🏗 Infrastructure enables intrusion  
🔎 Track attacker preparation  
🛡 Early detection disrupts campaigns  

</div>
