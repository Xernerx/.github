<!-- @format -->

![Xernerx Banner](https://www.xernerx.com/banner.png)

# Security Policy (`SECURITY.md`)

**Xernerx Studios** takes the security of the **Xernerx Suite**, our Discord applications, open-source NPM frameworks, and community data seriously. This organization-wide policy outlines our supported versions, security architecture, and how to responsibly disclose vulnerabilities.

For our full interactive Security & Licensing overview, visit **[https://xernerx.com/security](https://xernerx.com/security)**.

---

## 🛡️ Supported Versions & Ecosystem Scope

Security updates and patches are actively applied to the latest **Production (`latest`)** and **Canary (`canary`)** deployments across our ecosystem:

| Target / Workspace                                                                                                                                                                                                                            | Supported Versions         | Security Updates |
| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------- | :--------------- |
| **Xernerx Web Suite** (`*.xernerx.com` — `www`, `app`, `account`, `portal`, `store`, `docs`, `info`, `blog`, `admin`, `hosting`)                                                                                                              | Production & Canary (`v5`) | ✅ Active        |
| **Core Backend & Media** (`api.xernerx.com`, `cdn.xernerx.com`, `haste.xernerx.com`, `services/websocket`)                                                                                                                                    | `/v1/*`, `/secure/*`, `ws` | ✅ Active        |
| **Xernerx Desktop & Mobile Clients** (`clients/desktop`, `clients/mobile` — Stable & Canary channels)                                                                                                                                         | `>= 2.x`                   | ✅ Active        |
| **Official Discord Bots** (`Virtue`, `Metamorphosis`, `Zodiac`, `To-Do List Bot`, `Xernerx App`, `Xernerx Bot`)                                                                                                                               | Current Hosted Production  | ✅ Active        |
| **Open-Source SDKs, Examples & Docs** (`xernerx`, `@xernerx/framework`, `@xernerx/commands`, `@xernerx/extension-builder`, `@xernerx/hooks`, `@xernerx/stats`, `@xernerx/terminal`, `@xernerx/websocket`, `Xernerx/examples`, `Xernerx/docs`) | Latest Minor Release       | ✅ Active        |
| **Legacy / Deprecated Generations** (`v1` – `v4`)                                                                                                                                                                                             | `< 5.0.0`                  | ❌ End of Life   |

---

## 🚨 Reporting a Vulnerability (Responsible Disclosure)

> **Please do NOT report security vulnerabilities through public GitHub issues, pull requests, public Discord channels, or `info.xernerx.com`.**

If you discover a security vulnerability anywhere in the Xernerx ecosystem, please report it privately to our security team:

- **Email:** **[security@xernerx.com](mailto:security@xernerx.com)**
- **Contact Page:** [https://xernerx.com/contact](https://xernerx.com/contact)

### What to Include in Your Report

To help us triage and resolve the issue as quickly as possible, please include:

1. **Affected Component:** The specific subdomain (e.g., `api.xernerx.com`, `portal.xernerx.com`, `haste.xernerx.com`), bot (`Virtue`, `Xernerx App`), Desktop Client version, or NPM package (`@xernerx/*`).
2. **Vulnerability Type:** e.g., authentication/authorization bypass, IDOR, SSRF, XSS, CSRF, token leakage, or privilege escalation.
3. **Step-by-Step Reproduction:** Clear instructions, HTTP request/response samples, or a minimal proof-of-concept (PoC) demonstrating the issue.
4. **Impact Assessment:** What an attacker could realistically achieve and which privacy tier (`public`, `limited`, or `private`) is affected.

---

## ⏱️ Response Timeline & Disclosure Process

When you submit a report to **[security@xernerx.com](mailto:security@xernerx.com)**, you can expect:

- **Within 24–48 Hours:** Confirmation that we have received your report and assigned it for investigation.
- **Within 72 Hours:** Initial triage, severity classification, and verification of the reproduction steps.
- **Remediation & Verification:** We will develop and test a fix in our isolated Canary environment (or publish a patched NPM release) before shipping to Production and notifying you so you can verify the patch.

---

## 🤝 Safe Harbor & Rules of Engagement

Xernerx Studios supports good-faith security research. We will not pursue legal action or suspend accounts of researchers who adhere to these guidelines:

- **Test Only Against Your Own Accounts:** Use your own Discord/Xernerx test accounts, bots, organizations, and servers when testing permissions or privacy boundaries.
- **Respect User Privacy (`public` | `limited` | `private`):** Never attempt to view, modify, download, or exfiltrate private user profiles, private CDN blobs (`cdn.xernerx.com/raw/*`), private Haste pastes (`haste.xernerx.com`), or third-party API tokens/webhook secrets. If you encounter unauthorized data during testing, stop immediately and report the finding.
- **No Service Disruption:** Do not perform Denial-of-Service (DoS/DDoS) attacks, automated rate-limit exhaustion, spam floods against Discord webhooks, or social engineering/phishing against Xernerx staff or users.

---

## 🔒 Platform Security & Licensing Links

- **Security Overview:** [https://xernerx.com/security](https://xernerx.com/security)
- **Software & SaaS Licensing:** [https://xernerx.com/license](https://xernerx.com/license)
- **Terms of Service:** [https://xernerx.com/terms](https://xernerx.com/terms)
- **Privacy Policy:** [https://xernerx.com/privacy](https://xernerx.com/privacy)
- **Cookie Policy:** [https://xernerx.com/cookies](https://xernerx.com/cookies)
