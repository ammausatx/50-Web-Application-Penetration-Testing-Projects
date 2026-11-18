# 06. Robots.txt and Sitemap Analysis

**Tier:** Beginner  
**Lab:** Juice Shop or a local web server with robots.txt and sitemap.xml  
**Tools:** Browser, curl, Burp Suite

## Objective
Review publicly referenced paths and determine whether any resource is unintentionally exposed.

## Walkthrough

### 1. Request discovery files
~~~bash
curl -i http://<LAB_HOST>/robots.txt
curl -i http://<LAB_HOST>/sitemap.xml
~~~

### 2. Extract paths
Record disallowed paths, sitemap URLs, and references to staging, admin, test, or obsolete resources.

### 3. Validate paths individually
Request each discovered path and record status, redirect, content type, and authentication behavior. Do not assume a path is sensitive based on its name.

### 4. Verify exposure
Determine whether a resource actually returns sensitive information or allows an unauthorized action. A robots.txt entry alone is not a vulnerability.

### 5. Document findings
Include the source file, discovered path, observed response, access requirement, and verified impact.

## Screenshots
Simulated illustrations only; replace with your own lab evidence.

![Simulated robots and sitemap test](../../_assets/screenshots/test-execution.svg)

![Simulated resource validation review](../../_assets/screenshots/result-review.svg)

## Expected output
A resource discovery report distinguishing ordinary public routes from confirmed information disclosure.
