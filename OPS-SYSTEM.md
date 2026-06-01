# Ops UI System Notes

Ops UI is a public-safe operations dashboard template. A private deployment can connect it to internal APIs, databases, schedulers, and notification channels.

## Design Principles

- Keep secrets out of git.
- Keep private infrastructure details out of public docs.
- Prefer explicit configuration through environment variables.
- Treat public documentation as a product overview, not an internal runbook.
- Rotate credentials if they were ever committed to git history.

## Suggested Modules

- `Dashboard`: status, alerts, and recent activity
- `Tasks`: follow-up items and approvals
- `Integrations`: configured external services
- `Settings`: safe local configuration checks

## Deployment Notes

Deployments should use environment variables or a managed secret store. Public examples should use placeholders only.

Do not publish:

- Real production URLs
- Database URLs
- API tokens
- OAuth secrets
- Bot tokens or chat IDs
- Personal schedules or routines
- Private team or customer information
