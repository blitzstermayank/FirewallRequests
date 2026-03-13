# Security Policy

## Supported Versions

The following versions are currently receiving security updates and patches:

| Version | Supported          | End of Life     |
| ------- | ------------------ | --------------- |
| 5.1.x   | :white_check_mark: | Not yet set     |
| 5.0.x   | :x:                | January 2024    |
| 4.0.x   | :white_check_mark: | December 2024   |
| 3.x.x   | :x:                | June 2023       |
| < 3.0   | :x:                | End of life     |

> **Note:** We strongly recommend always using the latest stable release to ensure you receive all security patches and improvements.

---

## Reporting a Vulnerability

We take the security of this project seriously. If you have discovered a security vulnerability, we appreciate your help in disclosing it to us responsibly.

### 🔒 Private Disclosure (Preferred)

**Please do NOT open a public GitHub issue for security vulnerabilities.**

Instead, report vulnerabilities through one of the following channels:

- **GitHub Security Advisories:** Use the [Report a Vulnerability](../../security/advisories/new) button on this repository's Security tab *(preferred)*
- **Email:** Send details to **security@yourproject.com**
- **PGP Encrypted Email:** If your report contains highly sensitive information, please use our PGP key (Key ID: `0xABCD1234`, available on [keys.openpgp.org](https://keys.openpgp.org))

### 📋 What to Include in Your Report

To help us triage and resolve the issue quickly, please include:

- **Description** — A clear summary of the vulnerability and its potential impact
- **Affected versions** — Which version(s) are impacted
- **Steps to reproduce** — A detailed, step-by-step guide to reproduce the issue
- **Proof of concept** — Code snippets, screenshots, or a working PoC (if available)
- **Suggested fix** — If you have a recommendation for how to fix it (optional but appreciated)
- **Your contact info** — So we can follow up with you

### ⏱️ Response Timeline

We are committed to responding promptly to all security reports:

| Milestone                        | Target Timeframe     |
| -------------------------------- | -------------------- |
| Initial acknowledgement          | Within **48 hours**  |
| Triage & severity assessment     | Within **5 days**    |
| Status update to reporter        | Every **7 days**     |
| Patch development & testing      | Within **30 days**\* |
| Public disclosure (coordinated)  | Within **90 days**   |

> \* Complex vulnerabilities may require additional time. We will communicate any delays directly to the reporter.

---

## Vulnerability Severity Levels

We classify vulnerabilities using the [CVSS v3.1](https://www.first.org/cvss/v3.1/specification-document) scoring system:

| Severity | CVSS Score | Response Priority      |
| -------- | ---------- | ---------------------- |
| Critical | 9.0 – 10.0 | Immediate (hotfix)     |
| High     | 7.0 – 8.9  | Within 14 days         |
| Medium   | 4.0 – 6.9  | Within 30 days         |
| Low      | 0.1 – 3.9  | Next scheduled release |

---

## What to Expect After Reporting

1. **Acknowledgement** — You'll receive a confirmation that we received your report within 48 hours.
2. **Assessment** — Our security team will analyze the report and determine severity and impact.
3. **Accepted** — If accepted, we will work on a fix and keep you updated on progress. You will be credited in the release notes (unless you prefer anonymity).
4. **Declined** — If the issue is determined not to be a vulnerability or is out of scope, we will explain our reasoning clearly.
5. **Coordinated Disclosure** — Once a fix is released, we will work with you to coordinate public disclosure timing.

---

## Security Update Process

- Security patches are released as **patch versions** (e.g., `5.1.0` → `5.1.1`)
- Critical vulnerabilities may receive **out-of-band hotfix releases**
- All security-related releases are tagged with `[SECURITY]` in the [CHANGELOG](./CHANGELOG.md)
- Users are notified via [GitHub Security Advisories](../../security/advisories) and release notes

---

## Scope

### In Scope
- Vulnerabilities in the core codebase of this repository
- Authentication and authorization bypasses
- Remote code execution (RCE)
- SQL/NoSQL injection
- Cross-site scripting (XSS) and cross-site request forgery (CSRF)
- Sensitive data exposure
- Dependency vulnerabilities with direct exploitability

### Out of Scope
- Vulnerabilities in third-party services or dependencies (please report those upstream)
- Issues in unsupported versions
- Social engineering attacks targeting our team or users
- Denial of service (DoS) attacks
- Reports from automated scanners without proof of exploitability
- Issues requiring physical access to a user's device

---

## Bug Bounty Program

At this time, we do **not** operate a paid bug bounty program. However, we deeply value the contributions of security researchers and offer:

- Public credit in the security advisory and release notes
- A mention in our [Hall of Fame](#hall-of-fame) below
- Swag / merchandise for critical findings *(at maintainer discretion)*

---

## Hall of Fame

We thank the following researchers for responsibly disclosing vulnerabilities:

| Researcher         | Year | Severity | Advisory          |
| ------------------ | ---- | -------- | ----------------- |
| *(Your name here)* | —    | —        | —                 |

> Want to be listed here? Follow our responsible disclosure process above.

---

## Security Best Practices for Users

To keep your deployment secure, we recommend:

- **Always upgrade** to the latest supported version
- **Review our [CHANGELOG](./CHANGELOG.md)** for security-related updates
- **Enable dependency auditing** (e.g., `npm audit`, `pip audit`, Dependabot)
- **Follow the principle of least privilege** when configuring permissions
- **Monitor [GitHub Security Advisories](../../security/advisories)** for this repo by clicking **Watch → Security alerts**

---

## Legal

We operate under a **responsible disclosure** model. We will not pursue legal action against researchers who:

- Report vulnerabilities privately and give us reasonable time to remediate
- Do not exploit the vulnerability beyond what is necessary to demonstrate it
- Do not access, modify, or delete user data
- Act in good faith and comply with this policy

---

## Contact

| Purpose             | Contact                                                      |
| ------------------- | ------------------------------------------------------------ |
| Security issues     | security@yourproject.com                                     |
| General inquiries   | hello@yourproject.com                                        |
| Maintainer (GitHub) | [@yourusername](https://github.com/yourusername)             |

---

*This security policy was last updated: March 2026*
