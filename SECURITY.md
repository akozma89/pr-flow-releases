# Security Policy

Security is a top priority for PR Flow. While the app is designed with an offline-first and privacy-centric architecture, we take all security concerns seriously.

**Architecture Note for Researchers:** PR Flow operates entirely locally as a desktop application and does not use an intermediate backend server. For most integrations (GitHub, Jira, Claude), PR Flow delegates authentication and network requests entirely to the official command-line tools installed on the host system (e.g., `gh`, `acli`, `claude`) and does **not** store or have direct access to those credentials. For Gerrit, HTTP credentials are encrypted and stored securely on the local machine.

## Supported Versions

We currently provide security updates only for the latest major version of PR Flow. Please ensure you are running the most recent release before reporting an issue.

| Version | Supported          |
| ------- | ------------------ |
| v1.x.x  | :white_check_mark: |
| < v1.0  | :x:                |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

If you believe you have found a security vulnerability in PR Flow, please report it privately to ensure the safety of all users.

The preferred way to report is via GitHub's **Private Vulnerability Reporting**. Navigate to the **Security** tab of this repository and click `Report a vulnerability`.

Alternatively, you can send an email to: **arpadkozma89@gmail.com**

### What to include in your report:
* A title prefixed with `[PRFLOW-SECURITY]`
* A description of the vulnerability and its impact.
* Exact steps to reproduce the issue.
* Your operating system and PR Flow version.

We will acknowledge receipt of your vulnerability report within 48 hours and strive to send you regular updates about our progress. If the vulnerability is accepted, we will release a patch as soon as possible.

### Bug Bounty Program
PR Flow is built by an independent developer. While we deeply appreciate responsible disclosure and will credit you in our release notes (if desired), we do not currently operate a paid bug bounty program.
