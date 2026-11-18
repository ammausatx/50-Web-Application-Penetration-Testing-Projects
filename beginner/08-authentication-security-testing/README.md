# 08. Authentication Security Testing

**Tier:** Beginner  
**Lab:** WebGoat or Juice Shop with two disposable accounts  
**Tools:** Burp Suite, browser DevTools

## Objective
Assess whether the application enforces the expected security controls for authentication security testing.

## Lab preparation and scope
Deploy the selected application in an isolated VM, Docker network, or localhost environment. Use disposable test accounts and synthetic data. Record target URL, version, date, and tool versions. Never test third-party or production systems without written authorization.

## Baseline
Complete the normal workflow once. Capture the request and response in Burp and note expected behavior before changing requests.

## Step-by-step walkthrough

### Step 1

Create two lab accounts and capture a normal login request

### Step 2

Inspect submitted fields, CSRF values, cookies, redirects, and response

### Step 3

Submit a few controlled invalid credentials and compare error messages

### Step 4

Review password policy, throttling, lockout, MFA, and recovery behavior

### Step 5

Record account-enumeration signals; do not run high-volume attempts


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
