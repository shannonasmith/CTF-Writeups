<div align="center">

# 🔑 Get Admin  
## Authentication Logic Analysis & Session Manipulation

![Category](https://img.shields.io/badge/Category-Web%20Security-green?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Authentication%20Logic-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Session%20Manipulation-orange?style=for-the-badge)

</div>

---

## 🎯 Objective

Investigate a web application that restricts administrative functionality behind an authentication boundary.

The goal of the challenge was to determine whether the application’s access control mechanisms could be bypassed through analysis of client-side behavior.

This challenge focused on understanding how **session data and client-side controls influence authorization decisions**.

---

## 🖥 Environment

- Web browser  
- Browser Developer Tools  
- Application storage inspection  
- Cookie analysis  

---

## 🔎 Step 1 — Initial Application Exploration

The application presented a typical login interface that differentiated between regular users and administrators.

Initial observations:

- Standard login workflow
- Restricted administrative functionality
- No visible path to obtain administrative access

The working hypothesis was that administrative access was controlled through **client-visible session data**.

---

## 🔍 Step 2 — Inspect Application Storage

Opened **Developer Tools** and inspected the browser storage areas:

- Cookies
- Local storage
- Session storage

Modern web applications often store session indicators or user roles within these storage mechanisms.

During inspection, key session-related values were identified that appeared to influence authorization behavior.

---

## 🧪 Step 3 — Analyze Client-Side Authorization Behavior

Further investigation revealed that the application relied on **client-visible indicators** to determine whether a user had administrative privileges.

This meant that authorization decisions were partially dependent on data controlled by the browser.

Because client-side data can be modified, this created a potential pathway to escalate privileges.

---

## 🔄 Step 4 — Manipulate Session Context

Using Developer Tools, session-related values were modified to evaluate how the application responded.

By altering these indicators, it became possible to observe changes in the application's authorization behavior.

This demonstrated that administrative privileges were being determined by **client-controlled data rather than server-side validation**.

---

## 🧠 Methodology Framework Applied

1. Explore application interface  
2. Identify restricted functionality  
3. Inspect browser storage mechanisms  
4. Analyze session indicators  
5. Evaluate trust boundaries  
6. Manipulate client-side state  
7. Observe authorization changes  

---

## 🛡 Defensive Insight

This challenge highlights a critical web security principle:

> **Authorization decisions must never rely solely on client-controlled data.**

If role information is stored or trusted in the browser without server validation, attackers can manipulate that data to escalate privileges.

Secure applications must enforce authorization **server-side**, with client data treated only as informational.

---

## 💡 Skills Reinforced

- Browser Developer Tools analysis  
- Session and cookie inspection  
- Understanding authentication vs authorization  
- Identifying client-side trust vulnerabilities  
- Analyzing insecure web application design  

---

<div align="center">

🔎 Inspect the session  
🧠 Understand the trust boundary  
🛡 Authorization belongs on the server  

</div>
