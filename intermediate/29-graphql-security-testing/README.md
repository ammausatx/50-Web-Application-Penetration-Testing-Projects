# 29. GraphQL Security Testing

**Tier:** Intermediate  
**Lab:** Local GraphQL lab or suitable crAPI module  
**Tools:** Burp Suite, GraphQL Playground, Postman

## Objective
Assess graphql security testing using a repeatable test plan in an isolated training environment.

## Lab setup and scope
Deploy the lab target locally or in a dedicated host-only network. Create disposable test users and synthetic data. Record target, version, date, and tool versions. Only test assets explicitly in scope.

## Baseline
Perform the normal application workflow and capture a representative request and response before modifying any inputs. Redact secrets in saved evidence.

## Step-by-step walkthrough

### Step 1

Identify GraphQL endpoint and capture a normal query

### Step 2

Inspect schema behavior and identify queries and mutations available to the test role

### Step 3

Test authorization on selected fields and mutations using separate accounts

### Step 4

Measure depth and complexity limits with bounded queries

### Step 5

Document excessive exposure and recommend field-level authorization and query limits


## Screenshots and evidence
The images below are simulated training illustrations and are not real test evidence. Replace them with your own redacted lab screenshots after testing.

![Simulated test execution](../../_assets/screenshots/test-execution.svg)

![Simulated result review](../../_assets/screenshots/result-review.svg)

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
