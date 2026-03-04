# Bruteforce Me

## Challenge Overview

This challenge presents a login portal where the user has forgotten their credentials. The challenge description suggests the username may be one of the following:

```
pedro
admin
root
```

The objective is to discover valid login credentials and retrieve the flag.

This exercise demonstrates the risks associated with weak authentication controls and the importance of rate limiting and credential protection.

---

## Environment

Attack platform:

```
TryHackMe AttackBox
```

Target:

```
Web login service running on the target machine
```

Primary tools used:

```
hydra
curl
browser developer tools
```

---

## Initial Enumeration

After the machine started, the first step was to identify how authentication was handled.

Opening the login page revealed a standard form with username and password fields.

Before attempting brute force attacks, it is important to determine:

- login endpoint  
- request method  
- failure message  

Using browser developer tools confirmed the form submission used an HTTP POST request.

---

## Credential Brute Force

Because the challenge hints provided possible usernames, the attack focused on brute forcing the password.

Hydra was used with the **rockyou password list**.

Example command:

```bash
hydra -l pedro -P /usr/share/wordlists/rockyou.txt <TARGET_IP> http-post-form \
"/login:username=^USER^&password=^PASS^:F=incorrect"
```

Explanation:

```
-l pedro
specific username

-P rockyou.txt
password dictionary

http-post-form
brute forcing a web login form

F=incorrect
string returned when login fails
```

Hydra iterated through the password list until valid credentials were identified.

---

## Successful Login

Once the correct credentials were discovered, authentication succeeded and access to the application was granted.

After logging in, the application displayed the challenge flag.

```
THM{REDACTED}
```

*(Flags are redacted in this repository to avoid spoilers.)*

---

## Key Concepts Demonstrated

Credential brute forcing relies on testing large numbers of passwords against an authentication interface.

This challenge highlights several common security weaknesses:

- weak passwords  
- lack of login attempt limits  
- missing account lockout protections  

Without these protections, automated tools can compromise accounts quickly.

---

## Security Lessons

Organizations should implement protections against brute force attacks, including:

- account lockout after repeated failures  
- CAPTCHA protections  
- multi-factor authentication  
- monitoring for abnormal login attempts  
- strong password policies  

These measures significantly reduce the risk of automated credential attacks.

---

## Skills Demonstrated

- Web authentication analysis  
- Password brute forcing  
- Hydra usage  
- Understanding login request structure  
- Security control awareness  

---

## Next Challenge

➡️ **Endpoint**
