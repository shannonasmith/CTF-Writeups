<div align="center">

# 🧩 wm01 — Arrays in JavaScript  
## Client-Side Logic Analysis & Front-End Validation

![Category](https://img.shields.io/badge/Category-Web%20Security-green?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-JavaScript%20Logic-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Client%20Side%20Analysis-orange?style=for-the-badge)

</div>

---

## 🎯 Objective

Analyze a web application that uses JavaScript arrays to control application behavior.

The goal of the challenge was to identify how client-side logic was implemented and determine whether the validation mechanism could be manipulated.

This exercise focused on understanding **how front-end logic can be inspected and altered by an attacker**.

---

## 🖥 Environment

- Web browser  
- Browser Developer Tools  
- JavaScript console inspection  
- Source code review  

---

## 🔎 Step 1 — Initial Page Inspection

The application presented a web interface requiring interaction before revealing additional content.

Initial observations included:

- Client-side scripts handling page behavior  
- No immediate visible flag or hidden content  
- JavaScript controlling validation logic  

This indicated that the solution likely involved analyzing the **browser-executed code**.

---

## 🔍 Step 2 — Inspect Client-Side JavaScript

Opened **Developer Tools** and inspected the loaded JavaScript files.

Key findings:

- Arrays defined within the script
- Conditional logic referencing those arrays
- Validation performed entirely in the browser

Because JavaScript runs on the client side, its logic is fully visible and modifiable by anyone using Developer Tools.

---

## 🧪 Step 3 — Analyze Array-Based Logic

The script relied on arrays to control program flow.

This type of design often appears in beginner challenges because arrays can be used to:

- store validation values
- check input sequences
- control conditional branching

By analyzing how the array values were referenced within the code, it became possible to understand how the page determined valid outcomes.

---

## 🔄 Step 4 — Evaluate Trust Boundaries

Since the validation logic occurred entirely in the browser, it was subject to manipulation.

Important observations:

- The server was not performing validation
- All logic ran in client-side JavaScript
- Browser tools allowed full inspection of the logic

This meant that the challenge could be solved by understanding and manipulating the client-side code.

---

## 🧠 Methodology Framework Applied

1. Load the application
2. Inspect page source
3. Identify JavaScript dependencies
4. Review array definitions
5. Analyze validation logic
6. Understand client-side trust boundary
7. Derive correct application behavior

---

## 🛡 Defensive Insight

This challenge highlights a common security mistake:

> **Client-side validation should never be trusted as a security control.**

Because users control the browser environment, they can:

- modify JavaScript
- bypass validation
- manipulate application state

Secure applications must enforce validation **server-side**.

---

## 💡 Skills Reinforced

- Browser Developer Tools usage  
- JavaScript source inspection  
- Client-side logic analysis  
- Understanding trust boundaries in web applications  
- Recognizing insecure front-end validation patterns  

---

<div align="center">

🌐 Inspect the client  
🔎 Understand the logic  
🛡 Never trust the browser  

</div>
