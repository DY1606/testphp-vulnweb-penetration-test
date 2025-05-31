# 🛡️ Penetration Testing Report – testphp.vulnweb.com

## 📘 Overview
This project presents a full-scale penetration test on the intentionally vulnerable website `testphp.vulnweb.com`, conducted as part of a cybersecurity course and submitted to **Embrizon Technology**. The test simulates real-world web attacks using professional tools and demonstrates exploitation of common web application vulnerabilities.

## 📆 Date
March 31, 2025

## 🙋 Submitted By
**Yendluri Dinesh**  
Cybersecurity Student | Ethical Hacking Enthusiast  
Course Project Submission – Embrizon Technology

## 🧠 Objectives
- Identify vulnerabilities in a controlled testing environment
- Exploit and demonstrate real-world attack techniques
- Provide risk assessment and mitigation strategies

## 🛠️ Tools Used
- SQLmap - Automated SQL injection testing
- Burp Suite - Manual web application testing & proxy
- Nmap - Port scanning & OS detection
- Gobuster - Directory and file enumeration
- Nikto - Web server vulnerability scanner
- Curl - Server header and version info extraction

📄 [Download `tools_used.pdf`](./tools_used.pdf)

## 🔍 Vulnerabilities Discovered

| Vulnerability              | Risk Level | Description                                     |
|---------------------------|------------|-------------------------------------------------|
| SQL Injection (SQLi)      | High       | Extracted database credentials via injection    |
| Cross-Site Scripting (XSS)| High       | Executed malicious JavaScript via guestbook     |
| CSRF                      | Medium     | Performed actions on behalf of authenticated users |
| Open Directory Listing    | Medium     | Exposed internal files like `create.sql`        |
| Outdated Software         | High       | Detected old PHP/Nginx versions                 |
| Directory Enumeration     | Medium     | Found hidden directories using Gobuster         |
| Server Misconfiguration   | Medium     | Missing headers: CSP, X-Frame-Options, etc.     |
| Open Ports and Services   | Medium     | Found via Nmap; services exposed unnecessarily   |

## 📎 Project Files
- 📄 [`final_penetration_testing_report.pdf`](./xyz_company_penetration_testing.pdf) – Full report with disclaimer
- 📄 [`tools_used.pdf`](./tools_used.pdf) – Tools used in the assessment
- 📁 `/screenshots/` – Proof of concept images for each vulnerability

## 📸 Sample Screenshots
Screenshots include:
- SQL Injection revealing DB structure
- Stored XSS popup executed in guestbook
- CSRF attack form and successful exploit
- Open directory files like `create.sql`
- Gobuster and Nmap scans
- Missing security headers via cURL

## 🎓 Academic Context
This project was conducted as a part of a **cybersecurity course** and submitted to **Embrizon Technology** for academic evaluation. It reflects practical knowledge in ethical hacking and secure web application testing.

## ⚠️ Legal Disclaimer
> This penetration test was conducted in a **controlled lab environment** using an **intentionally vulnerable** target (`testphp.vulnweb.com`). It was performed **solely for educational and ethical purposes**. No real systems were harmed or accessed during this assessment.
