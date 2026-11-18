# 45. Web Cache Poisoning Testing

**Tier:** Advanced  
**Lab:** PortSwigger Academy or isolated reverse-proxy lab  
**Tools:** Burp Suite, curl, browser DevTools

## 1. Objective
Conduct a controlled assessment of web cache poisoning testing and understand the security boundary, prerequisites, and impact. Advanced projects require a dedicated lab and careful rules of engagement.

## 2. Lab setup and rules of engagement
Build the target only in an isolated training network. Use mock internal services, synthetic records, disposable accounts, and local callback endpoints where required. Record exact in-scope hosts and ports. Do not probe real internal networks, cloud metadata services, or third-party infrastructure.

## 3. Baseline and architecture
Document the normal workflow and relevant components before testing. Capture baseline requests, responses, application logs, and version information. Identify trust boundaries and expected authorization behavior.

## 4. Step-by-step walkthrough

### Step 1

Identify cacheable responses and determine cache-key behavior

### Step 2

Vary one header at a time using a benign marker

### Step 3

Check whether an unkeyed header influences the response or redirect

### Step 4

Verify only in the isolated lab and clear cache state between tests

### Step 5

Recommend correct cache-key normalization and safe handling of untrusted headers


## 5. Screenshots and evidence
These embedded images are simulated training illustrations, not real test evidence. Replace them with your own redacted captures from the authorized lab.

![Simulated test execution](../../_assets/screenshots/test-execution.svg)

![Simulated result review](../../_assets/screenshots/result-review.svg)

Preserve minimal reproducible requests, responses, timestamps, relevant logs, and test account roles. Redact secrets and personal information. Never publish live tokens, keys, customer records, or internal production details.

## 6. Technical analysis and expected output
Validate each observation manually. Explain root cause, trust boundary crossed, prerequisites, affected components, and demonstrated confidentiality, integrity, or availability impact. Document negative tests, false-positive checks, and limitations. A theoretical attack path is not a confirmed finding.

## 7. Findings, remediation, and retest
Use a consistent finding format: title, severity rationale, affected component, description, evidence, impact, reproduction, root cause, remediation, and retest result. Recommend architectural fixes where needed and verify that the fix closes the attack path without breaking legitimate behavior.

## 8. References
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)

**Safety:** Authorized isolated training environments only. Do not run advanced tests against systems without explicit written permission.
