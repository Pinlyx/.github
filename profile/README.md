<div align="center">

# Pinlyx

**Omnichannel AI CRM for modern customer-facing teams.**

Talk to customers on Telegram, X, Email, Live Chat and via Bot, from one inbox, one pipeline, one API.

[Website](https://pinlyx.com) · [App](https://app.pinlyx.com) · [Chrome Extension](https://chromewebstore.google.com/detail/crm-solid-clipper-save-le/mbdeafjdkhilgbdaoenggfamombmgpfm) · [API Docs](https://docs.pinlyx.com) · [Status](https://health.crmsolid.com)

</div>

---

## What Pinlyx is

Pinlyx is an omnichannel customer relationship platform that unifies five conversation channels behind one CRM:

- **Telegram**: multi-account, scraping, sequences, broadcasting
- **X / Twitter**: DMs and account management
- **Email**: per-user inbox, threading, templates
- **Live Chat**: embeddable web widget for your site
- **Bot**: programmable conversational workflows

On top of the inbox sit AI-powered lead scoring, automated outreach sequences, a public REST API, and an MCP server so AI agents can drive the CRM directly.

## Channels & capabilities

| Area | What ships today |
|---|---|
| Inbox | Telegram, X/Twitter, Email, Live Chat, Bot, all in one pane |
| Pipeline | Drag-and-drop stages, archive/restore, notes |
| Outreach | Sequences, broadcasting, spintax, scheduling |
| AI | Lead scoring, message analysis, reply suggestions |
| Billing | LemonSqueezy + WeePay, per-plan limits |
| Real-time | SignalR streams for inbox + job status |
| Reliability | Rate limiting with flood-wait backoff, proxy support |
| Browser extension | One-click capture from LinkedIn, X, Instagram, GitHub or any page, straight into the CRM |

## Developer surface

| Product | What it is | Status |
|---|---|---|
| Public REST API v1 | Bearer-key + scoped endpoints for contacts, messages, sequences, accounts | Stable |
| Webhooks | Outbound events for inbound messages, job status, billing | Stable |
| MCP server | Lets Claude, Cursor, ChatGPT and other AI clients drive the CRM over the Model Context Protocol | Stable |
| OpenAPI spec | Machine-readable definition of the public API | Published in-product |

## SDKs

| SDK | Language | Status | Repo |
|---|---|---|---|
| `pinlyx-dotnet` | C# / .NET 8+ | Alpha | [Pinlyx/pinlyx-dotnet](https://github.com/Pinlyx/pinlyx-dotnet) |
| `pinlyx-python` | Python 3.10+ | Planned | _coming soon_ |
| `pinlyx-node` | TypeScript / Node 20+ | Planned | _coming soon_ |
| `pinlyx-mcp` | TypeScript (MCP server) | Alpha | [Pinlyx/pinlyx-mcp](https://github.com/Pinlyx/pinlyx-mcp) |

## Guides

| Repo | What it is |
|---|---|
| [Pinlyx/mcp-social-media-guide](https://github.com/Pinlyx/mcp-social-media-guide) | Vendor-neutral tutorials for running social media DMs and scheduled posts through MCP |

## Get started

### 1. Create an API key

Sign in to https://app.crmsolid.com, open **Settings → Developers**, and generate a key. Each key is scoped: pick the smallest scope that matches your use case.

### 2. Install a SDK (example: .NET)

```bash
dotnet add package CrmSolid
```

```csharp
using CrmSolid;

var client = new CrmSolidClient("csk_live_...");

var page = await client.Contacts.ListAsync(limit: 50);

foreach (var c in page.Items)
{
    Console.WriteLine($"{c.Id}\t{c.Name}\t@{c.Username}");
}
```

> The .NET SDK is in alpha. The package name and exact API may change before v1.0.

### 3. Read the docs

Full REST reference, webhooks, and authentication: https://docs.pinlyx.com

## Open-source repositories

| Repo | Purpose | Status |
|---|---|---|
| [`.github`](https://github.com/Pinlyx/.github) | Org profile, community health files | Live |
| [`pinlyx-clipper`](https://github.com/Pinlyx/pinlyx-clipper) | Browser extension, full source of the published build | [Live on the Chrome Web Store](https://chromewebstore.google.com/detail/crm-solid-clipper-save-le/mbdeafjdkhilgbdaoenggfamombmgpfm) |
| [`pinlyx-dotnet`](https://github.com/Pinlyx/pinlyx-dotnet) | Official .NET SDK | Alpha |
| `pinlyx-python` | Official Python SDK | Planned |
| `pinlyx-node` | Official Node.js / TypeScript SDK | Planned |
| [`pinlyx-mcp`](https://github.com/Pinlyx/pinlyx-mcp) | MCP server reference implementation | Alpha |
| `pinlyx-docs` | Public docs site source | Planned |
| `pinlyx-openapi` | OpenAPI spec mirror + generator | Planned |
| `pinlyx-examples` | End-to-end examples across SDKs | Planned |

Stars and issues on these repos are welcome once they ship.

## Stay in touch

- Website: https://pinlyx.com
- App: https://app.crmsolid.com
- Docs: https://docs.pinlyx.com
- Support: info@pinlyx.com
- Security: info@pinlyx.com _(dedicated security@ inbox coming soon)_
- X / Twitter: [@pinlyx](https://x.com/pinlyx)
