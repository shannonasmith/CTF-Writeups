<div align="center">

# 🔐 Bruteforce Me  
## Authentication Weakness & Credential Attack Analysis

![Category](https://img.shields.io/badge/Category-Web%20Exploitation-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Credential%20Bruteforce-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Automated%20Enumeration-success?style=for-the-badge)
![Tool](https://img.shields.io/badge/Tool-Hydra%20(Kali%20Linux)-black?style=for-the-badge&logo=kalilinux)

<img src="https://www.kali.org/tools/hydra/images/hydra-logo.svg" width="120"/>

</div>

---

## 🎯 Objective

Access a protected login portal by identifying valid credentials.

The challenge description suggested the possible usernames:

```
pedro
admin
root
```

The goal was to determine the correct password and retrieve the flag.

This challenge demonstrates the risks associated with **weak authentication controls and password reuse**.

---

## 🖥 Environment

- TryHackMe AttackBox  
- Kali Linux tooling  
- Web browser  
- Hydra password brute-force tool  
- RockYou password list  

---

## 🔍 Step 1 — Initial Reconnaissance

After launching the target machine, the login page was inspected through a browser.

Observations:

- Standard username/password form
- Login request sent via **HTTP POST**
- Authentication error message returned when credentials failed

Understanding the **request structure** was necessary before attempting automated attacks.

---

## 🧪 Step 2 — Identify Attack Strategy

Because the challenge hinted at possible usernames, the attack focused on **password discovery rather than username enumeration**.

Brute forcing was selected as the most efficient approach.

Primary tool used:

```
Hydra
```

Hydra is a widely used credential attack tool included in **Kali Linux**.

---

## ⚙ Step 3 — Execute Credential Brute Force

Using the RockYou password list, Hydra was configured to test passwords against the login form.

Example command:

```bash
hydra -l pedro -P /usr/share/wordlists/rockyou.txt <TARGET_IP> http-post-form \
"/login:username=^USER^&password=^PASS^:F=incorrect"
```

### Command Breakdown

```
-l pedro
Specified username

-P rockyou.txt
Password dictionary

http-post-form
Indicates the target is a web login form

F=incorrect
Failure condition returned by the application
```

Hydra iterated through the password list until valid credentials were discovered.

---

## 🔓 Step 4 — Successful Authentication

Once the correct credentials were identified, authentication succeeded and the application granted access to the protected area.

The challenge flag was then visible within the authenticated page.

```
THM{REDACTED}
```

*(Flags are intentionally redacted in this repository to avoid spoilers.)*

---

# 🧠 Methodology Framework Applied

1. Identify authentication interface  
2. Inspect login request behavior  
3. Determine attack feasibility  
4. Select brute-force strategy  
5. Automate password testing  
6. Validate successful authentication  

---

# 🛡 Defensive Insight

Brute-force attacks remain one of the most common authentication threats.

This challenge reinforces the importance of implementing protective controls such as:

- login rate limiting  
- account lockout policies  
- multi-factor authentication  
- password complexity requirements  

Without these protections, automated credential attacks can compromise accounts quickly.

---

# 💡 Skills Reinforced

- Web authentication analysis  
- Credential brute-force methodology  
- Hydra tool usage  
- Login request inspection  
- Security control awareness  

---

<div align="center">

🔐 Protect authentication endpoints  
⚙ Automate repetitive testing  
🧠 Validate assumptions with evidence  

</div>
