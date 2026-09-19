# Security Guidance

This repository is a lab/portfolio project for identity lifecycle automation. It must not contain production credentials, employer data, real employee records, internal domain information or proprietary directory exports.

## Safe development rules

- Use synthetic users, departments, groups and ticket references only.
- Never commit passwords, API keys, tokens or connection secrets.
- Use environment variables or secret stores for any future integrations.
- Keep destructive operations behind dry-run/preview behaviour wherever possible.
- Require explicit execution for account/group changes.
- Log security-sensitive changes without logging passwords or secret values.
- Validate role configuration before touching Active Directory.
- Use least-privilege accounts in the lab and in any future production design.

## Production considerations

A production implementation would also require protected audit logs, formal approval workflows, secrets management, privileged access controls, change-management integration, rollback procedures and monitoring for unauthorised role-map changes.

## Reporting issues

If this repository is ever extended with real external integrations, security issues should be reported privately rather than by publishing credentials or exploitable details in a public issue.
