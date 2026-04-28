---
aliases: wyre-msp-mcp
display_name: MSP MCP
logo: msp-mcp.png
short_description: Model Context Protocol servers wrapping MSP tools (PSAs, RMMs, security, documentation) for AI assistants like Claude.
topic: msp-mcp
url: https://mcp.wyre.ai
related: mcp, model-context-protocol, msp
---

MSP MCP is a family of [Model Context Protocol](https://modelcontextprotocol.io) servers that expose Managed Service Provider (MSP) tooling to AI assistants. Each server wraps a vendor's API — PSAs (Autotask, ConnectWise, HaloPSA), RMMs (Datto, NinjaOne, Atera, Syncro), documentation platforms (IT Glue, Hudu, Liongard), security tools (SentinelOne, Huntress, Blumira, RocketCyber), email security (Proofpoint, Avanan, Abnormal, Mimecast, IRONSCALES, KnowBe4, SpamTitan), incident management (Rootly, PagerDuty), and more — as MCP-compliant tools so an MSP technician can ask Claude to triage a ticket, check device health, or pull documentation in plain English.

Repositories tagged with `msp-mcp` typically follow a common pattern: TypeScript or Python implementation, Streamable HTTP or stdio transport, structured tool schemas, and per-vendor authentication (API keys, OAuth, or session tokens). Many of them are also exposed centrally through the [WYRE MCP Gateway](https://mcp.wyre.ai), which provides OAuth 2.1 + PKCE auth, encrypted credential storage, and a single endpoint that fans out to whichever vendors an MSP has connected.
