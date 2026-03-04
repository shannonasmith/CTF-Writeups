<div align="center">

# ⬆️ Privilege Escalation — Expanding Access Rights
## Gaining Elevated System Permissions

![Category](https://img.shields.io/badge/Category-Privilege%20Escalation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Access%20Expansion-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors escalated privileges after gaining initial access to the environment.

Privilege escalation allows attackers to obtain **higher levels of system access**, enabling them to perform actions that normal users cannot perform, such as modifying system configurations, accessing restricted data, or disabling security controls.

This stage often marks the transition from **limited access** to **full system control**.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated techniques used to elevate privileges within compromised environments.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each actor leveraged privilege escalation to gain broader control over systems and network resources.

---

## 🔍 Observed Privilege Escalation Techniques

| Technique | Description |
|------|------|
| Account Manipulation | Modifying user accounts to grant elevated permissions |
| Credential Abuse | Using stolen or recovered credentials with higher privileges |
| Cloud Credential Theft | Extracting credentials from cloud services or instance metadata |
| Privileged Account Usage | Leveraging administrative or service accounts |

These techniques enable attackers to bypass normal access restrictions and gain control of critical systems.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Account Manipulation | T1098 |
| Valid Accounts | T1078 |
| Credential Access | T1003 |
| Abuse Elevation Control Mechanism | T1548 |

---

## 🛡 Defensive Insight

Privilege escalation often generates detectable indicators within authentication logs and system events.

Security teams should monitor for:

- unexpected administrative account usage  
- unusual privilege changes  
- new accounts granted elevated permissions  
- credential usage inconsistent with normal behavior  

Strong access control policies and privilege monitoring can significantly reduce the risk of privilege escalation attacks.

---

## 💡 Skills Reinforced

- Privilege escalation pattern recognition  
- Credential abuse detection concepts  
- MITRE ATT&CK technique mapping  
- Understanding attacker privilege expansion strategies  

---

<div align="center">

⬆️ Privileges expand attacker control  
🔎 Monitor administrative account activity  
🛡 Enforce least-privilege access  

</div>
