# 🌐 Web Application Security Audit

This project documents a full security audit conducted on an e-commerce web application, simulating real-world penetration testing aligned with the OWASP Top 10 framework. Key findings include SQL Injection, XSS, Authentication Bypass, and IDOR vulnerabilities.

---

## 🚀 Objectives

- Identify and exploit common web security vulnerabilities
- Use automated and manual testing tools
- Provide clear remediation steps
- Align with OWASP security best practices

---

## 🔍 Vulnerabilities Found

| Vulnerability        | Risk Level | Description                                                |
|----------------------|------------|------------------------------------------------------------|
| SQL Injection        | 🔴 High     | Bypassed login using union-based SQL injection             |
| Cross-site Scripting | 🟠 Medium   | Reflected XSS in search functionality                      |
| Auth Bypass          | 🔴 High     | Weak session validation allowed forced browsing            |
| IDOR                 | 🟠 Medium   | URL manipulation revealed other users’ invoices            |

---

## 🧪 Tools & Scripts Used

- 🧰 **Burp Suite**
- 🧰 **OWASP ZAP**
- 🧰 **sqlmap**
- 🧰 **Postman**
- 🧰 **Kali Linux**
- 🐍 Custom Python/Bash scripts (see `/scripts/`)

---

## 📁 File Highlights

- `audit-report/Web_Application_Security_Audit_Report.pdf` – Full report
- `scripts/sqlmap_test.sh` – SQLi testing script
- `scripts/xss_payloads.txt` – XSS fuzzing payloads
- `screenshots/` – Evidence of discovered vulnerabilities
- `vulnerable-app/` – Optionally includes setup for DVWA or custom Laravel app

---

## ✅ Remediation Recommendations

| Issue         | Fix |
|---------------|-----|
| SQL Injection | Use parameterized queries (e.g., PDO, ORM bindings) |
| XSS           | Sanitize inputs and escape outputs contextually     |
| Auth Bypass   | Implement secure session handling + token auth      |
| IDOR          | Validate object ownership before data access        |

---

## 📎 Report & Documentation

🔗 [Download Full Audit Report (PDF)](./audit-report/Web_Application_Security_Audit_Report.pdf)

---

## ⚠️ Disclaimer

This project is for **educational and ethical purposes only**. Do not use these techniques on systems you do not own or have permission to test.

---

## 📬 Contact

Created by Muhammad Ali – Security Enthusiast  
📧 alieeestan@gmail.com
