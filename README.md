# Ops UI

This repository is a public-safe template/reference for an AI-native operations interface.

It provides generic documentation and configuration examples for an operations UI without exposing private infrastructure, production endpoints, real credentials, personal schedules, private workflows, or internal service identifiers.

## What This Is

- A public-safe reference for an operations interface.
- A concise starting point for dashboards, operational signals, and coordination surfaces.
- A template that private deployments can adapt with their own application code, services, and secrets.

## What This Is Not

- It is not a production deployment.
- It does not include real credentials, production endpoints, private schedules, private workflows, or personal data.
- It does not define a complete application stack. Use the package manager configured by your application.

## Quick Start

```bash
git clone https://github.com/AlexMrCeo/ops-ui-public.git
cd ops-ui-public
cp .env.example .env.local
npm install
npm run dev
```

If the actual package manager differs, use the one configured by the application.

## Environment Variables

Copy `.env.example` to a local env file and replace placeholders with values for your own deployment:

- `SUPABASE_URL`
- `SUPABASE_ANON_KEY`
- `HERMES_URL`
- `OPS_API_URL`
- `OPS_API_TOKEN`

Real deployments should configure secrets via environment variables or the hosting provider's secret manager.

## Security / Public-Safe Boundaries

This repository must not include:

- Production endpoints
- Real credentials or tokens
- Private keys
- Bot tokens or chat IDs
- Personal schedules
- Private workflows
- Internal service identifiers
- Private architecture details
- Personal data

Any real credential that was ever committed should be rotated.

## Repository Structure

```text
.
├── .env.example
├── .github/workflows/secret-scan.yml
├── AGENTS.md
├── CONTRIBUTING.md
├── LICENSE
├── OPS-ARCHITECTURE.md
├── OPS-SYSTEM.md
├── OPS-VISION.md
├── README.md
└── SECURITY.md
```

## License

MIT. See [LICENSE](LICENSE).
