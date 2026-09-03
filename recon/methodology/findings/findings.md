# Security Testing Findings

## Target

**Target:** epapsy.gr  
**Assessment Type:** Non-intrusive web application security testing

---

## O-01 — Public WordPress Author/Username Enumeration

**Severity:** Informational / Low  
**Status:** Observed

### Description

The public WordPress sitemap exposes author archive URLs. An author archive associated with the username `epapsy_admin` was publicly accessible.

### Impact

Public username enumeration may provide information that could assist targeted authentication attacks.

No password, authentication bypass, privilege escalation, or account takeover was identified.

### Recommendation

Consider limiting unnecessary public author enumeration or avoiding exposure of usernames that correspond to authentication accounts.

---

# Tested Vulnerability Classes

| Vulnerability | Result |
|---|---|
| Cross-Site Scripting (XSS) | No confirmed vulnerability |
| SQL Injection | No confirmed vulnerability |
| CSRF | No confirmed vulnerability |
| Improper Access Control | No confirmed vulnerability |
| Open Redirect | No confirmed vulnerability |
| Input Validation | No confirmed vulnerability |
| Authentication | No confirmed vulnerability |
| Password Reset | No confirmed vulnerability |

---

## Additional Observations

### Complaint Form

A publicly accessible complaint form was identified and inspected. Its structure and parameters were reviewed, but no fabricated complaint or intrusive payload was submitted because the form creates a real external submission.

No vulnerability was confirmed.

### WooCommerce Functionality

Shop, cart and checkout pages displayed a store-preparation placeholder.

The product sitemap contained one product URL, but the product page also displayed a preparation placeholder. No active purchase, cart, quantity or payment functionality was available for testing.

### Newsletter Form

A valid-format newsletter submission produced a server-side error message. No security impact was demonstrated, so this was classified as a functional/server-side issue rather than a security vulnerability.

---

# Final Result

**Confirmed exploitable vulnerabilities: 0**

One informational/low-severity observation involving public WordPress author/username enumeration was documented.

The assessment was performed non-intrusively and without brute force, credential attacks, denial-of-service testing, unauthorized access, or destructive actions.
