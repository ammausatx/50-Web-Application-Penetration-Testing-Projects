# 50 Web Application Penetration Testing Projects

A hands-on collection of 50 web application security testing projects, arranged from beginner to advanced. Each project has its own walkthrough, lab guidance, test actions, evidence notes, embedded screenshots, and reporting guidance.

> **Authorization:** Use only intentionally vulnerable applications you control or systems covered by explicit written authorization. Keep labs isolated. Never test public or production systems without permission.

> **Screenshot notice:** The shared images embedded in each project are simulated training illustrations, not real test evidence. Replace them with your own redacted screenshots from an authorized lab. Each project README embeds three project-specific simulated tool-interface illustrations (setup, execution, and result review) using relative links. Replace them with your own redacted lab captures when available.

## Project walkthroughs

- [Project 01 — Web Application Reconnaissance](beginner/01-web-application-reconnaissance/README.md)
- [Project 02 — HTTP Request and Response Analysis](beginner/02-http-request-response-analysis/README.md)
- [Project 03 — Security Headers Assessment](beginner/03-security-headers-assessment/README.md)
- [Project 04 — Cookie Security Assessment](beginner/04-cookie-security-assessment/README.md)
- [Project 05 — SSL/TLS Security Assessment](beginner/05-ssl-tls-security-assessment/README.md)
- [Project 06 — Robots.txt and Sitemap Analysis](beginner/06-robots-txt-sitemap-analysis/README.md)
- [Project 07 — Directory and File Enumeration](beginner/07-directory-and-file-enumeration/README.md)
- [Project 08 — Authentication Security Testing](beginner/08-authentication-security-testing/README.md)
- [Project 09 — Password Reset Security Testing](beginner/09-password-reset-security-testing/README.md)
- [Project 10 — User Registration Security Testing](beginner/10-user-registration-security-testing/README.md)
- [Project 11 — Input Validation Testing](beginner/11-input-validation-testing/README.md)
- [Project 12 — Reflected XSS Testing](beginner/12-reflected-xss-testing/README.md)
- [Project 13 — HTML Form Security Testing](beginner/13-html-form-security-testing/README.md)
- [Project 14 — Error Handling and Information Disclosure](beginner/14-error-handling-information-disclosure/README.md)
- [Project 15 — Basic Access Control Testing](beginner/15-basic-access-control-testing/README.md)
- [Project 16 — SQL Injection Testing](intermediate/16-sql-injection-testing/README.md)
- [Project 17 — Stored XSS Testing](intermediate/17-stored-xss-testing/README.md)
- [Project 18 — DOM-Based XSS Testing](intermediate/18-dom-based-xss-testing/README.md)
- [Project 19 — IDOR Vulnerability Testing](intermediate/19-idor-vulnerability-testing/README.md)
- [Project 20 — Horizontal Privilege Escalation](intermediate/20-horizontal-privilege-escalation/README.md)
- [Project 21 — Vertical Privilege Escalation](intermediate/21-vertical-privilege-escalation/README.md)
- [Project 22 — CSRF Vulnerability Testing](intermediate/22-csrf-vulnerability-testing/README.md)
- [Project 23 — File Upload Security Testing](intermediate/23-file-upload-security-testing/README.md)
- [Project 24 — Path Traversal Testing](intermediate/24-path-traversal-testing/README.md)
- [Project 25 — Local File Inclusion Testing](intermediate/25-local-file-inclusion-testing/README.md)
- [Project 26 — SSRF Vulnerability Testing](intermediate/26-ssrf-vulnerability-testing/README.md)
- [Project 27 — REST API Authentication Testing](intermediate/27-rest-api-authentication-testing/README.md)
- [Project 28 — API Authorization Testing](intermediate/28-api-authorization-testing/README.md)
- [Project 29 — GraphQL Security Testing](intermediate/29-graphql-security-testing/README.md)
- [Project 30 — CORS Misconfiguration Testing](intermediate/30-cors-misconfiguration-testing/README.md)
- [Project 31 — JWT Security Testing](intermediate/31-jwt-security-testing/README.md)
- [Project 32 — Session Management Testing](intermediate/32-session-management-testing/README.md)
- [Project 33 — Business Logic Vulnerability Testing](intermediate/33-business-logic-vulnerability-testing/README.md)
- [Project 34 — Rate Limiting and Brute-Force Protection](intermediate/34-rate-limiting-brute-force-protection/README.md)
- [Project 35 — Web Cache Security Testing](intermediate/35-web-cache-security-testing/README.md)
- [Project 36 — Advanced SSRF Exploitation](advanced/36-advanced-ssrf-exploitation/README.md)
- [Project 37 — Insecure Deserialization Testing](advanced/37-insecure-deserialization-testing/README.md)
- [Project 38 — XML External Entity Testing](advanced/38-xxe-testing/README.md)
- [Project 39 — Server-Side Template Injection](advanced/39-server-side-template-injection-testing/README.md)
- [Project 40 — HTTP Request Smuggling](advanced/40-http-request-smuggling-testing/README.md)
- [Project 41 — WebSocket Security Testing](advanced/41-websocket-security-testing/README.md)
- [Project 42 — OAuth 2.0 and OpenID Connect Testing](advanced/42-oauth2-oidc-security-testing/README.md)
- [Project 43 — Multi-Tenant Authorization Testing](advanced/43-multi-tenant-authorization-testing/README.md)
- [Project 44 — GraphQL Advanced Security Testing](advanced/44-graphql-advanced-security-testing/README.md)
- [Project 45 — Web Cache Poisoning Testing](advanced/45-web-cache-poisoning-testing/README.md)
- [Project 46 — Host Header Injection Testing](advanced/46-host-header-injection-testing/README.md)
- [Project 47 — Race Condition Vulnerability Testing](advanced/47-race-condition-vulnerability-testing/README.md)
- [Project 48 — File Processing Security Testing](advanced/48-file-processing-security-testing/README.md)
- [Project 49 — Web Application Threat Modeling and Pentesting](advanced/49-web-application-threat-modeling-pentest/README.md)
- [Project 50 — Complete Web Application Penetration Test Capstone](advanced/50-complete-web-application-penetration-test/README.md)

## Learning path

| Tier | Projects | Focus |
|---|---:|---|
| Beginner | 01–15 | Reconnaissance, HTTP, configuration, cookies, authentication, input validation, access control |
| Intermediate | 16–35 | Injection, authorization, sessions, APIs, file handling, business logic, caching |
| Advanced | 36–50 | SSRF, deserialization, XXE, SSTI, request smuggling, WebSockets, OAuth, multi-tenancy, race conditions, threat modeling, capstone |

See [PROJECT_INDEX.md](PROJECT_INDEX.md) for a compact index.

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
