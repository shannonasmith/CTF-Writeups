<div align="center">

# 🔎 Scanner  
## Network Reconnaissance & Service Discovery

![Category](https://img.shields.io/badge/Category-Network%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Service%20Enumeration-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Reconnaissance-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze a target system to determine which services are exposed and accessible.

The goal of this challenge was to identify open ports and running services on the target host, then interpret the results to determine what systems or applications were available for further investigation.

This exercise focused on **network reconnaissance and service enumeration**.

---

## 🖥 Environment

- Kali Linux  
- Network scanning tools  
- Terminal-based enumeration utilities  
- Basic networking knowledge  

---

## 🔍 Step 1 — Identify the Target Host

The challenge provided a target system that required investigation.

Initial reconnaissance focused on identifying:

- reachable network services  
- exposed ports  
- potential entry points  

Before interacting with applications, it is important to understand **what services are available on the system**.

---

## 🔎 Step 2 — Perform Network Scanning

A network scanning tool was used to enumerate open ports and identify running services on the target host.

Scanning reveals:

- which ports are open
- which services are listening
- possible software running behind those services

Understanding the exposed attack surface is a foundational step in security assessments.

---

## 🔄 Step 3 — Analyze Scan Results

After scanning completed, the results were reviewed to determine:

- which services were active  
- what protocols were in use  
- whether version information was available  

Service banners and port information can provide valuable clues about system configuration and potential vulnerabilities.

---

## 🔐 Step 4 — Interpret Exposed Services

Once open services were identified, the next step was to determine which services were most relevant for further investigation.

Typical analysis includes:

- identifying web services
- checking administrative interfaces
- reviewing unusual or unexpected open ports

This step helps prioritize which services should be examined more closely during a security investigation.

---

# 🧠 Methodology Framework Applied

1. Identify target system  
2. Perform network reconnaissance  
3. Enumerate open ports  
4. Identify exposed services  
5. Analyze service information  
6. Prioritize potential attack surfaces  

---

# 🛡 Defensive Insight

Network scanning is one of the first techniques used during both legitimate security testing and malicious reconnaissance.

Organizations should monitor for scanning behavior and implement controls such as:

- network intrusion detection systems  
- firewall filtering  
- service hardening  
- minimizing exposed services  

Reducing unnecessary exposed services significantly limits the system's attack surface.

---

# 💡 Skills Reinforced

- Network reconnaissance  
- Service enumeration  
- Port scanning interpretation  
- Attack surface identification  
- Prioritizing investigation targets  

---

<div align="center">

🔎 Understand the attack surface first  
📡 Enumerate services before interacting with them  
🧠 Reconnaissance guides effective investigation  

</div>
