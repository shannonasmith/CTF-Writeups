<div align="center">

# 🌐 we01 — Hidden Web Content  
## Web Enumeration & Unlinked Resource Discovery

![Category](https://img.shields.io/badge/Category-Web%20Security-green?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-Enumeration%20%7C%20Source%20Inspection-blue?style=for-the-badge)

</div>

---

## 🎯 Objective

Identify hidden or unlinked content on a publicly accessible website.

The challenge title suggested that not all resources would be reachable through visible navigation.

---

## 🖥 Environment

- Web browser
- Developer Tools (View Source / Elements)
- Manual enumeration techniques
- External research on URL fuzzing concepts

---

## 🔎 Initial Observation

Upon loading the target site:

- No obvious flag or sensitive content visible
- Navigation appeared minimal
- No suspicious visible links

Initial hypothesis:  
The content is accessible via an unlinked resource.

---

## 🧭 Investigation Workflow

### 1️⃣ Manual Review of Visible Content

- Reviewed page structure
- Checked hyperlinks
- Looked for hidden UI elements
- Confirmed no obvious exposure

---

### 2️⃣ Source Code Inspection

Opened Developer Tools and reviewed:

- HTML structure
- Comments
- Referenced paths
- Hidden endpoints

Purpose:
Identify directories or resources not linked in the UI.

---

### 3️⃣ Research Enumeration Techniques

Opened external resources to review:

- URL fuzzing concepts
- Directory discovery methodology
- Hidden file enumeration patterns

This was not automated brute forcing —  
it was conceptual research to guide manual testing.

---

### 4️⃣ Manual Path Exploration

Using insight from:

- Source inspection
- Naming conventions
- Common directory structures

Tested alternative paths directly in the browser address bar.

---

## 🚪 Discovery

Located an unlinked page containing sensitive content.

The resource was:

- Not accessible via visible navigation
- Not linked directly on the homepage
- Reachable only through manual path discovery

---

## 🧠 Key Concepts Reinforced

- Not all web content is linked in UI navigation  
- Source inspection often reveals structural hints  
- Enumeration is often logical, not brute force  
- Research-driven pivoting improves efficiency  

---

## 🛡 Defensive Implications

- Sensitive files must not rely on obscurity  
- Unlinked ≠ inaccessible  
- Access control must be enforced server-side  

---

<div align="center">

🔎 Enumerate.  
🧭 Pivot.  
🛡️ Validate assumptions.

</div>
