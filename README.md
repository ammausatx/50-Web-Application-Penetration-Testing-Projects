# 50 Web Application Penetration Testing Projects

A structured, GitHub-ready portfolio of 50 hands-on web application penetration testing projects, organized by skill level and OWASP-aligned category. Companion collection to **50 Network Penetration Testing Projects**, following the same documentation standard.

> ⚠️ **Scope and ethics:** Every project in this repository was designed to be performed only against intentionally vulnerable applications you deploy yourself (OWASP Juice Shop, DVWA, WebGoat) in an isolated lab. Never run these techniques against systems you do not own or do not have explicit written authorization to test.

## Collection Overview

| Tier | Projects | Focus |
|------|----------|-------|
| Beginner | 15 (01–15) | Reconnaissance, configuration review, basic auth/session checks |
| Intermediate | 20 (16–35) | Injection, access control, session security, API security, file security |
| Advanced | 15 (36–50) | API internals, SSRF, deserialization, business logic, capstone |

## Project Categories

| Category | Testing Focus |
|----------|----------------|
| Reconnaissance | Web discovery, fingerprinting, enumeration |
| Authentication | Login security, password policies, MFA |
| Authorization | IDOR, privilege escalation, access control |
| Injection | SQLi, XSS, command injection, XXE, SSTI, NoSQLi |
| Session Security | Cookies, session fixation, hijacking |
| API Security | REST, GraphQL, API authorization |
| File Security | Upload vulnerabilities, LFI, path traversal |
| Configuration | Security headers, TLS, misconfigurations |
| Business Logic | Workflow abuse, price manipulation, race conditions |
| Advanced Testing | SSRF, deserialization, request smuggling, prototype pollution |

## Documentation Standard

Every project folder's `README.md` follows the same eight-section structure, and now includes a **conceptual attack-flow diagram** at the top of the walkthrough (Section 4) so the attack pattern is visible at a glance:

1. Project overview and objectives
2. Lab environment and setup
3. Tools and commands used
4. Step-by-step testing walkthrough — opens with a conceptual diagram (`_assets/diagrams/`), then the concrete steps
5. Interpretation and technical analysis
6. Findings (severity, risk, impact table)
7. Remediation recommendations
8. Final penetration testing report summary

Screenshot placeholders (`screenshots/0N-description.png`) are marked in each README with 📸 — add your own real captures as you run each lab, alongside the conceptual diagram. See `SCREENSHOTS_GUIDE.md` for what to capture.

## Repository Structure

```
50-Web-Application-Penetration-Testing-Projects/
│
├── _assets/
│   └── diagrams/        (10 conceptual attack-flow SVGs, one per category)
│
├── beginner/            (15 projects: 01-15)
│   ├── 01-web-fingerprinting-tech-stack/
│   │   ├── README.md
│   │   └── screenshots/
│   └── ...
│
├── intermediate/        (20 projects: 16-35)
│   └── ...
│
├── advanced/            (15 projects: 36-50)
│   └── ...
│
├── SCREENSHOTS_GUIDE.md
├── PROJECT_INDEX.md
└── README.md
```

## Tools and Lab Environments

- **Proxies/Scanners:** Burp Suite (Community/Pro), OWASP ZAP
- **Automation:** sqlmap, Gobuster, ffuf, testssl.sh, jwt_tool, Turbo Intruder
- **Vulnerable targets:** OWASP Juice Shop, DVWA, WebGoat
- **Attacker platform:** Kali Linux (VM or Docker)

## How to Use This Repository

1. Pick a project folder in order of tier (beginner → advanced).
2. Spin up the matching vulnerable app in your lab.
3. Read the walkthrough — the conceptual diagram at the top of Section 4 shows the attack pattern before you dive into the specific steps.
4. Follow the steps, capturing your own real screenshots at each 📸 marker.
5. Fill in the Findings, Remediation, and Report sections with your actual results.
6. Commit your filled-in README + screenshots back into that project's folder.

See `PROJECT_INDEX.md` for the full numbered list of all 50 projects with tier and category.
