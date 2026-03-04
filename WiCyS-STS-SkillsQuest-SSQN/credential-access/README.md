<div align="center">

# 🔑 Credential Access — Obtaining Authentication Secrets
## Harvesting and Cracking Credentials

![Category](https://img.shields.io/badge/Category-Credential%20Access-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Password%20Attacks-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors obtained authentication credentials within the compromised environment.

Credential access techniques allow attackers to collect usernames, passwords, tokens, or other authentication secrets that enable further movement across systems.

Successful credential harvesting often leads to **privilege escalation and lateral movement**.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated different techniques for acquiring authentication credentials.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each adversary leveraged different methods depending on the environment and the level of access already obtained.

---

## 🔍 Observed Credential Access Techniques

| Technique | Description |
|------|------|
| Password Guessing | Attempting commonly used passwords to gain access |
| Password Spraying | Trying a single password across many accounts |
| Credential Harvesting | Collecting credentials through phishing or system artifacts |
| Credential Extraction | Retrieving credentials stored in applications such as web browsers |
| Network Credential Capture | Intercepting credentials transmitted across the network |

These techniques allow attackers to expand their access within the environment.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Brute Force | T1110 |
| Password Spraying | T1110.003 |
| Credentials from Password Stores | T1555 |
| Adversary-in-the-Middle | T1557 |
| Network Sniffing | T1040 |

---

## 🛡 Defensive Insight

Credential access attempts often generate detectable patterns.

Security teams should monitor for:

- repeated authentication failures  
- login attempts across multiple accounts using the same password  
- unusual credential access from unfamiliar systems  
- suspicious network traffic associated with credential interception  

Implementing strong password policies, multi-factor authentication, and monitoring authentication events can significantly reduce the risk of credential compromise.

---

## 💡 Skills Reinforced

- Password attack pattern recognition  
- Credential theft detection concepts  
- MITRE ATT&CK credential access mapping  
- Understanding attacker authentication abuse techniques  

---

<div align="center">

🔑 Credentials unlock systems  
🔎 Monitor authentication behavior  
🛡 Protect identity to protect infrastructure  

</div>
