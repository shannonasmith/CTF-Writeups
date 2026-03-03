<div align="center">

# 🚨 Unwanted Visitor  
## Windows Log Investigation & Persistence Detection

![Category](https://img.shields.io/badge/Category-DFIR-darkred?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Windows%20Event%20Logs-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Incident%20Investigation-orange?style=for-the-badge)

</div>

---

## 🎯 Objective

Investigate Windows system artifacts to determine whether unauthorized activity occurred on the host.

The challenge required analyzing system logs to identify evidence of attacker behavior, persistence mechanisms, and suspicious command execution.

This exercise focused on identifying indicators of compromise within **Windows event logs and PowerShell activity records**.

---

## 🖥 Environment

- Windows Event Log artifacts  
- Log analysis tools  
- PowerShell log inspection  
- Windows security auditing concepts  

---

## 🔎 Step 1 — Inspect Security Event Logs

The investigation began with analysis of the **Security Event Log**.

Windows Security logs provide visibility into authentication activity, including:

- successful logins
- failed login attempts
- account privilege use
- account creation or modification

A key event type examined during the investigation was:

**Event ID 4624 — Successful Logon**

This event can reveal:

- the account used
- the logon type
- the originating host
- the authentication process involved

By reviewing these events, it became possible to identify when a user successfully authenticated to the system.

---

## 🔍 Step 2 — Identify Suspicious Authentication Activity

Log entries were reviewed to determine:

- which accounts logged into the system
- whether unexpected accounts were used
- the timing of authentication events

Unusual login activity can indicate that an attacker gained access to the host.

Investigating authentication events provides the first step toward reconstructing an attack timeline.

---

## 🧪 Step 3 — Review PowerShell Script Block Logging

Further analysis revealed PowerShell activity within the system logs.

PowerShell Script Block Logging records commands executed through PowerShell and can expose attacker techniques.

Of particular interest were commands involving:

- `Invoke-Expression (IEX)`
- encoded command execution
- suspicious script behavior

PowerShell is frequently abused by attackers because it allows powerful system interaction while blending into legitimate administrative activity.

---

## 🔄 Step 4 — Investigate Persistence Mechanisms

After identifying suspicious command execution, the investigation expanded to determine whether the attacker attempted to maintain access to the system.

Common persistence techniques include:

- scheduled tasks
- registry run keys
- service installation
- hidden user accounts

Evidence in the logs indicated activity consistent with persistence attempts, suggesting that the attacker intended to retain long-term access.

---

## 🧠 Methodology Framework Applied

1. Load Windows event log artifacts  
2. Review authentication events  
3. Identify suspicious logon activity  
4. Analyze PowerShell command execution  
5. Evaluate system changes for persistence indicators  
6. reconstruct attacker behavior timeline  
7. validate investigative findings  

---

## 🛡 Defensive Insight

Windows event logs provide critical forensic evidence during incident response.

Organizations should ensure that:

- security logging is enabled
- PowerShell Script Block Logging is configured
- centralized logging systems (such as SIEM platforms) collect and retain these events

Proper log visibility significantly improves an organization's ability to detect and investigate malicious activity.

---

## 💡 Skills Reinforced

- Windows event log analysis  
- Authentication event investigation  
- PowerShell activity inspection  
- persistence detection concepts  
- incident response investigation methodology  

---

<div align="center">

🔎 Investigate the logs  
🧠 Reconstruct the timeline  
🛡 Detect persistence early  

</div>
