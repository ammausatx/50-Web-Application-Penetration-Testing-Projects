# 13. HTML Form Security Testing

**Tier:** Beginner  
**Lab:** DVWA or WebGoat  
**Tools:** Burp Suite, browser DevTools, curl

## Objective
Assess whether the application enforces the expected security controls for html form security testing.

## Lab preparation and scope
Deploy the selected application in an isolated VM, Docker network, or localhost environment. Use disposable test accounts and synthetic data. Record target URL, version, date, and tool versions. Never test third-party or production systems without written authorization.

## Baseline
Complete the normal workflow once. Capture the request and response in Burp and note expected behavior before changing requests.

## Step-by-step walkthrough

### Step 1

Inventory form action, method, input names, hidden fields, and client-side constraints

### Step 2

Submit valid and invalid values and capture responses

### Step 3

Modify a hidden or client-controlled field in Burp

### Step 4

Remove required fields or change types to test server-side validation

### Step 5

Report security-relevant trust failures and recommend server-side enforcement


## Screenshots and evidence
The images are simulated training illustrations, not real test evidence. Replace them with your own redacted screenshots after running the authorized lab.

![Simulated test execution](../../_assets/screenshots/test-execution.svg)

![Simulated result review](../../_assets/screenshots/result-review.svg)

Save sanitized request/response examples. Redact credentials, cookies, reset links, tokens, and personal data.

## Analysis and expected output
Compare test behavior with baseline. Validate suspected issues manually and rule out expected application behavior. Record endpoint, test role, input, response, reproducibility, and verified impact.

## Findings and remediation
Use the report template in report/report-template.md. Recommend server-side controls, secure framework defaults, least privilege, and safe handling of user-controlled data as appropriate. Retest after remediation.

## References
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
