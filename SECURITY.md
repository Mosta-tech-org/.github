# MosTa‑TecH Security Policy

Security is a core engineering requirement for MosTa‑TecH platforms.

## Reporting vulnerabilities

Do not report security vulnerabilities through public GitHub Issues.

Use GitHub Private Vulnerability Reporting when enabled for the affected repository.

If private reporting is unavailable, contact the authorized MosTa‑TecH repository owner privately.

## Never publish

Do not include any of the following in Issues, Pull Requests, Discussions or screenshots:

- passwords;
- API keys;
- access tokens;
- Supabase secret keys;
- database credentials;
- customer personal information;
- prescription documents;
- payment evidence;
- private business information;
- production database exports.

## Supported versions

Security support normally applies to:

1. the current production release;
2. the current `main` branch.

Older releases may no longer receive security updates.

## Security-sensitive areas

Changes involving the following require additional review:

- authentication;
- authorization;
- PostgreSQL RLS;
- Supabase Storage;
- payment verification;
- prescription workflows;
- inventory accounting;
- branch isolation;
- audit logging;
- AI tool permissions;
- deployment credentials;
- GitHub Actions;
- production environment variables.

## Credential exposure

If a credential is accidentally exposed:

1. revoke it immediately;
2. create a replacement;
3. update production environments;
4. inspect audit logs;
5. determine the exposure window;
6. document the incident privately;
7. remove the secret from Git history where appropriate.

Deleting a secret from the latest commit is not sufficient after it has been pushed.

## Production principles

Production systems should use:

- least privilege;
- MFA for privileged accounts;
- RLS;
- private storage for sensitive documents;
- encrypted transport;
- secure cookies;
- audit logging;
- dependency monitoring;
- protected branches;
- reviewed deployments;
- tested backups.
