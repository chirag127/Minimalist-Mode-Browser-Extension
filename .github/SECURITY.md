# Security Policy

## Supported Versions

We are committed to providing a secure and reliable extension. As such, we are currently only supporting and patching security vulnerabilities in the latest stable release of FocusFlow.

## Reporting a Vulnerability

We appreciate your efforts to responsibly disclose security vulnerabilities. If you find a security issue, please follow these steps:

1.  **DO NOT** open a public issue.
2.  Send an email to our dedicated security team at `security@example.com` (Note: This is a placeholder. In a real project, this would be a specific, monitored email address).
3.  In your email, please include:
    *   A detailed description of the vulnerability.
    *   Steps to reproduce the vulnerability.
    *   Any relevant system information (e.g., browser version, extension version).
    *   Proof of Concept (PoC) code or screenshots, if applicable.
4.  Allow us a reasonable time (e.g., 7-14 days) to investigate and address the issue before disclosing it publicly.

We will acknowledge your report within 48 hours and provide updates on the status of the fix.

## Security Best Practices

FocusFlow is built with security in mind. However, as a browser extension, user security also depends on:

*   **Browser Updates:** Ensure your browser is always up-to-date with the latest security patches.
*   **Official Sources:** Only install FocusFlow from the official browser web store or trusted sources specified on our official repository (`https://github.com/chirag127/FocusFlow-Distraction-Free-Browser-Extension`).
*   **Extension Permissions:** Be mindful of the permissions requested by any browser extension. FocusFlow requests only the necessary permissions to function.

## Security Audits & Tools

We aim to maintain a high level of security by:

*   **Automated Scanning:** Integrating security scanning tools into our CI/CD pipeline (`https://github.com/chirag127/FocusFlow-Distraction-Free-Browser-Extension/actions/workflows/ci.yml`).
*   **Code Reviews:** Conducting thorough code reviews for all changes.
*   **Dependency Management:** Regularly updating dependencies to their latest secure versions using `uv` and `Ruff` to identify and fix potential vulnerabilities.

Thank you for helping us keep FocusFlow secure!
