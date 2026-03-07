<div align="center">

# 🔌 connection

## Network Service Discovery & Data Extraction Investigation

![Category](https://img.shields.io/badge/Category-Linux%20Investigation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Network%20Services-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Service%20Enumeration-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a Linux environment to identify and interact with a locally hosted network service that exposes hidden data.

The challenge required discovering open services, retrieving hosted files, and decoding encoded data to reveal the final message.

This exercise focused on **service enumeration, data retrieval, and multi-stage artifact decoding**.

---

### 🖥 Environment

| Tool                    | Purpose                  |
| ----------------------- | ------------------------ |
| Linux Terminal          | Command-line interaction |
| `nmap`                  | Service discovery        |
| `curl`                  | HTTP interaction         |
| `xxd`                   | Hex decoding             |
| `tar`, `unzip`, `bzip2` | Archive extraction       |

---

### 📦 Step 1 — Discover Running Services

The investigation began by identifying services running on the local machine.

Command used:

```bash
nmap -sT localhost
```

📸 **Local Service Discovery**

<img src="../images/image059_redacted.png" width="600">

The scan revealed an HTTP service running on port **9000**.

---

### 🔍 Step 2 — Interact With the Service

After identifying the service, HTTP requests were sent to the server to inspect its behavior.

Commands used:

```bash
curl http://localhost:9000
curl --http0.9 http://localhost:9000
```

📸 **HTTP Service Interaction**

<img src="../images/image060_redacted.png" width="600">

This revealed accessible resources hosted by the service.

---

### 🧪 Step 3 — Retrieve Encoded Artifact

A file containing encoded data was discovered within the environment.

Commands used:

```bash
cd /var/backups
cp encoded.hex /home/assistant/toolbox/
```

📸 **Encoded Artifact Retrieval**

<img src="../images/image061_redacted.png" width="600">

The file required decoding before further analysis.

---

### 🔄 Step 4 — Decode and Extract Data

The encoded file was converted back into binary format and extracted.

Commands used:

```bash
cat encoded.hex | xxd -ps -r > decoded.zip.bz2
bzip2 -d decoded.zip.bz2
unzip decoded.zip
tar -xvf message.tar.gz
```

📸 **Archive Extraction Process**

<img src="../images/image062_redacted.png" width="600">

These steps revealed a text file containing the hidden message.

---

### 🔐 Step 5 — Inspect Final Message

The final artifact was inspected to reveal the hidden information.

Command used:

```bash
cat message.txt
```

📸 **Recovered Message**

<img src="../images/image063_redacted.png" width="600">

```
SSQ{[redacted]}
```

---

## 🧠 Methodology Framework Applied

```
Service discovery
      ↓
HTTP interaction
      ↓
Artifact retrieval
      ↓
Data decoding
      ↓
Archive extraction
      ↓
Message recovery
```

---

## 🛠 Techniques Used

Primary techniques used:

* service enumeration
* HTTP interaction with curl
* hex decoding with xxd
* archive extraction

Key concept investigated:

```
multi-stage artifact decoding
```

---

## 🛡 Defensive Insight

Attackers often host data on local services and hide information within encoded artifacts.

Proper monitoring of internal services and validation of stored data formats can help detect suspicious activity.

---

## 💡 Skills Reinforced

* network service enumeration
* HTTP interaction
* artifact decoding
* archive extraction
* Linux investigation workflows

---

<div align="center">

🔌 Network services may expose hidden artifacts
📦 Encoded data often hides sensitive information
🧠 Investigation requires layered analysis

</div>
