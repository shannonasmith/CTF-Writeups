<div align="center">

# 📝 Notepad Online  
## Authorization Logic Analysis & Direct Object Reference Investigation

![Category](https://img.shields.io/badge/Category-Web%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Authorization%20Control-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Parameter%20Manipulation-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a web-based note-taking service that claims user notes are visible **only to the account owner**.

The challenge required analyzing how the application retrieves user notes and determining whether access controls were properly enforced.

The goal was to determine whether **direct object references within the application could expose other users’ data**.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Web browser | Application interaction |
| Browser address bar | Parameter manipulation |
| Manual testing | Authorization validation |
| Application observation | Access control behavior |

---

### 📦 Step 1 — Access the Notepad Application

The investigation began by accessing the provided web application and logging in using the supplied credentials.

📸 **Application Login Interface**

<img src="../images/image008.png" width="600">

After authentication, the application displayed the user’s personal notes within the interface.

The application appeared to assign notes based on a **numeric identifier present in the page URL**.

---

### 🔍 Step 2 — Inspect URL Parameters

Closer inspection of the browser address bar revealed that the application used a query parameter similar to:

```
?id=1
```

📸 **Observed URL Parameter**

<img src="../images/image009.png" width="600">

This suggested that the application retrieved note data by referencing an **internal numeric identifier**.

Applications that directly expose internal identifiers can sometimes allow users to **access other resources by modifying the parameter value**.

---

### 🧪 Step 3 — Test Parameter Manipulation

To test whether the application properly enforced authorization controls, the numeric identifier was modified manually.

The parameter value was changed to a different number to observe how the application responded.

📸 **Modified Identifier**

<img src="../images/image010.png" width="600">

The application responded by displaying a different note resource, indicating that the system retrieved data solely based on the identifier provided in the request.

---

#### 🔎 Analytical Observation

This behavior indicates a classic **Insecure Direct Object Reference (IDOR)** vulnerability.

IDOR occurs when:

- applications reference internal objects directly
- authorization checks are missing or insufficient
- users can access resources by altering identifiers

Instead of verifying ownership of the requested object, the application simply returned the resource associated with the provided identifier.

---

### 🔄 Step 4 — Analyze Application Response

The modified request returned a different note stored on the system.

This confirmed that the application allowed users to **access resources that were not associated with their account**.

The vulnerability occurred because the server did not validate whether the requesting user was authorized to access the specified resource.

---

### 🔐 Step 5 — Confirm Unauthorized Data Access

Once the parameter manipulation was verified, the application displayed a protected resource that should not have been accessible.

📸 **Unauthorized Note Access**

<img src="../images/image011_redacted.png" width="600">

This confirmed that the application was vulnerable to **Insecure Direct Object Reference**, allowing unauthorized access to internal data through simple parameter manipulation.

---

## 🧠 Methodology Framework Applied

```
Application login
      ↓
URL parameter inspection
      ↓
Identifier discovery
      ↓
Parameter manipulation
      ↓
Unauthorized resource access
      ↓
Access control vulnerability confirmed
```

---

## 🛠 Techniques Used

Primary techniques used:

- application interface inspection  
- URL parameter analysis  
- manual parameter manipulation  
- authorization testing  

Key concept investigated:

```
Insecure Direct Object Reference (IDOR)
```

---

## 🛡 Defensive Insight

Applications must enforce **server-side authorization checks** whenever resources are requested.

If identifiers are exposed within URLs, the server must verify that the authenticated user is permitted to access the requested object.

Recommended security practices include:

- validating object ownership on the server  
- implementing proper access control checks  
- avoiding predictable sequential identifiers  
- logging and monitoring suspicious access attempts  

Without proper authorization validation, attackers can enumerate identifiers to access sensitive data belonging to other users.

---

## 💡 Skills Reinforced

- Web application reconnaissance  
- Authorization control analysis  
- URL parameter manipulation  
- Identification of IDOR vulnerabilities  
- Understanding insecure direct object references  

---

<div align="center">

🔍 Always test how applications reference internal objects  
🧠 Authorization must be enforced server-side  
🔐 Never trust identifiers supplied by the client  

</div>
