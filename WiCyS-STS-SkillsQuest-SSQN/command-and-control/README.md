<div align="center">

# 📡 Command and Control — Remote Attacker Communication
## Maintaining Control of Compromised Systems

![Category](https://img.shields.io/badge/Category-Command%20%26%20Control-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Network%20Communication-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors established **command and control (C2)** channels to communicate with compromised systems.

Command and control infrastructure allows attackers to send instructions to infected machines, receive collected data, and coordinate further activity within the environment.

Maintaining reliable communication channels is critical for sustaining attacker operations.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated different methods of establishing remote communication with compromised systems.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Each group implemented command-and-control mechanisms suited to their operational needs.

---

## 🔍 Observed Command & Control Techniques

| Technique | Description |
|------|------|
| Web Service Communication | Using standard web protocols to communicate with attacker infrastructure |
| Application Layer Protocol | Leveraging common protocols such as HTTP or HTTPS for C2 traffic |
| Non-Standard Application Protocol | Using uncommon or custom protocols to evade detection |
| Remote Access Software | Using remote tools to control compromised machines |

These techniques allow attackers to maintain persistent communication with infected systems.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Application Layer Protocol | T1071 |
| Web Protocols | T1071.001 |
| Non-Standard Port | T1571 |
| Remote Access Software | T1219 |

---

## 🛡 Defensive Insight

Command and control traffic often blends with normal network communication to avoid detection.

Security teams should monitor for:

- unusual outbound connections  
- connections to newly registered or suspicious domains  
- unexpected traffic patterns over common protocols such as HTTP or HTTPS  
- persistent connections from internal systems to external infrastructure  

Network traffic analysis and anomaly detection can help identify potential command-and-control channels.

---

## 💡 Skills Reinforced

- Network traffic behavior analysis  
- Command-and-control detection concepts  
- MITRE ATT&CK C2 technique mapping  
- Understanding attacker remote control mechanisms  

---

<div align="center">

📡 Attackers must communicate to control  
🔎 Monitor outbound network traffic  
🛡 Detect suspicious external connections  

</div>
