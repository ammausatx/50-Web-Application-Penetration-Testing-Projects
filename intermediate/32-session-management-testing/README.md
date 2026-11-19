# 32. Session Management Testing

**Tier:** Intermediate  
**Lab:** Juice Shop or DVWA with test accounts  
**Tools:** Burp Suite, browser DevTools

## Objective
Assess session management testing using a repeatable test plan in an isolated training environment.

## Lab setup and scope
Deploy the lab target locally or in a dedicated host-only network. Create disposable test users and synthetic data. Record target, version, date, and tool versions. Only test assets explicitly in scope.

## Baseline
Perform the normal application workflow and capture a representative request and response before modifying any inputs. Redact secrets in saved evidence.

## Step-by-step walkthrough

### Step 1

Capture session identifiers before and after login

### Step 2

Check rotation after authentication and privilege changes

### Step 3

Test idle and absolute expiration against the stated lab policy

### Step 4

Log out and verify server-side invalidation; compare concurrent sessions if supported

### Step 5

Recommend secure generation, rotation, expiry, and invalidation


## Screenshots and evidence
The images below are simulated training illustrations and are not real test evidence. Replace them with your own redacted lab screenshots after testing.



Preserve the baseline, test request, response, timestamp, test account role, and relevant logs. Never publish passwords, session tokens, API keys, or personal information.

## Expected results and analysis
Compare each test with the baseline. Manually reproduce any suspected issue and document false-positive checks. State exactly what the application did, which security boundary was affected, and what impact was demonstrated. A tool alert alone is not a confirmed finding.

## Findings, remediation, and retest
Document confirmed findings with affected endpoint, prerequisites, severity reasoning, evidence, impact, and root cause. Recommend server-side enforcement and secure defaults appropriate to the weakness. Retest after remediation and record the result.

## References
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)

**Safety:** Authorized isolated lab targets only. No testing against systems without explicit written permission.

## Project-specific simulated tool screenshots

> Fictional training illustrations of setup, test execution, and analyst review—not genuine captures, actual scan output, or proof of a vulnerability. Reproduce the workflow in an authorized lab and replace these examples with your own redacted evidence.

![Project 32 tool setup — simulated training illustration](screenshots/01-tool-setup.svg)

![Project 32 test execution — simulated training illustration](screenshots/02-test-execution.svg)

![Project 32 result review — simulated training illustration](screenshots/03-result-review.svg)
