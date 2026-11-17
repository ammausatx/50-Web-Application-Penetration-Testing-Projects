# Screenshot Guide

Each project README now opens Section 4 with a **conceptual attack-flow diagram** (`_assets/diagrams/<category>.svg`) so you have a picture to orient yourself with while reading — it illustrates the general shape of that category's attack, not this specific run.

Beyond that diagram, each README still references four screenshot placeholders for your own real lab evidence:

1. **`01-lab-setup.png`** — The target application running (e.g., Juice Shop home page) with Burp Suite's proxy configured and intercepting, proving the test environment is correctly set up.
2. **`02-request-capture.png`** — The relevant HTTP request/response captured in Burp's Proxy or Repeater, showing the parameter/endpoint under test *before* any payload is sent.
3. **`03-exploitation-step.png`** — The payload submission itself: the modified request in Repeater/Intruder, or the relevant tool's (sqlmap, jwt_tool, etc.) terminal output.
4. **`04-result-confirmation.png`** — The confirmed result: the response proving the vulnerability (e.g., bypassed login, extracted data, executed script). If the result is sanitized or partially redacted for sharing, label the image clearly, e.g. `04-result-confirmation-REDACTED.png`, and note the redaction in the README's Findings section.

## General rules
- Store screenshots inside that project's own `screenshots/` folder, referenced with a relative path (`screenshots/01-lab-setup.png`) so GitHub renders them inline automatically.
- Never include real third-party data, production hostnames, or credentials in a screenshot — lab apps only.
- If a finding could not be safely reproduced for the public repo, replace the live screenshot with a clearly labeled simulated/mock diagram instead of omitting it, and say so in the README.
- Keep filenames exactly as the placeholders specify so links in the README resolve without edits.
- Don't delete or rename the `_assets/diagrams/` folder — every project's Section 4 links into it.
