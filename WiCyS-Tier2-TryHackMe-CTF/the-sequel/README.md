<div align="center">

# 🧬 The Sequel  
## SQL Injection & Database Enumeration Investigation

![Category](https://img.shields.io/badge/Category-Web%20Security-orange?style=for-the-badge)
![Focus](https://img.shields.io/badge/Focus-SQL%20Injection-blue?style=for-the-badge)
![Method](https://img.shields.io/badge/Method-Query%20Manipulation-success?style=for-the-badge)

</div>

---

### 🎯 Objective

Investigate a web application suspected of being vulnerable to **SQL injection** due to improper handling of user-supplied input.

The challenge description hinted that the application did not properly sanitize database queries.

The objective was to determine whether database queries could be manipulated to extract internal information from the backend database.

---

### 🖥 Environment

| Tool | Purpose |
|-----|------|
| Web browser | Application interaction |
| Kali Linux AttackBox | Testing environment |
| Browser input fields | Injection testing |
| SQL query manipulation | Database enumeration |

---

### 📦 Step 1 — Access the Target Application

After launching the challenge machine, the web application was accessed through the provided address.

```
http://10.10.x.x:3000
```

The application contained multiple pages including a **billing section** that appeared to interact with backend database records.

📸 **Application Billing Interface**

<img src="../images/image014.png" width="600">

Because this page retrieved database information dynamically, it became the primary candidate for SQL injection testing.

---

### 🔍 Step 2 — Test Basic SQL Injection

To determine whether the application was vulnerable to SQL injection, a simple query manipulation payload was inserted into the input field.

```
1 UNION SELECT 1,2,3
```

📸 **Initial Injection Test**

<img src="../images/image015.png" width="600">

The server returned a modified response, confirming that user input was being inserted directly into the backend SQL query.

This behavior confirmed the presence of a **SQL injection vulnerability**.

---

### 🧪 Step 3 — Enumerate Database Tables

Once SQL injection was confirmed, the next step was to identify the database structure.

A query was crafted to retrieve table names from the database metadata:

```sql
1 UNION SELECT 1,table_name,3 FROM information_schema.tables
```

📸 **Database Table Enumeration**

<img src="../images/image016.png" width="600">

This query returned information about the database tables, allowing the investigation to identify potential targets containing sensitive data.

---

### 🔄 Step 4 — Identify Table Columns

After locating a table of interest, the next step was to enumerate the column names within that table.

The following query retrieved column information from the database schema:

```sql
1 UNION SELECT 1,GROUP_CONCAT(column_name),3 
FROM information_schema.columns 
WHERE table_name='flag'
```

📸 **Column Enumeration**

<img src="../images/image017.png" width="600">

This step revealed the structure of the table storing the protected data.

---

### 🔐 Step 5 — Retrieve Sensitive Data

Once the table structure was understood, the query was adjusted to retrieve the stored information from the identified column.

📸 **Database Data Retrieval**

<img src="../images/image018_redacted.png" width="600">

The application returned the contents of the protected field, confirming that the SQL injection vulnerability allowed **direct extraction of backend database data**.

---

## 🧠 Methodology Framework Applied

```
Web application access
      ↓
Input field testing
      ↓
SQL injection confirmation
      ↓
Database table enumeration
      ↓
Column structure discovery
      ↓
Sensitive data extraction
```

---

## 🛠 Techniques Used

Primary techniques used:

- SQL injection testing  
- UNION query manipulation  
- database schema enumeration  
- metadata extraction using `information_schema`  

Key concept investigated:

```
SQL Injection
```

---

## 🛡 Defensive Insight

SQL injection vulnerabilities occur when applications construct database queries using unsanitized user input.

Secure development practices include:

- parameterized queries  
- prepared statements  
- input validation and sanitization  
- restricting database permissions  

Proper query handling prevents attackers from manipulating database commands and extracting sensitive information.

---

## 💡 Skills Reinforced

- Web application vulnerability testing  
- SQL injection identification  
- Database enumeration techniques  
- Query manipulation and schema discovery  
- Secure database interaction awareness  

---

<div align="center">

🧬 Test how applications build database queries  
🔍 Enumerate database structure methodically  
🔐 SQL injection can expose entire databases  

</div>
