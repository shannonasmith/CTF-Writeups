<div align="center">

# 🏠 df03 — New House Investigation
## Multi-Artifact Incident Investigation

![Category](https://img.shields.io/badge/Category-DFIR-darkred?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Multi--Artifact%20Analysis-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Timeline%20Reconstruction-orange?style=for-the-badge)

</div>

---

## 🎯 Objective

Investigate a collection of system artifacts to determine what activity occurred on a compromised environment.

The challenge required analyzing multiple data sources including:

- Windows system logs  
- Linux indicators  
- network packet captures (PCAP)  
- downloaded artifacts  

The objective was to reconstruct attacker behavior and identify key indicators of compromise across the system.

---

## 🖥 Environment

- Windows log artifacts  
- PCAP network capture  
- HTTP traffic inspection  
- host artifact review tools  

---

## 🔎 Step 1 — Establish Investigation Scope

The provided artifacts suggested that the system had experienced suspicious activity involving both host-level and network-level behavior.

Initial investigative goals included:

- identifying suspicious system changes  
- determining attacker access methods  
- identifying tools used during the intrusion  
- reconstructing a timeline of events  

Understanding the available evidence sources was the first step toward building an investigative workflow.

---

## 🔍 Step 2 — Investigate Host Artifacts

Host-level artifacts were examined to identify system modifications.

Areas of focus included:

- user and group changes  
- scheduled task activity  
- system configuration changes  

These artifacts help determine whether the attacker attempted to establish persistence or modify system privileges.

Host-based investigation provides the foundation for understanding how the attacker interacted with the compromised machine.

---

## 🧪 Step 3 — Analyze Network Traffic

A packet capture file was provided to examine network communications associated with the incident.

PCAP analysis focused on identifying:

- external connections made by the host  
- suspicious downloads  
- command and control communication patterns  

By examining HTTP traffic within the capture, it became possible to identify potential tools or files transferred to the system during the compromise.

---

## 🌐 Step 4 — Attribute Network Activity

Network traffic inspection revealed identifying characteristics of the tools and clients involved.

One key artifact examined during this phase was the **HTTP User-Agent string**, which can provide clues about:

- the application making the request  
- the operating system involved  
- automation tools used by attackers  

User-Agent analysis can assist investigators in identifying the tooling used during an attack.

---

## 🔄 Step 5 — Reconstruct the Attack Timeline

By combining information from:

- host artifacts  
- authentication events  
- network traffic  
- downloaded files  

it became possible to build a timeline of activity across the system.

Correlating these events helped reveal the sequence of attacker actions and how the compromise progressed.

---

## 🧠 Methodology Framework Applied

1. Identify available artifacts  
2. Establish investigative scope  
3. analyze host-level indicators  
4. inspect network traffic  
5. identify attacker tooling  
6. correlate host and network evidence  
7. reconstruct event timeline  

---

## 🛡 Defensive Insight

Real-world incident investigations often require correlation across multiple evidence sources.

Attackers rarely leave evidence in only one location. Instead, indicators may appear in:

- authentication logs  
- system configuration changes  
- network communications  
- downloaded artifacts  

Effective detection and response requires the ability to **correlate these artifacts into a coherent investigative narrative**.

---

## 💡 Skills Reinforced

- multi-artifact forensic investigation  
- host and network correlation  
- PCAP inspection  
- HTTP artifact analysis  
- timeline reconstruction techniques  

---

<div align="center">

🔎 Follow the artifacts  
🧠 Correlate the evidence  
🛡 Build the timeline  

</div>
