<div align="center">

# 💉 The Sequel  
## SQL Injection & Database Query Manipulation

![Category](https://img.shields.io/badge/Category-Web%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-SQL%20Injection-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Input%20Manipulation-success?style=for-the-badge)

</div>

---

## 🎯 Objective

Investigate a web application that accepts user input and determine whether it improperly interacts with a backend database.

The challenge required analyzing how user-supplied data was processed and identifying whether the application was vulnerable to **SQL injection attacks**.

The goal was to manipulate the application's database query logic in order to bypass normal restrictions.

---

## 🖥 Environment

- Web browser  
- Browser developer tools  
- Manual input testing  
- SQL injection payload experimentation  

---

## 🔍 Step 1 — Analyze Application Input Fields

The investigation began by interacting with the application's input fields.

Initial testing focused on:

- Observing how user input was processed  
- Determining whether errors occurred when special characters were used  
- Identifying how the application responded to unexpected input  

Web applications that directly incorporate user input into database queries are often vulnerable to injection attacks.

---

## 🔎 Step 2 — Test for Injection Behavior

Input fields were tested using characters commonly associated with SQL syntax, including:

- quotation marks
- logical operators
- comment characters

The application's responses indicated that user input was being incorporated into a backend query without proper sanitization.

This suggested that the application was vulnerable to **SQL query manipulation**.

---

## 🔄 Step 3 — Manipulate Query Logic

By carefully modifying the structure of the input, it became possible to alter the logic of the underlying SQL query.

Instead of returning results based strictly on the intended query conditions, the manipulated input caused the database to evaluate a different logical expression.

This allowed the application to return results that would normally be restricted.

---

## 🔐 Step 4 — Confirm Database Manipulation

Further testing confirmed that the input was successfully influencing the database query.

This demonstrated that:

- Input validation was insufficient
- Queries were likely constructed dynamically
- The database logic could be altered through crafted input

This confirmed the presence of a **classic SQL injection vulnerability**.

---

# 🧠 Methodology Framework Applied

1. Identify application input points  
2. Test special character handling  
3. Observe application response patterns  
4. Introduce structured query manipulation input  
5. Evaluate altered database behavior  
6. Confirm injection vulnerability  

---

# 🛡 Defensive Insight

SQL injection vulnerabilities occur when user input is incorporated into database queries without proper sanitization or parameterization.

Secure application design should include:

- Parameterized queries  
- Prepared statements  
- Strict input validation  
- Database query separation from user input  

Failure to implement these protections allows attackers to manipulate database queries and retrieve unauthorized data.

---

# 💡 Skills Reinforced

- Web application vulnerability testing  
- SQL injection detection techniques  
- Database query logic analysis  
- Input validation assessment  
- Application response pattern analysis  

---

<div align="center">

💉 User input should never control database queries  
🔎 Observe how applications interpret unexpected input  
🧠 Secure applications separate logic from data  

</div>
