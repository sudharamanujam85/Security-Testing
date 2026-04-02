# 🔐 Security Testing

> A hands-on cybersecurity portfolio covering web application penetration testing,
> cloud-based Kali Linux lab setup, and authorized social engineering simulation —
> built using industry-standard tools and ethical hacking methodology.

[![Burp Suite](https://img.shields.io/badge/Tool-Burp%20Suite-orange?style=flat-square)](https://portswigger.net/burp)
[![OWASP ZAP](https://img.shields.io/badge/Tool-OWASP%20ZAP-blue?style=flat-square)](https://www.zaproxy.org)
[![Kali Linux](https://img.shields.io/badge/OS-Kali%20Linux-557C94?style=flat-square&logo=kalilinux)](https://www.kali.org)
[![AWS](https://img.shields.io/badge/Cloud-AWS%20EC2-FF9900?style=flat-square&logo=amazonaws)](https://aws.amazon.com)
[![Ethical Hacking](https://img.shields.io/badge/Domain-Ethical%20Hacking-red?style=flat-square)]()
[![OWASP Top 10](https://img.shields.io/badge/Standard-OWASP%20Top%2010-green?style=flat-square)]()

> ⚠️ **Ethical Use Only** — All techniques documented here are strictly for authorized penetration testing, cybersecurity research, and security awareness training. Never use these techniques on systems you do not own or have explicit written permission to test.

---

## 📌 Project Overview

This repository contains four detailed, step-by-step security testing manuals that demonstrate practical, hands-on proficiency with the tools and techniques used by professional penetration testers and security QA engineers.

The documents cover:
- **Web application security testing** using the two most widely used industry tools
- **Cloud-based penetration testing lab setup** on AWS
- **Authorized social engineering simulation** using phishing frameworks

All testing was performed in controlled, authorized lab environments against intentionally vulnerable applications.

---

## 📂 Repository Contents

| Document | Description |
|---|---|
| 📄 **Burp Suite Manual.docx** | Step-by-step web application security testing using Burp Suite — proxy interception, SQL injection, XSS, brute force, session analysis |
| ☁️ **Creating_AWS_Instance_KaliLinux Server.docx** | Deploy a Kali Linux server on AWS EC2, configure SSH access, deploy a vulnerable web app target, and manage cloud services |
| 🟢 **OWASP ZAP MANUAL.docx** | Web application security testing using OWASP ZAP — active/passive scanning, spidering, fuzzing, and CI/CD integration |
| ⚠️ **Phishing Using Zphisher and URL Masking with Facad1ng.docx** | Authorized phishing simulation using Zphisher and URL masking with Facad1ng in a Kali Linux environment |

---

## 🛠️ Tools & Technologies

| Tool | Category | Purpose |
|---|---|---|
| **Burp Suite** | Web App Security | Proxy, Repeater, Intruder, Scanner — manual penetration testing |
| **OWASP ZAP** | Web App Security | Open-source automated security scanning; CI/CD integration |
| **Kali Linux** | Operating System | Industry-standard ethical hacking OS — all tools run here |
| **AWS EC2** | Cloud Infrastructure | Cloud-based penetration testing lab environment |
| **Ngrok / Cloudflared** | Tunnelling | Expose local services to public URLs for phishing simulation |
| **Zphisher** | Social Engineering | Phishing page generation for authorized awareness testing |
| **Facad1ng** | URL Masking | URL masking for authorized phishing simulation campaigns |
| **DVWA** | Target Application | Damn Vulnerable Web App — intentionally vulnerable legal test target |

---

## 📖 Document Summaries

### 🔴 1. Burp Suite Manual

Burp Suite is the world's leading web application penetration testing platform. This manual covers:

- **Proxy setup** — configuring browser to route traffic through Burp; installing CA certificate for HTTPS interception
- **Intercepting & modifying requests** — capturing live HTTP/HTTPS traffic and manipulating parameters, headers, and cookies
- **Repeater** — manually replaying and modifying individual requests to test server responses
- **Intruder** — automated fuzzing and brute-force attacks using wordlists; Sniper and Cluster Bomb attack modes
- **SQL Injection testing** — injecting payloads into form fields, URL parameters, and HTTP headers
- **Cross-Site Scripting (XSS)** — reflected and stored XSS detection through payload injection
- **Session Token Analysis** — using Sequencer to measure entropy and detect weak session identifiers
- **Decoder** — encoding/decoding Base64, URL, HTML, and Hex payloads
- **OWASP Top 10 coverage** — practical testing for all 10 critical web application risk categories

---

### ☁️ 2. Creating an AWS Kali Linux Penetration Testing Lab

This guide covers building a professional cloud-based security testing environment:

- **AWS account & IAM setup** — configuring permissions and billing alerts
- **EC2 instance launch** — selecting Kali Linux AMI; choosing appropriate instance type
- **Security Group configuration** — restricting SSH access to authorized IPs only
- **Key pair & SSH access** — generating RSA key pairs; connecting securely via terminal
- **Elastic IP assignment** — ensuring a persistent public IP across reboots
- **Target application deployment** — installing DVWA as a legal, intentionally vulnerable test target
- **Service management** — starting/stopping Apache and MySQL; managing instance lifecycle to control costs

---

### 🟢 3. OWASP ZAP Manual

OWASP ZAP (Zed Attack Proxy) is the world's most widely used open-source web security tool. This manual covers:

- **Passive scanning** — monitoring traffic without sending attack requests; zero-disruption detection
- **Active scanning** — sending crafted attack payloads to identify vulnerabilities automatically
- **Spider** — crawling the target application to map all URLs, forms, and endpoints
- **Ajax Spider** — extending crawling to JavaScript-heavy single-page applications (SPAs)
- **Fuzzer** — injecting custom payloads into request parameters
- **Break Points** — intercepting and modifying HTTP requests in real-time
- **Alerts dashboard** — triaging findings by severity (High / Medium / Low / Informational)
- **Report generation** — producing HTML, XML, and JSON security reports for stakeholders
- **CI/CD integration** — using ZAP's Docker image and GitHub Actions for automated pipeline security scanning

**OWASP Top 10 vulnerabilities tested with ZAP:**
- A01 Broken Access Control
- A02 Cryptographic Failures
- A03 Injection (SQL, XSS, Command)
- A05 Security Misconfiguration
- A07 Authentication Failures
- A09 Security Logging & Monitoring Failures

---

### ⚠️ 4. Phishing Simulation — Zphisher & Facad1ng

> 🔒 **Authorization Required** — This guide is for authorized penetration testing and security awareness training **only**. A signed Rules of Engagement (RoE) document must be obtained before conducting any phishing simulation.

This manual covers an end-to-end authorized phishing simulation workflow:

- **Zphisher** — open-source phishing framework for generating convincing login page clones inside Kali Linux
- **Ngrok / Cloudflared tunnelling** — exposing the local phishing page on a publicly accessible URL
- **Facad1ng URL masking** — wrapping the tunnel URL behind a more convincing domain to simulate real-world phishing techniques
- **Credential capture** — monitoring captured submissions in real-time during authorized testing
- **Reporting** — compiling click rates, credential submission rates, and time-to-click metrics into a security assessment report
- **Security awareness recommendations** — translating simulation results into actionable training plans

**Simulation workflow:**
```
Authorization obtained → Launch Kali on AWS → Run Zphisher → Start Ngrok tunnel
→ Apply Facad1ng URL masking → Send phishing email (authorized) → Monitor captures → Report findings
```

---

## 🎯 Skills Demonstrated

### Technical
- Web application penetration testing (manual + automated)
- OWASP Top 10 vulnerability identification and exploitation
- HTTP proxy interception and traffic manipulation
- SQL injection, XSS, brute force, and session analysis
- Cloud lab setup and management (AWS EC2, Kali Linux)
- Authorized phishing simulation and social engineering methodology
- Linux command line proficiency
- Security report writing and findings documentation

### Professional
- Ethical hacking methodology: Reconnaissance → Scanning → Exploitation → Reporting
- Scope and authorization discipline — understanding legal boundaries in security testing
- Tool selection judgement — right tool for each testing scenario
- Clear technical documentation across four detailed step-by-step manuals

---

## 🔗 Key Security Standards Referenced

- [OWASP Top 10](https://owasp.org/www-project-top-ten/) — most critical web application security risks
- [PTES (Penetration Testing Execution Standard)](http://www.pentest-standard.org/) — structured pen testing methodology
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework) — identify, protect, detect, respond, recover

---

## ⚖️ Ethical & Legal Disclaimer

All techniques, tools, and workflows documented in this repository are intended **strictly** for:

- ✅ Authorized penetration testing with written client permission
- ✅ Cybersecurity research in controlled lab environments
- ✅ Security awareness training within organizations
- ✅ Educational and portfolio demonstration purposes

**Never use these techniques against systems you do not own or do not have explicit written authorization to test.** Unauthorized use may violate computer misuse laws including the Computer Fraud and Abuse Act (CFAA), the UK Computer Misuse Act, and equivalent legislation in other jurisdictions.

---

## 👩‍💻 About

Built by **Sudha** — transitioning into cybersecurity and QA automation with 20+ years of professional experience.

This portfolio demonstrates hands-on practical skills in:
- Web application security testing (Burp Suite, OWASP ZAP)
- Cloud-based penetration testing infrastructure (AWS, Kali Linux)
- Authorized social engineering simulation
- Professional security documentation and reporting

---

> 💡 *All lab testing was conducted against intentionally vulnerable applications (DVWA) in authorized, isolated cloud environments — no real systems or user data were involved.*
