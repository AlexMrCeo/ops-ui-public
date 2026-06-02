# Ops UI

Ops UI is an AI-native operations interface for turning scattered signals, tasks, automations, and system context into one clear command surface.

It is designed as a lightweight foundation for internal dashboards, agent control panels, operational workflows, and coordination tools around real products or teams.

The public repository focuses on the interface model, architecture, and integration boundaries. Production deployments can connect their own APIs, databases, agents, automations, and infrastructure through environment variables and external secret management.

## Core Ideas

- One command surface for operational context
- Clear separation between public interface patterns and private deployment details
- Environment-driven integrations
- Safe defaults for sharing architecture without exposing infrastructure
- Agent-friendly documentation and operating boundaries

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

## Security

Security rules and reporting guidance live in [SECURITY.md](SECURITY.md).

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
