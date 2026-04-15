# Hacktify Penetration Testing Labs 🚀

This repository contains my penetration testing reports and hands-on write-ups from the Hacktify cybersecurity labs.

## 📚 Overview

During this internship, I performed black-box security testing on vulnerable web applications and identified multiple vulnerabilities including:

* HTML Injection
* Cross-Site Scripting (XSS)
* SQL Injection (SQLi)
* Insecure Direct Object References (IDOR)
* Cross-Site Request Forgery (CSRF)
* Cross-Origin Resource Sharing (CORS)
* Capture The Flag (CTF) Challenges

## 📂 Repository Structure

* `reports/` → Original lab reports (PDFs)
* `writeups/` → Simplified vulnerability write-ups
* `screenshots/` → Proof of exploitation

## 🛠 Tools Used

* Burp Suite
* Wireshark
* Browser DevTools
* Manual Testing Techniques

## 🎯 Skills Demonstrated

* Vulnerability Identification & Exploitation
* Web Application Security Testing
* Risk Analysis & Mitigation
* Real-world Attack Simulation

## ⚠️ Disclaimer

This project is for educational purposes only. All testing was conducted in controlled lab environments.
# HTML Injection

## 🧾 Description
HTML Injection occurs when a web application fails to sanitize user input, allowing attackers to inject malicious HTML code.

## 🔍 Where it was found
Hacktify Week 1 Labs

## ⚙️ How I discovered it
Tested input fields such as search bars and file uploads with HTML tags.

## 💥 Exploitation
Example payload:
```html
<h1>Injected</h1>

---

## 📄 writeups/xss.md

```md
# Cross-Site Scripting (XSS)

## 🧾 Description
XSS allows attackers to inject malicious scripts into web pages viewed by other users.

## 🔍 Where it was found
Hacktify Week 1 Labs

## ⚙️ How I discovered it
Injected JavaScript into input fields and observed execution.

## 💥 Exploitation
```html
<script>alert('XSS')</script>

---

## 📄 writeups/sqli.md

```md
# SQL Injection

## 🧾 Description
SQL Injection allows attackers to manipulate database queries.

## 🔍 Where it was found
Hacktify Week 2 Labs

## ⚙️ How I discovered it
Tested input fields with SQL characters and observed database errors.

## 💥 Exploitation
```sql
' OR 1=1 --

---

## 📄 writeups/idor.md

```md
# Insecure Direct Object Reference (IDOR)

## 🧾 Description
IDOR occurs when applications expose internal object references without proper authorization.

## 🔍 Where it was found
Hacktify Week 2 Labs

## ⚙️ How I discovered it
Modified user ID parameters in URLs.

## 💥 Exploitation
Changed:

## ⚠️ Impact
- Unauthorized data access
- Account compromise

## 🛡️ Mitigation
- Implement access control checks
- Use indirect references
# Cross-Site Request Forgery (CSRF)

## 🧾 Description
CSRF tricks authenticated users into performing unintended actions.

## 🔍 Where it was found
Hacktify Week 3 Labs

## ⚙️ How I discovered it
Observed lack of CSRF tokens in sensitive requests.

## 💥 Exploitation
Crafted malicious request to perform actions without user consent.

## ⚠️ Impact
- Unauthorized transactions
- Account manipulation

## 🛡️ Mitigation
- Use CSRF tokens
- Validate request origin
# Cross-Origin Resource Sharing (CORS)

## 🧾 Description
Misconfigured CORS allows unauthorized domains to access sensitive data.

## 🔍 Where it was found
Hacktify Week 3 Labs

## ⚙️ How I discovered it
Tested origin headers and observed permissive responses.

## 💥 Exploitation
Set malicious origin and accessed restricted data.

## ⚠️ Impact
- Data theft
- Cross-origin attacks

## 🛡️ Mitigation
- Restrict allowed origins
- Avoid wildcard (*)# CTF Challenges

## 🧾 Description
Solved multiple web-based CTF challenges involving reconnaissance and exploitation.

## 🔍 Techniques Used
- Directory enumeration
- Base64 decoding
- Packet analysis (Wireshark)

## 💥 Example
Discovered hidden file:

Decoded Base64 to retrieve flags.

## ⚠️ Skills Demonstrated
- Reconnaissance
- Traffic analysis
- Problem-solving

---
