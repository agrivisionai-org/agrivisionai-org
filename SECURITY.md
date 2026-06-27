# Security Policy

AGRIVISION AI builds AI-powered agricultural intelligence used by extension workers and farmers across 40+ countries. The trust of those users -- many of whom are first-time internet users operating in low-connectivity environments -- is something we take seriously. If you've found a security issue in any of our systems, thank you for helping us protect them.

## Supported Versions

We provide security updates for the following:

| Product / Surface | Supported |
| --- | --- |
| YieldAI Global (production) | Yes |
| YieldAI Global (staging / preview builds) | Yes |
| Public APIs at `*.agrivisionai.org` | Yes |
| Open-source repositories under `github.com/agrivisionai-org` (latest `main`) | Yes |
| Archived or deprecated repositories (marked as such on GitHub) | No |

## Reporting a Vulnerability

Please report suspected vulnerabilities privately to **security@agrivisionai.org**.

Include, where possible:

- A clear description of the issue and its impact
- Steps to reproduce, or a proof-of-concept
- The affected product, URL, repository, or commit
- Your name or handle for credit (optional)

PGP-encrypted reports are welcome on request -- email us first and we'll share a key.

## Our Response Commitment

- **Acknowledgement:** within **48 hours** of receipt.
- **Initial triage and severity assessment:** within **5 business days**.
- **Fix for critical vulnerabilities:** within **30 days** of confirmation.
- **Fix for high / medium / low severity:** prioritized and communicated on a case-by-case basis.

We'll keep you updated throughout, and credit you in our release notes or a published advisory if you'd like.

## Coordinated Disclosure

We follow a **90-day coordinated disclosure window** from the date a report is confirmed. We ask that you do not publicly disclose details -- including blog posts, social media, conference talks, or write-ups -- until the earlier of: a fix being released, or 90 days elapsing. If more time is needed, we'll work with you in good faith to extend it.

## Out of Scope

To keep our farmer users safe, please **do not**:

- Run denial-of-service, load, or stress tests against our infrastructure
- Attempt social engineering of AGRIVISION AI staff, contractors, or users
- Access, modify, or exfiltrate data belonging to other users
- Test against production accounts you do not own
- Perform physical attacks against our offices or staff
- Spam our forms, endpoints, or email systems as part of testing

Findings limited to missing best-practice headers, outdated library versions without a working exploit, or theoretical issues without demonstrated impact are generally considered informational rather than vulnerabilities.

## Safe Harbor

If you act in good faith, stay within this policy, and make a reasonable effort to avoid privacy violations and service disruption, we will not pursue legal action against you for your research. We treat researchers as partners.

---

Questions about this policy: **security@agrivisionai.org**
General contact: **hello@agrivisionai.org**
