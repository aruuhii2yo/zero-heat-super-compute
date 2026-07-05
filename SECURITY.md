# Security Policy

## Reporting a vulnerability

If you believe you've found a security issue in the Zero Heat Super Compute
gateway, any engine binary, or the download service, please email
**aruuh@advancedapparchitect.com** with the details. Please do not open a
public issue for security reports.

We aim to acknowledge reports within 72 hours.

## Scope notes

- All license verification is performed server-side against Gumroad.
- Quezar storage uses AES-256-GCM authenticated encryption (NIST SP 800-38D).
- Engine downloads are personalized per license and delivered via short-lived
  (1 hour) signed URLs.
