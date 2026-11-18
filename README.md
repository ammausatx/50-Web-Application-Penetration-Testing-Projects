# 50 Web Application Penetration Testing Projects

A hands-on collection of 50 web application security testing projects, arranged from beginner to advanced. Each project has its own walkthrough, lab guidance, test actions, evidence notes, embedded screenshots, and reporting guidance.

> **Authorization:** Use only intentionally vulnerable applications you control or systems covered by explicit written authorization. Keep labs isolated. Never test public or production systems without permission.

> **Screenshot notice:** The shared images embedded in each project are simulated training illustrations, not real test evidence. Replace them with your own redacted screenshots from an authorized lab. Every project README embeds both images using relative Markdown links.

## Learning path

| Tier | Projects | Focus |
|---|---:|---|
| Beginner | 01–15 | Reconnaissance, HTTP, configuration, cookies, authentication, input validation, access control |
| Intermediate | 16–35 | Injection, authorization, sessions, APIs, file handling, business logic, caching |
| Advanced | 36–50 | SSRF, deserialization, XXE, SSTI, request smuggling, WebSockets, OAuth, multi-tenancy, race conditions, threat modeling, capstone |

See [PROJECT_INDEX.md](PROJECT_INDEX.md) for navigation.

## Repository layout
- `beginner/` — projects 01–15
- `intermediate/` — projects 16–35
- `advanced/` — projects 36–50
- `_assets/screenshots/` — shared illustrative SVG screenshots
- `SCREENSHOTS_GUIDE.md` — replacing illustrations with real captures
- `CONTRIBUTING.md` — evidence and contribution rules

## Suggested lab targets and tools
Targets: OWASP Juice Shop, DVWA, WebGoat, OWASP crAPI, PortSwigger Web Security Academy labs, and purpose-built local apps.

Tools: Burp Suite, OWASP ZAP, Nmap, WhatWeb, ffuf, Gobuster, curl, OpenSSL, testssl.sh, Postman, and browser Developer Tools.

## Workflow
1. Read the project scope and safety notes.
2. Deploy the target in an isolated lab.
3. Capture baseline behavior.
4. Follow the walkthrough and verify results manually.
5. Replace simulated screenshots with your own redacted lab captures.
6. Complete reports using verified evidence only.
7. Retest after remediation.

Do not commit credentials, session tokens, personal information, production data, or unredacted customer evidence.

## Disclaimer
Educational material only. It is not authorization to test any system. Follow applicable law, contracts, and rules of engagement.
