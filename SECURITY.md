# Internal Security Guidelines

This document outlines security best practices for all LinkCXO engineering team members.

## 🔐 Credentials & Secrets

1. **Zero Hardcoded Secrets**: Never commit `.env` files, API tokens, database connection strings, JWT secrets, or private keys to any repository.
2. **Environment Variables**: Use Doppler / AWS Secrets Manager / GitHub Organization Secrets for injecting runtime credentials into CI/CD pipelines.
3. **Pre-commit Checks**: Run local linters or tools like `git-secrets` / `trufflehog` to catch accidental secret commits before pushing.
4. **Credential Rotation**: If a key or token is accidentally pushed to Git, report it immediately to the DevOps lead and rotate the compromised credential across all environments.

## 🛡️ Repository & Access Standards

- **Branch Protection**: Direct pushes to `main` and `production` branches are strictly disabled. All changes must go through a pull request with at least one approved code review.
- **Access Control**: Repository access is strictly managed via GitHub Teams and principle of least privilege.
- **Dependency Auditing**: Regularly run dependency scans (`npm audit`, `pip-audit`, etc.) to remediate vulnerable third-party packages.

## 🚨 Incident & Vulnerability Reporting

If you identify a security issue, exposed credential, or critical system vulnerability:
- **Do not** discuss it in public channels.
- Notify the Tech Lead and DevOps team immediately via the `#security-alerts` internal channel.
