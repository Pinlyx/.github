<div align="center">

# Pinlyx

**AI-powered omnichannel CRM for Telegram, WhatsApp, Instagram, Messenger, X, email and live chat.**

One inbox, one pipeline and an AI agent that answers customer messages on every channel.

[Website](https://pinlyx.com) · [App](https://app.pinlyx.com) · [Docs](https://docs.pinlyx.com) · [Chrome Extension](https://chromewebstore.google.com/detail/crm-solid-clipper-save-le/mbdeafjdkhilgbdaoenggfamombmgpfm) · [X](https://x.com/pinlyx)

</div>

---

## Start here

Three tools anyone can use today. None of them needs a Pinlyx account.

| Repo | What it does | Try it |
|---|---|---|
| [messaging-mcp](https://github.com/Pinlyx/messaging-mcp) | WhatsApp, Instagram, Messenger and Telegram for your AI assistant, on the official APIs. Self-hosted MCP server that stops a reply the platform would reject before it is sent. | `npx -y messaging-mcp --demo` |
| [messaging-skills](https://github.com/Pinlyx/messaging-skills) | Fifteen agent skills for customer messaging: WhatsApp templates that pass review, reply windows, Instagram DM automation, comment to DM funnels, AI DM agents, webhooks, Telegram bots. | `npx skills add Pinlyx/messaging-skills` |
| [open-business-finder](https://github.com/Pinlyx/open-business-finder) | Local businesses by country, district and category from open map data. A Google Maps scraper alternative with no API key, no browser and no scraping. | `uvx --from git+https://github.com/Pinlyx/open-business-finder obf --help` |

## Libraries and tools

| Repo | What it does |
|---|---|
| [messaging-rules](https://github.com/Pinlyx/messaging-rules) | (npm `messaging-rules`) Can I message this person right now? Source-cited rules for WhatsApp, Instagram, Messenger, Telegram and X (reply windows, message tags, templates, length, media and rate limits) as data, a TypeScript and Python library and an MCP server. |
| [dm-bench](https://github.com/Pinlyx/dm-bench) | Open benchmark for AI agents that answer customer DMs: 70 scenarios in 7 languages covering made-up facts, handoff, platform rules, prompt injection and privacy. |
| [unified-message](https://github.com/Pinlyx/unified-message) | (npm `unified-message`) One normalized message object for Telegram, WhatsApp, Instagram, Messenger and X webhooks, with signature verification for each. Zero dependencies. |
| [telegram-channel-stats](https://github.com/Pinlyx/telegram-channel-stats) | Subscribers, views, reach and posting frequency for any public Telegram channel, benchmarked against its size class. No API key. |
| [contact-channel-detector](https://github.com/Pinlyx/contact-channel-detector) | Which ways does a website give customers to reach it? WhatsApp, live chat widgets, social profiles, e-mail and phone, with evidence. |
| [turkiye-il-ilce](https://github.com/Pinlyx/turkiye-il-ilce) | Offline reverse geocoding for Turkey: coordinates to province and district, with 2026 boundaries as GeoJSON. |

## Integrations and SDKs

| Repo | What it is |
|---|---|
| [pinlyx-mcp](https://github.com/Pinlyx/pinlyx-mcp) | MCP server: read and answer conversations, manage contacts and deals, schedule posts from any MCP client |
| [n8n-nodes-pinlyx](https://github.com/Pinlyx/n8n-nodes-pinlyx) | n8n community node |
| [pinlyx-zapier](https://github.com/Pinlyx/pinlyx-zapier) | Zapier integration: triggers, actions and searches over the public API |
| [pinlyx-dotnet](https://github.com/Pinlyx/pinlyx-dotnet) | .NET SDK (`dotnet add package Pinlyx`) |
| [pinlyx-clipper](https://github.com/Pinlyx/pinlyx-clipper) | Browser extension that saves a LinkedIn, X, Instagram or GitHub profile into the CRM |
| [pinlyx-agent-kit](https://github.com/Pinlyx/pinlyx-agent-kit) | Plugin and skills for AI coding agents (Claude Code, Gemini CLI, Kiro) on the Pinlyx MCP server |
| [vscode-pinlyx](https://github.com/Pinlyx/vscode-pinlyx) | Adds the Pinlyx MCP server to VS Code, Cursor and other Open VSX editors |
| [dify-plugin-pinlyx](https://github.com/Pinlyx/dify-plugin-pinlyx) | Dify tool plugin: contacts, deals and tasks |
| [activepieces-piece-pinlyx](https://github.com/Pinlyx/activepieces-piece-pinlyx) | Activepieces piece: contacts, deals, tasks and webhook triggers |
| [gtm-pinlyx-live-chat](https://github.com/Pinlyx/gtm-pinlyx-live-chat) | Google Tag Manager template for the Pinlyx live chat widget |

## Guides

| Repo | What it is |
|---|---|
| [mcp-social-media-guide](https://github.com/Pinlyx/mcp-social-media-guide) | Vendor-neutral tutorials for running social media DMs and scheduled posts through MCP |
| [google-ads-mcp](https://github.com/Pinlyx/google-ads-mcp) | Run a Google Ads account from an MCP client: tutorials and tool reference |

## Open data

| Repo | What it is |
|---|---|
| [turkey-business-digital-data](https://github.com/Pinlyx/turkey-business-digital-data) | Website, phone and social media presence for 1,786,700 businesses in Turkey, by province and sector. CC BY 4.0 |
| [turkey-website-contact-channels](https://github.com/Pinlyx/turkey-website-contact-channels) | WhatsApp vs live chat on 5,014 Turkish business websites. CC BY 4.0 |
| [business-online-presence-by-region](https://github.com/Pinlyx/business-online-presence-by-region) | How many local businesses list a website, region by region: 50.9M places in 15 countries, normalised with official population data. CC BY 4.0 |

More research: [Telegram channel reach 2026](https://pinlyx.com/research/telegram-channel-reach-2026), [Turkey business digital report](https://pinlyx.com/research/turkey-business-digital-report), [WhatsApp vs live chat on Turkish websites](https://pinlyx.com/research/turkey-website-whatsapp-live-chat-2026)

## Contact

- Support: support@pinlyx.com
- Docs and API reference: https://docs.pinlyx.com
- Issues and pull requests are welcome on every repo above.
