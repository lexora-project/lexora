# Security Policy

The canonical security policy for Lexora is published at:

**[https://lexora.sh/security](https://lexora.sh/security)**

## Reporting a Vulnerability

**Please do not post security vulnerabilities publicly** — including in GitHub Issues, pull requests, or public forums.

Report security-sensitive findings privately by emailing:

**[lexora.dev@proton.me](mailto:lexora.dev@proton.me)**

Include a description of the issue, reproduction steps, and any relevant environment details. We will acknowledge receipt and work to address confirmed vulnerabilities promptly.

## Security-Relevant Areas

The following areas of Lexora are particularly security-sensitive:

- **Provider routing** — how requests are dispatched to translation providers, cloud AI, and user-configured endpoints
- **Selected-text handling** — how user-selected content is captured, processed, and transmitted
- **Extension message boundaries** — communication between the extension's content scripts, background service worker, and popup
- **Token and key leakage** — handling of API keys and tokens provided by the user
- **Settings and privacy bypasses** — scenarios where user privacy preferences could be circumvented

If you are uncertain whether a finding is security-relevant, err on the side of reporting it privately.
