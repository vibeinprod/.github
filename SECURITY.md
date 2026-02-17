# Security Policy

VibeInProd takes security seriously. If you believe you’ve found a security vulnerability, please report it responsibly.

## Supported Versions

Unless otherwise stated in a repository, only the **default branch** (typically `main`) is considered supported for security fixes.

## Reporting a Vulnerability

Please **do not** open a public GitHub issue for security vulnerabilities.

Instead, report privately using one of the following:

- **Email:** security@vibeinprod.com  
- If email is not available, use the repository’s **Private vulnerability reporting** feature (if enabled).

Include as much of the following as possible:

- A clear description of the issue and potential impact
- A minimal proof-of-concept (PoC), if available
- Steps to reproduce
- Affected components (endpoints, modules, versions, commits)
- Any relevant logs, screenshots, or crash traces
- Your assessment of severity (if you have one)

### Sensitive Data

Please **avoid** sending:
- Real user data
- Secrets (API keys, private keys, access tokens)
- Proprietary source code beyond what is required to demonstrate the issue

If secrets were accidentally included, rotate them immediately and mention what was rotated.

## Response Timeline

We aim to:
- Acknowledge receipt within **3 business days**
- Provide a status update within **7 business days**

Complex issues may take longer. If you have a coordinated disclosure timeline, include it in your report.

## Coordinated Disclosure

We prefer coordinated disclosure and will work with you on:
- Patch development
- Release timing
- Credit (optional)

Please do not disclose publicly until a fix is available or we’ve agreed on a timeline.

## Scope

This policy covers:
- Vulnerabilities in code within this organization’s repositories
- Build pipelines and release artifacts where applicable

Out of scope (unless explicitly stated by a repo):
- Social engineering, phishing, or physical attacks
- Denial of service (volumetric) testing
- Vulnerabilities requiring compromised devices/accounts unless they demonstrate a repo-specific issue

## Security Hardening Expectations (For Contributors)

If you are contributing code, please ensure:
- No secrets are committed (use env vars and secret managers)
- Dependencies are reviewed and kept minimal
- Inputs are validated and output is encoded appropriately
- AuthZ decisions are explicit and tested (deny-by-default)
- Risky changes include a threat model note in the PR

Thank you for helping keep our software safe.
