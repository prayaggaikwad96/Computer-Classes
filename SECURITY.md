# Security Policy

## Supported versions

The default branch, `main`, is the maintained version of this learning archive. Historical branches and snapshots are retained for reference and recovery; they are not guaranteed to receive updates.

## Reporting a vulnerability

Please do not publish credentials, tokens, personal data, exploit details, or a working exploit in a public issue or pull request.

Use GitHub's **Report a vulnerability** option in the repository's **Security** tab when private vulnerability reporting is available. Otherwise, contact the repository owner through their GitHub profile and request a private disclosure route.

Include the affected path or component, the potential impact, safe reproduction steps, and a suggested mitigation when known. Do not test against systems or data you do not own or have explicit permission to assess.

## Secrets

Never commit secrets. If a credential is exposed, revoke or rotate it immediately; deleting the file or commit alone does not invalidate the credential.
