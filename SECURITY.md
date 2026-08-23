# Security Policy

Nexus is closed-source desktop software. This repository does not contain
application source code, so standard code-scanning/pull-request-based
disclosure doesn't apply here — but we still want to hear about security
issues in the app, our infrastructure, or our website.

## Reporting a Vulnerability

**Please do not open a public GitHub issue for security vulnerabilities.**
Public issues are visible to everyone immediately, including before a fix
ships.

Instead, email **security@getnexus.app** (or getnexusupport@gmail.com if
that inbox isn't live yet) with:

- A description of the issue and its potential impact
- Steps to reproduce, or a proof of concept if you have one
- The Nexus version and OS you tested on
- Whether you're aware of it being publicly known or exploited

## What to expect

| Stage | Timeline |
|---|---|
| Acknowledgement of your report | Within 3 business days |
| Initial assessment / severity triage | Within 7 business days |
| Fix or mitigation, for confirmed issues | Varies by severity — critical issues are prioritized |
| Public disclosure | Coordinated with you, after a fix ships |

We'll credit reporters (with permission) in the release notes once a fix
ships, unless you'd prefer to stay anonymous.

## Scope

**In scope:**
- The Nexus desktop application (all platforms)
- getnexus.app and any subdomains
- Update/download infrastructure

**Out of scope:**
- Social engineering, physical attacks, or attacks requiring physical
  access to a user's device
- Denial of service via resource exhaustion
- Issues in third-party dependencies with no demonstrated path to
  impacting Nexus itself (please report those upstream instead)

Thanks for helping keep Nexus and its users safe.
