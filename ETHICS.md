# Responsible automation policy

This is the standard I hold my public work to. It is intentionally short.

## What I ship

- **Local-first by default.** Tools must work without an account, a cloud service, or a network connection.
- **No telemetry.** No analytics, crash reporting, or usage pings unless a user explicitly opts in.
- **No credential exfiltration.** Secrets stay on the machine that owns them. Tools may read a credential to perform a local action; they must never transmit it to a third party.
- **Security is documented.** Every project with a network surface ships a `SECURITY.md` and a threat model.
- **Honest READMEs.** If a package is not published, the README says so. If a feature is experimental, it is labeled.
- **OSI-approved licenses.** Public tools use Apache-2.0, MIT, or GPL-3.0 where an upstream license requires it. Custom "open source" licenses are not used.

## What I do not ship

- Self-bots, token harvesters, or automation that violates a platform's terms of service.
- Fake engagement, fake download counts, fake stars, or purchased metrics.
- Tools that impersonate another product or hide their data flow.
- "Growth hacks" that require a user to join a server, follow an account, or hand over a token to unlock basic functionality.

## Discord and WhatsApp automation

Bots that connect through official bot APIs are fine. User-account automation is not. Projects that touch unofficial APIs must carry a prominent warning, must not be promoted as flagship work, and must be archived when they no longer serve a legitimate purpose.

## Reporting

If a project of mine violates this policy, open a private security advisory on the repository or contact me through GitHub. I will fix or archive it.
