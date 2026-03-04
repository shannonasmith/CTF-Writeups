<div align="center">

# 📤 Exfiltration — Data Extraction from Compromised Systems
## Removing Data from the Target Environment

![Category](https://img.shields.io/badge/Category-Exfiltration-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Data%20Theft-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors removed sensitive data from compromised systems.

Exfiltration represents the stage where attackers transfer stolen information outside the target environment.  
This phase often occurs after attackers have completed discovery, credential access, and lateral movement.

Successful exfiltration allows attackers to achieve their primary objectives, such as data theft, espionage, or financial gain.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated different techniques used to transfer stolen data.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each group leveraged different channels to move data outside the environment.

---

## 🔍 Observed Exfiltration Techniques

| Technique | Description |
|------|------|
| Web Service Exfiltration | Transferring stolen data using standard web protocols |
| Cloud Storage Exfiltration | Uploading data to attacker-controlled cloud accounts |
| Alternative Protocol Transfer | Using uncommon protocols to bypass network monitoring |
| Encrypted Communication | Protecting exfiltrated data from inspection |

These techniques help attackers extract information while minimizing detection.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Exfiltration Over Web Service | T1567 |
| Exfiltration Over Alternative Protocol | T1048 |
| Exfiltration to Cloud Storage | T1567.002 |
| Encrypted Channel | T1041 |

---

## 🛡 Defensive Insight

Exfiltration activity often produces detectable network anomalies.

Security teams should monitor for:

- unusually large outbound data transfers  
- connections to unfamiliar external services  
- data transfers outside normal business hours  
- encrypted traffic to suspicious destinations  

Network monitoring, data loss prevention (DLP), and traffic anomaly detection can help prevent successful data exfiltration.

---

## 💡 Skills Reinforced

- Data exfiltration pattern recognition  
- Network traffic monitoring concepts  
- MITRE ATT&CK exfiltration technique mapping  
- Understanding attacker data theft strategies  

---

<div align="center">

📤 Data theft is the attacker objective  
🔎 Monitor outbound data movement  
🛡 Detect exfiltration before damage occurs  

</div>
