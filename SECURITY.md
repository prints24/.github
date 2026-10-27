# Super91 Security Policy

Super91 takes the security of our platform, user credentials, customer artworks, and production systems very seriously. We appreciate the responsible disclosure of any potential vulnerabilities.

---

## 🛡️ Supported Versions

We actively provide security updates and patches for the following versions:

| Version / Branch | Supported | Notes |
|---|---|---|
| `v1.1` | :white_check_mark: Yes | Primary active production release (`super91.com`) |
| `main` | :x: No | Legacy / Inactive branch (not in active use) |
| Older releases | :x: No | Please upgrade to the latest active release (`v1.1`) |

---

## 🚨 Reporting a Vulnerability

**Please DO NOT report security vulnerabilities through public GitHub issues or public discussions.**

Instead, report vulnerabilities through one of the following secure channels:

### Option 1: GitHub Private Vulnerability Reporting (Recommended)
1. Navigate to the repository's **Security** tab on GitHub.
2. Under "Reporting", click **Report a vulnerability**.
3. Provide details of the finding and submit privately to our security team.

### Option 2: Direct Email
Send an encrypted or confidential email to:
* **Email:** [support@super91.com](mailto:support@super91.com)
* **Subject line:** `[SECURITY] Potential vulnerability in <repository/subsystem>`

---

## 📋 What to Include in Your Report

To help us triage and resolve the issue quickly, please provide:
* **Description:** A clear summary of the issue and potential impact.
* **Component Affected:** Target repository, branch, API route, or frontend component.
* **Steps to Reproduce:** Step-by-step instructions or proof-of-concept (PoC) code.
* **Expected vs Actual Behavior:** What happened vs what was expected.
* **Suggested Remediation:** Any proposed fix or mitigation (if available).

---

## ⏱️ Response Timelines & SLA

Our engineering and security team commits to the following schedule:

| Milestone | Target Response Time |
|---|---|
| **Initial Acknowledgment** | Within 24 to 48 hours |
| **Triage & Severity Assessment** | Within 3 to 5 business days |
| **Patch Release & Verification** | Priority P0 (within 24-72 hours), P1 (within 7 days) |
| **Public Disclosure Coordination** | Coordinated only after the patch is deployed and verified |

---

## 🤝 Responsible Disclosure Guidelines

* Give us reasonable time to investigate and resolve the issue before disclosing it to the public or any third party.
* Do not access, modify, or delete customer data, order files, or production databases.
* Avoid denial of service (DoS), automated high-volume stress testing, or disruption of production services.
