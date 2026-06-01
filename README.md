# Ops UI

Ops UI is a public template for a lightweight operations dashboard. It is intended to help teams collect operational signals, review alerts, and coordinate follow-up actions without exposing private infrastructure details.

This repository contains public-safe documentation and configuration examples only. Real deployment URLs, service identifiers, credentials, private schedules, and internal workflows must be configured outside git.

## What This Project Covers

- Dashboard and API concepts for operational visibility
- Environment variable examples with placeholders
- Security guidance for keeping private deployments safe
- High-level architecture notes that can be adapted to a private system

## Configuration

Copy `.env.example` to `.env` locally and replace placeholder values with your own credentials.

Never commit `.env` files or real secrets.

## Required Environment Variables

- `SUPABASE_URL`
- `SUPABASE_ANON_KEY`
- `HERMES_URL`
- `OPS_API_URL`
- `OPS_API_TOKEN`

See `.env.example` for placeholder values.

## Security

Read [SECURITY.md](SECURITY.md) before deploying or connecting this project to real services.
