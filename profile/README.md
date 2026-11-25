# whatt.io — Open-Source Ecosystem for Asgaard, Citadel & IronPass

> **Asgaard is the Sovereign Agentic OS & MCP Fabric that turns any open-source app into an agent-driven, DPP-connected workspace citizen—running on hardware you own.**
>
> **Citadel** is the Sovereign Zero-IP Linux Security Fabric, **BIFROST** is the Reticulum Ghost Browser connecting worlds with 0 open ports, and **IronPass** nails physical hardware identity and GS1 EPCIS 2.0 ledgers into iron.

---

### Core Focus Areas
- **Digital Product Passports (DPP):** EU ESPR (Regulation (EU) 2024/1781), CIRPASS-2 JSON-LD, GS1 Digital Link, GS1 EPCIS 2.0, Substances of Concern (SoC), and Critical Raw Materials (CRM) compliance tooling.
- **Zero-IP Sovereign Networking (Reticulum + BIFROST):** Closing *"The Last-Meter Leak"* in CIRPASS-2 & EU ESPR — end-to-end encrypted **512-bit Curve25519 (X25519 + Ed25519)** links across untrusted Fiber, Starlink, 5G & Sub-GHz LoRa with **0 open server ports, 0 local HTTP sockets, 0 DNS, and 0 cookies**.
- **Product Content Management (PCM):** Sovereign, AI-ready product data harvesting, structured BOM & specification management, 3D/visual pipelines, and verifiable integrity proofs.
- **Native MCP Everywhere:** Every app we ship exposes a clean HTTP JSON-RPC `/api/mcp` endpoint so it runs completely standalone today—or snaps straight into **Asgaard Agentic OS** and your own AI agent workflows.

---

### Sovereign Zero-IP Architecture: Reticulum, Citadel, BIFROST & IronPass

> **“Verifiable Credentials protect the passport. Chrome leaks the mission.”**

Standard HTTPS browsers expose DNS queries, IP addresses, TLS SNI hostnames, cookies, and public server ports (`:443`)—revealing pattern-of-life metadata even when DPP payloads are signed. Our 4-pillar architecture eliminates that last-meter leak while staying **100% compatible with EU ESPR & GS1 EPCIS 2.0**:

| Pillar | Role | What It Does |
| :--- | :--- | :--- |
| **ASGAARD** | Sovereign Agentic AI OS | Orchestrated by **Heimdall**, forged by **Andvari, Brokk & Sindri**, housing **Sessrumnir** & **Gladsheim** spatial vaults. |
| **CITADEL** | 0-Port Linux Security Fabric | Turns any hardened Debian/Ubuntu Linux server (micro-server to multi-GPU AI cluster) into an invisible 0-port Reticulum fortress (`nftables` DROP inbound). |
| **BIFROST** | *The Reticulum Ghost Browser* | 5 MB clean-room Rust browser (`bifrost://` & `ironpass://`) with **0 local HTTP ports, 0 DNS, 0 cookies**, RAM-only incognito sessions, local Rust Ed25519 verification, and optional local NPU/LLM AI omnibox. |
| **IRONPASS** | Hardware Identity & **IronPass Ledger** | Hybrid `#ip=` NFC (NXP NTAG 424 DNA) & QR tags: consumers get a zero-app public EU ESPR tap; authorized operators cross **BIFROST** to verify the classified BOM & hash-chained GS1 EPCIS 2.0 **IronPass Ledger** in ~30 ms. |

*Protocol Attribution:* Our Zero-IP networking builds on the **Public Domain Reticulum Wire Protocol** invented by Danish engineer **Mark Qvist** ([reticulum.network](https://reticulum.network)), implemented strictly in clean-room, commercial-safe **MIT Rust** (`citadel-rns-rs`) with zero restricted Python RNS dependencies.

---

### Three Ways We Offer Software for Free

| Tier | Where | What You Get |
| :--- | :--- | :--- |
| **Free Web App (Hosted)** | [whattio.app](https://whattio.app) | Instant browser access on our infrastructure—zero setup. |
| **Free Self-Hosted (Docker / Linux)** | `docker compose up` / `.deb` | Run locally, 0-port over Reticulum, or air-gapped on hardware you own. |
| **Open Source Code (GitHub)** | This organization (**AGPLv3** / **MIT** wire stack) | Audit, fork, modify, and extend via native `/api/mcp` tools & clean-room Rust. |

---

### Sovereign Zero-IP & Reticulum Stack

| Repository | License | Description |
| :--- | :--- | :--- |
| [`citadel-rns-rs`](https://github.com/whattio/citadel-rns-rs) | **MIT** | Clean-room MIT Rust Reticulum HTTP-over-Reticulum vault daemon, `FastTcp` (`TCP_NODELAY` + $O(1)$ HDLC), and in-process client library. |
| [`bifrost`](https://github.com/whattio/bifrost) | **AGPLv3 + Commercial** | **BIFROST — The Reticulum Ghost Browser** (`bifrost://` & `ironpass://`): 0-port Rust browser, local Ed25519 + GS1 EPCIS 2.0 IronPass Ledger verifier, built-in offline showcase & Ubuntu `.deb` installer. |

---

### Wave 1 Open-Source Apps

| Repository | Focus Area | Description |
| :--- | :--- | :--- |
| `soc-shield` | DPP / Compliance | Substances of Concern (REACH / SVHC / RoHS) BOM screening & MCP tool server. |
| `crm-database` | DPP / Compliance | EU Critical Raw Materials (CRMA) lookup & BOM dependency risk analyzer. |
| `dpp-playground` | DPP / Standards | Interactive CIRPASS-2 JSON-LD, GS1 Digital Link & ESPR validator sandbox. |
| `andvaris-forge` | PCM / Ingestion | Structured product content harvester for specs, datasheets, and BOMs. |
| `dpp-explorer` | DPP / PCM | Visual browser, graph inspector, and SHA-256 verifier for Digital Product Passports. |
| `asgaard-ai-vision` | PCM / Edge AI | Local GPU/NPU visual product inspection & media analysis over MCP. |

---

### Sovereign Enterprise & Commercial Licensing
Application repositories in this organization are dual-licensed under **GNU AGPLv3** + **Commercial License** (see [`COMMERCIAL-LICENSE.md`](../COMMERCIAL-LICENSE.md)) for proprietary embedding, OEM distribution, live EU regulatory feeds, 15-year ESPR passport hosting, turnkey **Citadel** Linux appliances, **IronPass NTAG 424 DNA** hardware provisioning, and full **Asgaard Agentic OS** orchestration.

- 🛡️ **Citadel, BIFROST & IronPass:** [citadel.ironpass.tech](https://citadel.ironpass.tech)
- 🌐 **Asgaard Agentic OS:** [asgaard.whattio.me](https://asgaard.whattio.me)
- 🚀 **Free Hosted Web Apps:** [whattio.app](https://whattio.app)
- 💼 **Commercial & Enterprise Inquiries:** [whatt.io](https://whatt.io) · `info@whatt.io`
