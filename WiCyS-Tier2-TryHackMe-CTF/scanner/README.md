<div align="center">

# 📡 Scanner  
## Service Discovery & Unusual Port Analysis

![Category](https://img.shields.io/badge/Category-Network%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Service%20Discovery-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Port%20Analysis-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a mysterious signal originating from a remote system and determine whether the service reveals hidden information.

The challenge description suggested that the system exposed a service but provided limited opportunities to discover it.

The objective was to perform **network scanning and service interrogation** to determine whether the host exposed any accessible resources.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Kali Linux AttackBox | Network investigation |
| Nmap | Port and service scanning |
| curl | Direct HTTP interaction |
| Terminal | Command execution |

---

### 📦 Step 1 — Perform Initial Service Discovery

The investigation began by scanning the target host to identify available services.

Because the challenge hinted at a hidden signal, a targeted scan was performed against a specific port using Nmap.

The scan included the **http-headers script** to identify whether the service returned HTTP metadata.

---

### 🔍 Step 2 — Analyze Nmap Script Output

The Nmap scan revealed that the target system responded to requests on an **unusual port**.

Rather than using a typical web port such as:

```
80
443
8080
```

the service responded on **port 1**, which is rarely used for web applications.

This unusual configuration suggested that the challenge intentionally hid the service on a **non-standard port** to make discovery more difficult.

---

### 🧪 Step 3 — Interact with the Service

After confirming that the port responded to HTTP requests, the next step was to manually interact with the service using `curl`.

This allowed the response body to be retrieved directly from the server.

```
curl TARGET_IP:1
```

The server returned an HTTP response containing embedded information.

---

#### 🔎 Analytical Observation

Security testing often involves investigating **non-standard ports** because services may run outside their expected locations.

Attackers frequently discover exposed services by scanning the entire port range and identifying unusual responses.

This challenge demonstrates how **services running on uncommon ports can still expose sensitive information**.

---

### 🔄 Step 4 — Analyze the HTTP Response

The HTTP response returned by the server contained embedded data that was not visible without directly interacting with the service.

Because the service was hosted on an unusual port, it would likely be overlooked during casual inspection.

This emphasizes the importance of **comprehensive service enumeration during reconnaissance**.

---

### 🔐 Step 5 — Confirm Exposed Information

The response from the service confirmed that the system exposed sensitive information through the HTTP response.

📸 **Service Response from Unusual Port**

<img src="../images/image009_redacted.png" width="600">

This confirmed that the service hosted on the unexpected port contained the information required to complete the investigation.

---

## 🧠 Methodology Framework Applied

```
Target identification
      ↓
Port scanning
      ↓
Service detection
      ↓
Manual HTTP interrogation
      ↓
Response analysis
      ↓
Sensitive information discovery
```

---

## 🛠 Techniques Used

Primary techniques used:

- network port scanning  
- service detection  
- HTTP header analysis  
- manual service interaction  

Key concept investigated:

```
Non-standard service ports
```

---

## 🛡 Defensive Insight

Services running on unusual ports are not inherently secure.

Security through obscurity can delay discovery but does not prevent attackers from identifying exposed services through systematic scanning.

Organizations should ensure that:

- only necessary services are exposed
- firewall rules restrict unnecessary ports
- network monitoring detects unusual service behavior

Proper service management reduces the attack surface of exposed infrastructure.

---

## 💡 Skills Reinforced

- Network reconnaissance  
- Port scanning methodology  
- Service discovery techniques  
- HTTP response analysis  
- Identifying services running on non-standard ports  

---

<div align="center">

📡 Scan beyond common ports  
🔍 Unusual services may hide sensitive data  
🧠 Enumeration is the foundation of security testing  

</div>
