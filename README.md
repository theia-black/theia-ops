# theia-ops

Theia's operational infrastructure — GitHub Actions workflows for periodic jobs, monitoring, and automation.

All workflows hit the public API at https://theia.theiasystems.co.uk with token auth. No localhost, no local dependencies. Boundless.

## Architecture

- **GCP (stateful):** Brain, neural-signal, Discord, gateway, web apps — persistent connections
- **GitHub Actions (stateless):** Cron jobs, health checks, digest pipelines, embed processing — run and exit

## Secrets Required

- BRAIN_TOKEN — X-Brain-Token for brain API auth
