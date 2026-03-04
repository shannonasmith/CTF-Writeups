<div align="center">

# 🚚 Contrabando  
## Boot-to-Root Investigation & System Privilege Escalation

![Category](https://img.shields.io/badge/Category-System%20Exploitation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Privilege%20Escalation-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-System%20Enumeration-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Investigate a vulnerable system to identify weaknesses that allow deeper access to the environment.

The challenge required analyzing the exposed services, interacting with system components, and identifying opportunities to escalate privileges within the system.

This exercise focused on **system enumeration, exploitation methodology, and privilege escalation concepts** commonly encountered in boot-to-root style challenges.

---

## 🖥 Environment

- Kali Linux  
- Terminal-based system interaction  
- Enumeration utilities  
- Linux command-line investigation tools  

---

## 🔍 Step 1 — Initial System Reconnaissance

The investigation began by examining the available services exposed by the system.

Initial reconnaissance focused on:

- identifying accessible interfaces  
- determining which services were running  
- observing how the system responded to connection attempts  

Understanding the exposed attack surface helps guide further investigation.

---

## 🔎 Step 2 — Enumerate System Components

After establishing initial access to the environment, the next step involved enumerating system components to identify potential weaknesses.

Enumeration activities included:

- reviewing available files and directories  
- identifying configuration artifacts  
- inspecting permissions and accessible resources  

System enumeration often reveals misconfigurations that can be leveraged for deeper access.

---

## 🔄 Step 3 — Identify Privilege Escalation Opportunity

Further inspection of the system revealed behavior or configuration elements that suggested a potential privilege escalation path.

Indicators of privilege escalation opportunities can include:

- improperly configured permissions  
- accessible scripts or binaries  
- misconfigured system services  

Careful inspection of system artifacts helped reveal the mechanism necessary to progress further in the challenge.

---

## 🔐 Step 4 — Achieve Elevated Access

By leveraging the identified system weakness, it became possible to access information or functionality that was restricted under normal conditions.

This demonstrated that the system contained a **privilege escalation pathway**, allowing deeper access into the environment.

The challenge highlighted how small configuration issues can lead to significant security risks when combined with systematic investigation techniques.

---

# 🧠 Methodology Framework Applied

1. Perform initial system reconnaissance  
2. Enumerate system services and resources  
3. Inspect system configuration artifacts  
4. Identify potential privilege escalation paths  
5. Leverage discovered weakness  
6. Confirm elevated system access  

---

# 🛡 Defensive Insight

Privilege escalation vulnerabilities often arise from configuration errors or overly permissive system settings.

Secure system design should include:

- strict permission management  
- regular system auditing  
- secure configuration of services and scripts  
- monitoring for suspicious privilege escalation attempts  

Preventing privilege escalation is critical for maintaining system security once an attacker gains initial access.

---

# 💡 Skills Reinforced

- System enumeration techniques  
- Linux environment investigation  
- Privilege escalation analysis  
- Boot-to-root methodology  
- Security evaluation of system configurations  

---

<div align="center">

🚚 Hidden system weaknesses often enable escalation  
🔎 Enumeration reveals privilege pathways  
🧠 Boot-to-root challenges reinforce full investigation workflows  

</div>
