# Zero Heat Super Compute — MCP Gateway

[![smithery badge](https://smithery.ai/badge/aruuhii2yo/maxion-mcp-gateway)](https://smithery.ai/servers/aruuhii2yo/maxion-mcp-gateway)

**J&K Advanced Technologies — AWS Certified Partner.**

Enterprise MCP (Model Context Protocol) server suite with **19 tools** across four product namespaces: thermal performance management, zero-trust security, AES-256-GCM encrypted storage, and AI video/image generation.

Hosted on AWS Lambda. **Free 30-minute trial auto-activates on your first tool call** — no signup, no config, no credit card.

---

## Quickstart (30 seconds)

Connect via [Smithery](https://smithery.ai/servers/aruuhii2yo/maxion-mcp-gateway) and your AI client can call all 19 tools immediately.

Or add the endpoint directly to any MCP client:

```
https://5pu357jdkqc3qynzkjvu3okgqy0ncsiy.lambda-url.us-east-1.on.aws/mcp
```

Already purchased? Enter your Gumroad license key when connecting (Smithery prompts for it), or pass it via the `x-fleet-key` header.

---

## Products

### 🌡️ Maxion V16 — Thermal Performance Management

Eliminates heat accumulation in server racks and HPC nodes. Reduces power draw by up to 36%, prevents thermal throttling, and extends hardware lifespan — no infrastructure changes required.

**Verified bare-metal test results** (production 2U rack node, continuous stress sequence):

| Metric | Before | After |
|---|---|---|
| CPU package temperature | 95°C | 38°C (−57°C) |
| Relative power draw | 100% | 64% (−36%) |
| Thermal throttle | ACTIVE | ELIMINATED |
| Stability index | 61% | 100% |

Tools: `engine.maxion.activate` · `engine.maxion.deactivate` · `engine.maxion.status` · `engine.maxion.diagnostics`

### 🛡️ Diamonize LSA — Zero-Trust Security

Military-grade security scanning for data centers, HPC clusters, and campus networks. SHA-256 hashing, threat analysis, and real-time memory scan results.

Tools: `security.diamonize.scan` · `security.diamonize.quarantine` · `security.diamonize.logs` · `security.diamonize.status`

### 🔐 Quezar — AES-256-GCM Encrypted Storage

Sub-millisecond encrypted storage with 92x compression. AES-256-GCM authenticated encryption (NIST SP 800-38D).

Tools: `storage.quezar.store` · `storage.quezar.retrieve` · `storage.quezar.delete` · `storage.quezar.list` · `storage.quezar.status`

### 🎬 Lineage.0 VC — AI Video & Image Generation

Watermark-free 4K AI video via Amazon Nova Reel 1.1 and commercial-use image generation via Amazon Nova Canvas. Pay-per-video — no subscription.

Tools: `media.lineage0.generate` · `media.lineage0.status` · `media.lineage0.archive`

---

## Pricing

| Product | Tier | Price |
|---|---|---|
| Maxion V16 | Free trial | 30 minutes, auto-granted on first call |
| Maxion V16 | Hourly | $2.50/hr |
| Maxion V16 | Monthly | $20/mo |
| Diamonize LSA | Free trial | 30 minutes, auto-granted on first call |
| Diamonize LSA | Monthly | $20/mo |
| Quezar | Free trial | 30 minutes, auto-granted on first call |
| Quezar | Monthly | $9.99/mo (includes 25GB pre-compressed storage) |
| Lineage.0 VC | Pay-per-video | $0.14/sec — from $0.99 (6s) to $11.76 (84s) |
| Fleet / Enterprise | Custom | aruuh@advancedapparchitect.com |

All purchases are processed by [Gumroad](https://gumroad.com). Call the `billing.purchase` tool from your AI client for a direct checkout link, or visit [advancedapparchitect.com](https://advancedapparchitect.com).

---

## Local Engines (Windows)

Maxion, Diamonize, and Quezar can also run **natively on your own machine** as compiled engine binaries — your data never leaves your hardware. A valid license is required; your download contains only the engine(s) your license covers.

See [INSTALL.md](INSTALL.md) for the full local setup guide.

---

## Tool Catalog

The complete machine-readable tool catalog (names, descriptions, input/output schemas, safety annotations) is in [`server-card.json`](server-card.json) — the same document served live at:

```
https://5pu357jdkqc3qynzkjvu3okgqy0ncsiy.lambda-url.us-east-1.on.aws/.well-known/mcp/server-card.json
```

---

## Links

- 🌐 **Website:** https://advancedapparchitect.com
- ⚡ **Smithery:** https://smithery.ai/servers/aruuhii2yo/maxion-mcp-gateway
- 🏢 **Enterprise:** aruuh@advancedapparchitect.com

## License

The gateway service, engine binaries, and all product software are proprietary — see [LICENSE.md](LICENSE.md). This repository contains documentation and public metadata only.
