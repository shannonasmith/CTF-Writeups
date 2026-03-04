<div align="center">

# 🌐 Endpoint  
## Web Endpoint Discovery & Information Disclosure

![Category](https://img.shields.io/badge/Category-Web%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Endpoint%20Discovery-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Web%20Enumeration-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Identify a hidden or undocumented web endpoint that exposes sensitive information or functionality.

The challenge required analyzing how web applications structure resources and discovering endpoints that are not directly visible through normal navigation.

This exercise focused on **web enumeration and resource discovery**.

---

## 🖥 Environment

- Web browser
- Developer Tools (browser inspection)
- Manual URL manipulation
- Basic web enumeration techniques

---

## 🔍 Step 1 — Initial Site Inspection

The investigation began by loading the provided web application and observing its visible functionality.

Initial exploration included:

- Interacting with available page elements
- Observing page behavior
- Inspecting any visible input fields or links

At this stage, no obvious sensitive functionality was exposed.

---

## 🔎 Step 2 — Inspect Client-Side Code

Using browser developer tools, the page source and loaded resources were examined.

This step included:

- Reviewing HTML source
- Checking linked JavaScript files
- Inspecting embedded comments
- Identifying potential references to backend routes

Client-side code often reveals hidden endpoints used by the application.

---

## 🔄 Step 3 — Endpoint Enumeration

Based on patterns observed in the application, the next step was to test potential backend endpoints manually.

This involved:

- Modifying URL paths
- Testing alternative routes
- Exploring common endpoint naming conventions

Enumeration techniques often reveal functionality not exposed through the user interface.

---

## 🔐 Step 4 — Identify Hidden Endpoint

Through manual enumeration and inspection of application structure, a hidden endpoint was discovered.

This endpoint exposed functionality or information that was not accessible through the normal navigation flow of the site.

This confirmed the presence of **improper access control or endpoint exposure**.

---

# 🧠 Methodology Framework Applied

1. Observe application behavior  
2. Inspect client-side code  
3. Identify patterns in resource structure  
4. Enumerate potential endpoints  
5. Validate endpoint responses  
6. Confirm exposed functionality  

---

# 🛡 Defensive Insight

Hidden endpoints are a common source of vulnerabilities when:

- Developers assume endpoints cannot be discovered
- Sensitive functionality is not properly restricted
- Authorization checks rely on obscurity rather than enforcement

Security testing must always include **endpoint enumeration** in addition to visible UI testing.

---

# 💡 Skills Reinforced

- Web application reconnaissance  
- Client-side code inspection  
- Manual endpoint enumeration  
- Resource discovery techniques  
- Understanding of insecure endpoint exposure  

---

<div align="center">

🌐 Enumerate what the interface hides  
🔎 Inspect the code behind the page  
🧠 Never trust that hidden means protected  

</div>
