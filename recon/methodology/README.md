# Methodology

The security assessment followed a structured, non-intrusive web application testing methodology.

## 1. Reconnaissance
- Identified the target and publicly accessible attack surface.
- Reviewed robots.txt and WordPress XML sitemaps.
- Identified technologies and publicly accessible application areas.
- Enumerated relevant pages, forms, authentication endpoints and product functionality.

## 2. Scanning and Enumeration
- Examined accessible URLs and application functionality.
- Identified search, forms, authentication, password-reset and WooCommerce-related endpoints.
- Reviewed publicly exposed WordPress author information.

## 3. Manual Security Testing
The following vulnerability classes were assessed where applicable:

- Cross-Site Scripting (XSS)
- SQL Injection
- Cross-Site Request Forgery (CSRF)
- Improper Access Control
- Open Redirect
- Input Validation
- Authentication and Password Reset

## 4. Verification
Potential observations were checked for reproducibility and security impact.

No intrusive exploitation, brute-force attacks, denial-of-service testing, credential attacks, or unauthorized access attempts were performed.

## 5. Documentation
Testing results, observations, screenshots and limitations were documented.

The final assessment distinguishes between confirmed security vulnerabilities, informational observations and functionality that was not testable.
