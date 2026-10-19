# Security Policy

This is an early-stage prototype. Do not submit sensitive personal or business data to it.

## Reporting a concern
Contact the project maintainer through the [SNTL 84 GitHub profile](https://github.com/SNTL84). Include a concise description and safe reproduction steps. Do not publish credentials, tokens, or personal information in issues.

## Development safeguards
- Never commit secrets or production credentials.
- Keep local environment files out of Git.
- Treat public listing submissions as untrusted until reviewed.
- Before adding authentication or data storage, define access rules and test them.
- Use server-side controls for privileged operations; frontend checks alone are not authorization.
