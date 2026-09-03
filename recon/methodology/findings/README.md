# Bug Hunting on EPAPSY

## Cyber Security Major Project

A non-intrusive web application security assessment performed on the
publicly accessible **EPAPSY website (`epapsy.gr`)** as part of a
cybersecurity major project.

---

## 🎯 Objective

The objective of this project was to perform structured security testing
on an authorized open bug-bounty target and identify potential web
application vulnerabilities while following responsible and
non-intrusive testing practices.

---

## 🌐 Target

**Target:** https://www.epapsy.gr/

**Scope:** epapsy.gr

The assessment focused only on publicly accessible functionality within
the target scope.

---

## 🔍 Methodology

The assessment followed these stages:

1. Reconnaissance
2. Endpoint and functionality enumeration
3. Manual security testing
4. Vulnerability verification
5. Evidence collection
6. Findings classification
7. Documentation

---

## 🛠️ Tools & Techniques

- Web browser / Developer Tools
- JavaScript Console
- Network inspection
- WordPress XML sitemap analysis
- `robots.txt` analysis
- Manual HTTP request/response inspection
- Manual input testing

---

## 🧪 Security Tests Performed

The following vulnerability classes were assessed where applicable:

- Cross-Site Scripting (XSS)
- SQL Injection
- Cross-Site Request Forgery (CSRF)
- Improper Access Control
- Open Redirect
- Input Validation
- Authentication
- Password Reset

---

## 📊 Results

| Test | Result |
|---|---|
| XSS | No confirmed vulnerability |
| SQL Injection | No confirmed vulnerability |
| CSRF | No confirmed vulnerability |
| Improper Access Control | No confirmed vulnerability |
| Open Redirect | No confirmed vulnerability |
| Input Validation | No confirmed vulnerability |
| Authentication | No confirmed vulnerability |
| Password Reset | No confirmed vulnerability |

### Informational Finding

**O-01 — Public WordPress Author/Username Enumeration**

A publicly accessible WordPress author archive exposed an author
associated with the username `epapsy_admin`.

No password, authentication bypass, privilege escalation, or account
takeover was identified.

**Severity:** Informational / Low

---

## 🔎 Additional Reconnaissance

The assessment identified:

- Public WordPress XML sitemaps
- Public author archives
- Search functionality
- Elementor-based forms
- WooCommerce-related endpoints
- Public authentication and password-reset pages
- Public complaint form
- Newsletter form

The Shop, Cart, Checkout and Product pages were found to be in a
store-preparation state, so active purchasing functionality was not
available for testing.

---

## 🛡️ Testing Ethics

Testing was performed using a non-intrusive approach.

The assessment did **not** include:

- Brute-force attacks
- Credential stuffing
- Denial-of-service testing
- Destructive testing
- Unauthorized account access
- Accessing other users' private information
- Spam or fabricated submissions
- Aggressive automated scanning

Only functionality that could be safely assessed without causing harm
was tested.

---

## 📁 Repository Structure

```text
Bug-Hunting-EPAPSY/
│
├── README.md
│
├── methodology/
│   └── README.md
│
├── findings/
│   └── findings.md
│
├── recon/
│   └── target.txt
│
└── evidence/
    └── screenshots/
