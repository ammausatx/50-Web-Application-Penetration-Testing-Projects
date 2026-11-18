# 23. File Upload Security Testing

**Tier:** Intermediate  
**Lab:** DVWA or dedicated upload lab  
**Tools:** Burp Suite, browser DevTools, file utility

## 1. Objective
Validate file upload security testing in a controlled training application. The purpose is to establish normal behavior, test one security boundary at a time, and preserve reproducible evidence.

## 2. Lab setup and scope
Deploy the selected target in an isolated VM, Docker network, or localhost-only environment. Use disposable accounts and synthetic records. Record the exact target URL, application version, date, and tool versions. Stay within the authorized lab scope.

## 3. Baseline
Complete the normal workflow first. Capture the request and response in Burp, note the expected behavior, and save a sanitized baseline.

## 4. Step-by-step walkthrough

### Step 1

Map upload form and record allowed extensions, size limits, and response behavior

### Step 2

Upload a harmless text or image file and inspect storage and retrieval

### Step 3

Change filename and MIME metadata in Burp while keeping content harmless

### Step 4

Check actual content validation, renaming, storage location, and execution restrictions

### Step 5

Recommend allowlists, content inspection, safe storage, and size limits


## 5. Screenshots and evidence
The embedded images are simulated training illustrations, not real test evidence. Replace them with your own redacted screenshots after executing the lab.

![Simulated test execution](../../_assets/screenshots/test-execution.svg)

![Simulated result review](../../_assets/screenshots/result-review.svg)

Preserve the request, response, test account role, timestamp, and relevant application logs. Redact credentials, session identifiers, tokens, and personal data.

## 6. Analysis and expected output
A scanner alert or unexpected response is not sufficient by itself. Reproduce the behavior manually, compare it with baseline, and explain the preconditions and verified confidentiality, integrity, or availability impact. Note false-positive checks and limitations.

## 7. Findings and remediation
Use the report format in [SCREENSHOTS_GUIDE.md](../../SCREENSHOTS_GUIDE.md) as evidence guidance and document a finding only when confirmed. Include root cause, affected endpoint, severity reasoning, remediation, and retest steps.

## 8. References
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)

**Safety:** Authorized, isolated training targets only. Do not run these tests against systems without explicit written permission.
