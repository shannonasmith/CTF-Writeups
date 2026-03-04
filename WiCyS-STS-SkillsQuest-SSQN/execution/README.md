<div align="center">

# ⚙️ Execution — Command & Script Activity
## Running Malicious Code on Target Systems

![Category](https://img.shields.io/badge/Category-Execution-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Command%20Execution-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-MITRE%20ATT%26CK-red?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze how simulated threat actors executed commands or malicious code after gaining initial access.

Execution is the phase where attackers begin actively interacting with compromised systems by running scripts, launching tools, or executing commands that enable further control of the environment.

This phase often marks the transition from **initial compromise** to **active attacker operations**.

---

## 🖥 Investigation Context

Within the SkillsQuest investigation scenario, several adversary groups demonstrated different methods of executing commands on compromised systems.

Threat actors analyzed included:

- Ethereal Treasure  
- Nuclear Tangerine  
- Black Lotus  
- Moriarty  
- Reichenbach  

Execution methods varied depending on attacker capabilities and objectives.

---

## 🔍 Observed Execution Techniques

| Technique | Description |
|------|------|
| Command Interpreter | Running commands through system shells such as PowerShell or Windows Command Prompt |
| Script Execution | Using scripting languages to automate attacker tasks |
| Client-Side Exploitation | Triggering code execution through vulnerabilities in client software |
| Scheduled Task Execution | Running commands automatically through system scheduling mechanisms |

Execution activity often enables attackers to begin discovery, persistence, or lateral movement operations.

---

## 🧠 MITRE ATT&CK Mapping

| Technique | ID |
|------|------|
| Command and Scripting Interpreter | T1059 |
| PowerShell | T1059.001 |
| Windows Command Shell | T1059.003 |
| Scheduled Task / Job | T1053 |

---

## 🛡 Defensive Insight

Execution activity frequently leaves identifiable artifacts within system logs.

Security teams can detect this phase by monitoring:

- PowerShell Script Block logging
- unusual command-line activity
- suspicious scheduled task creation
- unexpected script execution

Early detection of malicious execution can prevent attackers from escalating privileges or expanding their access.

---

## 💡 Skills Reinforced

- Command execution analysis  
- Script interpreter behavior recognition  
- MITRE ATT&CK technique mapping  
- Understanding attacker operational workflow  

---

<div align="center">

⚙️ Execution turns access into control  
🔎 Monitor command activity closely  
🛡 Detect attacker actions early  

</div>
