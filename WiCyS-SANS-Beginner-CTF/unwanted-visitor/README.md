<div align="center">

# 🪟 Unwanted Visitor  
## Windows Log Analysis & Suspicious Activity Investigation

![Category](https://img.shields.io/badge/Category-DFIR-darkred?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Windows%20Log%20Analysis-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Incident%20Investigation-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate suspicious activity occurring on a Windows system and determine how an unauthorized user gained access and executed malicious actions.

The challenge required analyzing Windows artifacts to identify evidence of attacker behavior.

This investigation focused on **authentication events, PowerShell execution, and persistence mechanisms**.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Kali / Ubuntu Linux VM | Investigation environment |
| Windows Event Logs | Authentication event analysis |
| PowerShell Script Block Logs | Command execution tracking |
| Log inspection tools | Artifact examination |

---

### 📦 Step 1 — Examine the Security Event Log

The investigation began by reviewing the **Security.evtx** log.

Windows Security logs record authentication activity and can reveal suspicious login behavior.

Key events of interest included:

```
Event ID 4624 — Successful Logon
```

These events identify when a user successfully authenticates to the system.

---

### 🔍 Step 2 — Identify Suspicious Authentication Activity

Reviewing Event ID 4624 entries revealed login activity associated with a user account accessing the system.

Important fields examined included:

- **Account Name**
- **Logon Type**
- **Workstation Name**
- **Source Network Address**

These details help determine whether the login originated from a legitimate source.

---

### 🧪 Step 3 — Analyze PowerShell Script Block Logs

Further investigation focused on **PowerShell Script Block Logging**, which records commands executed within PowerShell sessions.

Script block logs can reveal attacker activity such as:

- command execution
- malicious script downloads
- privilege escalation attempts

One notable indicator identified during analysis was the use of:

```
Invoke-Expression (IEX)
```

This command is commonly used by attackers to execute dynamically downloaded scripts.

---

### 🔄 Step 4 — Identify Persistence Mechanism

Further log review revealed evidence of **scheduled task creation**.

Scheduled tasks are frequently used by attackers to maintain persistence on compromised systems.

By creating a scheduled task, attackers can ensure their code executes automatically even after system restarts.

This behavior is consistent with common persistence techniques observed in real-world attacks.

---

### 🔐 Step 5 — Detect Obfuscation Techniques

Further analysis revealed that some commands used **ROT13-style obfuscation**.

Obfuscation techniques are commonly used by attackers to avoid detection and make malicious scripts harder to identify during log review.

Decoding the obfuscated content revealed the true intent of the executed commands.

---

## 🧠 Methodology Framework Applied

```
Artifact acquisition
      ↓
Security event log analysis
      ↓
Authentication event investigation
      ↓
PowerShell execution review
      ↓
Persistence detection
      ↓
Obfuscation analysis
```

---

## 🛠 Techniques Used

Primary techniques used:

- Windows event log analysis
- authentication event tracking
- PowerShell command investigation
- persistence mechanism detection
- script obfuscation analysis

Key investigation artifacts:

```
Security.evtx
PowerShell Script Block Logs
```

---

## 🛡 Defensive Insight

Windows logs provide valuable forensic evidence during incident investigations.

Important detection opportunities include:

- unusual authentication patterns
- PowerShell command execution
- scheduled task creation
- obfuscated command usage

Monitoring these indicators can significantly improve an organization's ability to detect malicious activity.

Script block logging in particular provides **high-fidelity visibility into attacker behavior**.

---

## 💡 Skills Reinforced

- Windows event log investigation  
- Authentication event analysis  
- PowerShell command inspection  
- Persistence detection techniques  
- Obfuscation identification  
- Incident response methodology  

---

<div align="center">

🪟 Logs reveal attacker behavior  
🔍 Authentication events tell the story  
🛡 Detection begins with investigation  

</div>
