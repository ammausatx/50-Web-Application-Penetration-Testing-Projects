# 01. Web Application Reconnaissance

**Tier:** Beginner  
**Lab:** OWASP Juice Shop or another local web application  
**Tools:** Nmap, WhatWeb, Burp Suite, browser DevTools, curl

## Objective
Identify the application's externally visible attack surface before attempting vulnerability testing.

## Lab setup and scope
Deploy Juice Shop locally or in an isolated VM. Record the exact target URL and IP. Do not scan anything outside the lab. Create an evidence folder and record tool versions.

## Walkthrough

### 1. Confirm the target
Open the application in a browser and confirm it loads. Record the target host, port, date, and application version.

### 2. Check reachability and service
Run:
~~~bash
ping -c 3 <LAB_IP>
nmap -sV -p 3000 <LAB_IP>
~~~
Record the open port and detected service. Keep the scan limited to the lab host.

### 3. Fingerprint the web technology
Run:
~~~bash
whatweb http://<LAB_HOST>:3000
curl -sSI http://<LAB_HOST>:3000
~~~
Compare WhatWeb output with response headers. Treat fingerprints as clues, not proof of a vulnerable version.

### 4. Browse and map the application
Visit the home page, login, registration, search, product, and other normal features. Record page URLs, forms, input fields, and visible roles.

### 5. Capture application traffic
Configure Burp Suite as the browser proxy. Browse the app and inspect HTTP history. Record methods, endpoints, status codes, parameters, cookies, and API requests. Redact tokens.

### 6. Build the attack-surface inventory
Group observations into pages, forms, authentication, APIs, technologies, and potentially sensitive functions. Select candidates for later projects.

## Evidence and screenshots
The images are shared simulated illustrations, not actual scan evidence. Replace them with your own redacted lab captures.

![Simulated reconnaissance test execution](../../_assets/screenshots/test-execution.svg)

![Simulated reconnaissance result review](../../_assets/screenshots/result-review.svg)

## Expected output
A reconnaissance report with target details, exposed services, technology observations, page and endpoint inventory, and follow-up testing recommendations.

## Analysis and remediation
A discovered endpoint is not automatically a vulnerability. Verify whether it exposes sensitive information or permits unauthorized actions. Remove unnecessary public resources and enforce authentication and authorization server-side.

## Report checklist
- [ ] Scope and target recorded
- [ ] Tool versions and commands saved
- [ ] Pages, forms, and endpoints inventoried
- [ ] Evidence redacted
- [ ] Findings independently validated
- [ ] Recommendations and limitations documented
