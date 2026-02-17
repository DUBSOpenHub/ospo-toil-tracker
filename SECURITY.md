# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in any automation built from this tracker, please report it responsibly:

1. **Do not** open a public issue
2. Email the maintainers directly (see repo contacts)
3. Include a description of the vulnerability and steps to reproduce

We will acknowledge your report within 48 hours and provide a timeline for a fix.

## Scope

This repository primarily tracks toil ideas and lightweight automations. Security concerns may include:

- **Webhook secrets** — Ensure Slack webhook URLs are stored as secrets, never in code
- **API tokens** — Any automation scripts must use environment variables or secret managers for credentials
- **Permissions** — Automations should follow the principle of least privilege
