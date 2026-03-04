<div align="center">

# 📝 Notepad Online  
## Web Application Logic & Client-Side Trust Analysis

![Category](https://img.shields.io/badge/Category-Web%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Client--Side%20Logic-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Application%20Inspection-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze the functionality of an online note-taking application to determine whether sensitive operations rely on insecure client-side logic.

The challenge required inspecting how the application handled user input and identifying whether security decisions were enforced by the client rather than the server.

The goal was to understand how **client-side trust assumptions can expose application vulnerabilities**.

---

## 🖥 Environment

- Web browser  
- Browser Developer Tools  
- HTML and JavaScript inspection  
- Manual request interaction  

---

## 🔍 Step 1 — Initial Application Exploration

The investigation began by interacting with the online notepad interface.

Initial observations included:

- Ability to create and modify notes
- Client-side rendering of note content
- Minimal server-side interaction visible through the interface

At first glance, the application appeared to behave like a simple front-end note editor.

---

## 🔎 Step 2 — Inspect Client-Side Code

Using browser developer tools, the page source and associated JavaScript were examined.

Key inspection areas included:

- Client-side validation logic
- JavaScript functions controlling note actions
- Any hidden parameters or variables controlling behavior

Client-side scripts often reveal assumptions about user permissions or system behavior.

---

## 🔄 Step 3 — Identify Client-Side Trust Model

Review of the JavaScript logic revealed that certain application behavior depended entirely on client-side conditions.

This suggested that:

- The application trusted values provided by the browser
- Authorization or validation checks might occur only in JavaScript

Applications relying on client-side checks can often be manipulated by modifying the application state locally.

---

## 🔐 Step 4 — Manipulate Client-Side State

By altering values or logic within the browser environment, it was possible to bypass the application's intended restrictions.

This confirmed that the application relied on **client-side enforcement rather than server-side validation**.

As a result, sensitive functionality could be triggered by manipulating the browser environment.

---

# 🧠 Methodology Framework Applied

1. Interact with application features  
2. Inspect HTML and JavaScript resources  
3. Identify validation and logic controls  
4. Determine whether checks occur client-side or server-side  
5. Modify client-side variables or conditions  
6. Observe resulting behavior  

---

# 🛡 Defensive Insight

Applications must never rely solely on client-side logic to enforce security decisions.

Client-side controls are easily bypassed because users have full control over their browser environment.

Proper application security requires:

- Server-side validation  
- Authorization enforcement on the backend  
- Client-side logic used only for usability, not security  

---

# 💡 Skills Reinforced

- Web application reconnaissance  
- JavaScript logic inspection  
- Client-side trust model analysis  
- Browser developer tool usage  
- Identification of insecure validation patterns  

---

<div align="center">

📝 Inspect the logic behind the interface  
🔎 Client-side code is always visible to attackers  
🧠 Security must be enforced on the server  

</div>
