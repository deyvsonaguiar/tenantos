# Deployment Notes

This repository is intended to support a Docker-based deployment of TenantOS.

## Runtime expectations
- Node/Next application exposed internally on port `3000`
- Reverse proxy expected in front of the app for HTTPS in production
- OpenClaw data mounted read-only into the container
- Secrets injected at runtime through environment variables

## Keep out of this repository
Do not commit:
- real `ADMIN_PASSWORD`
- real `AUTH_SECRET`
- host-specific private paths that are not safe to publish
- incident notes or operational secrets

## Private operations repository
Operational deployment state, validated compose files, troubleshooting history, and infrastructure notes are tracked in the private repository:

`https://github.com/deyvsonaguiar/tenantos-ops`
