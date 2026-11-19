# Security Policy

## Reporting a Vulnerability

Please **do not** open a public GitHub issue for security vulnerabilities.

Instead, report vulnerabilities privately via:
- **GitHub Security Advisories** ("Report a vulnerability" in the Security tab of the affected repository), or
- **Email:** `security@whatt.io` (or `info@whatt.io` with subject `[SECURITY] whattio/<repo>`)

Please include:
1. Affected repository, version, or commit SHA
2. Reproduction steps or proof of concept
3. Potential impact (especially any air-gap egress bypass, MCP tool injection, or file-path traversal)

We aim to acknowledge reports within **48 hours** and provide a remediation timeline within **5 business days**.

## Sovereign & Air-Gap Security Invariants

All applications in the `whattio` organization are designed to run inside air-gapped corporate environments and Asgaard Sovereign Enclaves:
- No silent outbound telemetry or phone-home requests.
- Strict input validation on all `/api/mcp` JSON-RPC tool arguments.
- Uploaded BOMs, PDFs, images, and DPP payloads are processed locally without external transmission unless explicitly configured by the operator.
