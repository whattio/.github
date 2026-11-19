# Contributing to whatt.io / Asgaard Open Source

Thank you for contributing to the **whatt.io / Asgaard** open-source ecosystem!

## Licensing & Contributor License Agreement (CLA)

Repositories in the `whattio` organization are dual-licensed under **GNU AGPLv3** and a **Commercial License** (see [`COMMERCIAL-LICENSE.md`](./COMMERCIAL-LICENSE.md)).

- Before we can merge any external pull request, you must sign our **Contributor License Agreement (CLA)** via the automated PR check.
- You retain copyright to your contributions while granting **Asgaard Technology / whatt.io** the rights necessary to distribute your contribution under both AGPLv3 and our commercial license.

## Contribution Guidelines

1. **Keep it sovereign & standalone:** Do not introduce mandatory cloud API dependencies, telemetry beacons, or proprietary endpoints. Everything must work cleanly offline/air-gapped.
2. **Preserve MCP compatibility:** Any new core capability should be exposed cleanly via `/api/mcp` with strict input/output JSON schemas and unit tests.
3. **Zero secrets or real customer data:** Use only synthetic fixtures in tests and sample files.
4. **Third-party dependencies:** Only add dependencies with AGPLv3-compatible open-source licenses and update `NOTICE` if attribution is required.

## Pull Request Checklist

- [ ] `docker compose up --build` starts cleanly with default `.env.example` values.
- [ ] All unit tests and `/api/mcp` smoke tests pass.
- [ ] `asgaard.app.json` remains valid JSON and reflects any new ports/mounts/contracts.
- [ ] CLA check is signed and green.
