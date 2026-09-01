# Security Policy

This is the default security policy for repositories in the
[GMEDIA](https://github.com/gmedia) organization. Individual repositories may
publish their own `SECURITY.md` with a narrower scope or additional contacts —
where they do, that file takes precedence.

## Please do not use public issues

**Do not report security vulnerabilities through public GitHub issues, pull
requests, or discussions.**

A public report exposes the issue to everyone before a fix exists, including
users of the affected system. Report privately and give us a chance to fix it
first.

## How to report

**Preferred — GitHub private vulnerability reporting.** Open the affected
repository, go to the **Security** tab, and choose **Report a vulnerability**.
This creates a private advisory visible only to the maintainers and keeps the
whole exchange in one place.

**If private reporting is not enabled on that repository**, contact GMEDIA
through the official channels listed at <https://gmedia.id/contact> and ask to
be routed to the engineering team responsible for the repository. Please state
that the message concerns a security vulnerability, and do not include the
technical details until you are in contact with that team.

If you encounter an address presented as a GMEDIA security contact, verify it
against <https://gmedia.id> before sending anything sensitive.

## What to include

The more of this you can provide, the faster we can triage:

- The affected repository or project, and the affected version, tag, or commit.
- A description of the vulnerability and the underlying weakness.
- Step-by-step reproduction instructions, or a proof of concept.
- The impact you believe it has — what an attacker gains.
- Any suggested mitigation or fix, if you have one.
- Your environment, where it is relevant to reproducing the issue.

**Remove sensitive data before sending.** Redact credentials, API keys, tokens,
personal data, and customer information from logs, screenshots, and proof-of-
concept output. Send the minimum needed to demonstrate the issue.

## Testing boundaries

Please confine your testing to systems you are entitled to test — your own
deployment, or a local instance you control.

Do not test against GMEDIA production systems, customer environments, or
third-party infrastructure. Do not access, modify, or exfiltrate data that is
not yours, and do not run denial-of-service, spam, or social-engineering tests.

## What happens next

We will acknowledge your report and work with you on the details, remediation,
and the timing of any public disclosure.

Please keep the report private until a fix is available and disclosure has been
coordinated with us.

We do not offer a bug bounty, and we do not publish guaranteed response or
remediation timelines. Projects in this organization are at different stages of
maturity — some are explicitly early-stage foundations rather than production
systems — and we would rather set no expectation than one we cannot meet
consistently.

If you would like credit for a report, tell us how you want to be named. If you
prefer to stay anonymous, that is fine too.
