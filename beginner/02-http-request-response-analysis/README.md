# 02. HTTP Request and Response Analysis

**Tier:** Beginner  
**Lab:** Juice Shop or WebGoat  
**Tools:** Burp Suite, curl, browser DevTools

## Objective
Understand how browser requests are processed and how server responses reveal application behavior.

## Walkthrough

### 1. Capture a baseline request
Open the lab app through a browser configured to use Burp. Load the home page and select its request in Proxy → HTTP history.

### 2. Inspect the request
Record method, path, host, query parameters, headers, cookies, and body. Identify which values are controlled by the browser.

### 3. Inspect the response
Record status code, response headers, content type, redirects, cookies, and body format. Compare HTML responses with API responses.

### 4. Compare HTTP methods
Run:
~~~bash
curl -i http://<LAB_HOST>:3000/
curl -I http://<LAB_HOST>:3000/
curl -i -X OPTIONS http://<LAB_HOST>:3000/
~~~
Record the actual behavior; do not assume every method is supported.

### 5. Use Repeater
Send a normal search or display request to Repeater. Change one harmless parameter and resend. Compare response status, length, and returned content.

### 6. Document the behavior
Create a request/response table with endpoint, method, parameters, status, content type, and observations. Save sanitized examples.

## Screenshots
These are simulated illustrations. Replace them with your own authorized lab screenshots.



## Expected output
An HTTP traffic analysis report explaining the application's normal request patterns, response behavior, headers, cookies, and user-controlled parameters.

## Analysis
A changed response does not automatically mean a vulnerability. Explain what the application did and whether the behavior violates a security requirement. Redact session identifiers and credentials.


## Simulated tool screenshots

> These are **simulated tool-interface examples** created for learning. They are not live captures, real scan output, or proof that a vulnerability exists. Values and results are illustrative. Reproduce the workflow in your own authorized lab before reporting a finding.

### Step 1 — Tool setup and initial command

![Simulated HTTP Request and Response Analysis tool setup](screenshots/01-tool-setup.svg)

The screen shows the selected tool, the lab target, and the initial command or configuration. Use it as a visual guide when preparing your own test.

### Step 2 — Test execution

![Simulated HTTP Request and Response Analysis test execution](screenshots/02-test-execution.svg)

This screen illustrates the request, input, or test action. Compare it with the walkthrough instructions and adjust only within your authorized lab scope.

### Step 3 — Result review

![Simulated HTTP Request and Response Analysis result review](screenshots/03-result-review.svg)

This screen illustrates an example result and analyst review. It is not a confirmed finding. Validate actual behavior, preserve your own evidence, and complete the report template.
