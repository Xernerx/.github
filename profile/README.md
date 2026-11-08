<!-- @format -->

<p align="center">
  <img src="https://www.xernerx.com/banner.png" alt="Xernerx Studios Banner" width="100%" />
</p>

<h1 align="center">Xernerx Studios</h1>

<p align="center">
  <b>Enterprise-grade infrastructure, modular Discord frameworks, and modern full-stack web &amp; desktop applications.</b>
</p>

<p align="center">
  <a href="https://xernerx.com"><img src="https://img.shields.io/badge/Website-xernerx.com-5865F2?style=for-the-badge" alt="Website" /></a>
  <a href="https://app.xernerx.com"><img src="https://img.shields.io/badge/App-app.xernerx.com-5865F2?style=for-the-badge" alt="App" /></a>
  <a href="https://docs.xernerx.com"><img src="https://img.shields.io/badge/Docs-docs.xernerx.com-informational?style=for-the-badge" alt="Documentation" /></a>
  <a href="https://portal.xernerx.com"><img src="https://img.shields.io/badge/Portal-portal.xernerx.com-success?style=for-the-badge" alt="Developer Portal" /></a>
  <a href="https://xernerx.com/discord"><img src="https://img.shields.io/badge/Discord-Join_Server-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
</p>

<p align="center">
  <img src="https://api.xernerx.com/v1/status/badge.svg" alt="Xernerx Platform Status" />
</p>

---

## 🌐 The Xernerx Suite Ecosystem

**Xernerx Studios** builds an interconnected ecosystem of web platforms, desktop clients, verified Discord applications, and open-source TypeScript developer toolkits:

| Platform | URL | Description |
| :--- | :--- | :--- |
| **Xernerx Home** | [`xernerx.com`](https://xernerx.com) | Official showcase, applications catalog, legal & security governance, and [Desktop Client download](https://xernerx.com/download). |
| **Xernerx App** | [`app.xernerx.com`](https://app.xernerx.com) | Unified dashboard, bot & server directory explorer, Virtue leveling studio, leaderboards, and live `/overlay`. |
| **Account Hub** | [`account.xernerx.com`](https://account.xernerx.com) | Identity & privacy settings (`public` / `limited` / `private`), OAuth connections, QR sign-in, and billing history. |
| **Developer Portal** | [`portal.xernerx.com`](https://portal.xernerx.com) | Team organizations, bot publishing, slash command synchronization, API tokens, and signed HMAC-SHA256 webhooks. |
| **Documentation** | [`docs.xernerx.com`](https://docs.xernerx.com) | Interactive REST API v1 playground, WebSocket RPC gateway specs, CDN streaming guides, and TypeDoc package references. |
| **Store** | [`store.xernerx.com`](https://store.xernerx.com) | Subscriptions, Virtue Server Boosts, Personal XP Boosts, cosmetic profile themes, and gifting. |
| **Info & Support Hub** | [`info.xernerx.com`](https://info.xernerx.com) | Public roadmap, feature suggestions, bug tracker, interactive FAQ, live status telemetry, and release changelogs. |
| **Xernerx Haste** | [`haste.xernerx.com`](https://haste.xernerx.com) | First-party Hastebin-compatible code pastebin with syntax highlighting, TTL expirations, and `/raw/[id]` streaming. |
| **Xernerx Blog** | [`blog.xernerx.com`](https://blog.xernerx.com) | Official engineering deep-dives, security advisories, product announcements, and `/rss.xml` feed. |

---

## 📦 Open-Source TypeScript SDKs & Bot Framework (`Apache-2.0`)

All public developer packages published by **Xernerx Studios** on npm are open-source under the **[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)**:

| Package | Repository | Documentation | Description |
| :--- | :--- | :--- | :--- |
| **[`xernerx`](https://www.npmjs.com/package/xernerx)** | [`Xernerx/xernerx`](https://github.com/Xernerx/xernerx) | [Docs](https://docs.xernerx.com/packages/xernerx) | All-in-one Xernerx Suite SDK, CLI (`xernerx` & `create-xernerx-app`), and Discord Bot Framework meta-package. |
| **[`@xernerx/framework`](https://www.npmjs.com/package/@xernerx/framework)** | [`Xernerx/xernerx-framework`](https://github.com/Xernerx/xernerx-framework) | [Docs](https://docs.xernerx.com/packages/@xernerx/framework) | Modular class-based Discord.js framework (`XernerxClient`, `XernerxShardClient`, builders, handlers, validators, `XernerxUser`). |
| **[`@xernerx/commands`](https://www.npmjs.com/package/@xernerx/commands)** | [`Xernerx/xernerx-commands`](https://github.com/Xernerx/xernerx-commands) | [Docs](https://docs.xernerx.com/packages/@xernerx/commands) | Developer diagnostic commands (`xc!`) & Slash/Context/Message Commands REST API synchronization SDK (`XernerxCommands`, `CommandsClient`). |
| **[`@xernerx/extension-builder`](https://www.npmjs.com/package/@xernerx/extension-builder)** | [`Xernerx/xernerx-extension-builder`](https://github.com/Xernerx/xernerx-extension-builder) | [Docs](https://docs.xernerx.com/packages/@xernerx/extension-builder) | Official base `ExtensionBuilder` class and lifecycle contract (`main`, `defer`) for `@xernerx/framework` extensions. |
| **[`@xernerx/hooks`](https://www.npmjs.com/package/@xernerx/hooks)** | [`Xernerx/xernerx-hooks`](https://github.com/Xernerx/xernerx-hooks) | [Docs](https://docs.xernerx.com/packages/@xernerx/hooks) | HMAC-SHA256 webhook receiver (`X-Xernerx-Signature`) & zero-database engagement cache (`voted`, `reviewed`, `tipped`) with REST fallback. |
| **[`@xernerx/stats`](https://www.npmjs.com/package/@xernerx/stats)** | [`Xernerx/xernerx-stats`](https://github.com/Xernerx/xernerx-stats) | [Docs](https://docs.xernerx.com/packages/@xernerx/stats) | Automated Discord bot telemetry extension, shard aggregator, and Stats REST API SDK (`XernerxStats`, `StatsClient`). |
| **[`@xernerx/terminal`](https://www.npmjs.com/package/@xernerx/terminal)** | [`Xernerx/xernerx-terminal`](https://github.com/Xernerx/xernerx-terminal) | [Docs](https://docs.xernerx.com/packages/@xernerx/terminal) | Scoped CLI logger, structured ANSI formatter, and interactive TTY spinner (`Terminal`, `terminal`, `Spinner`). |
| **[`@xernerx/websocket`](https://www.npmjs.com/package/@xernerx/websocket)** | [`Xernerx/xernerx-websocket`](https://github.com/Xernerx/xernerx-websocket) | [Docs](https://docs.xernerx.com/packages/@xernerx/websocket) | Promise-based real-time bidirectional JSON-RPC client for the Xernerx WebSocket Gateway (`XernerxWebsocket`). |
| **[`@xernerx/docs`](https://docs.xernerx.com/packages)** | [`Xernerx/docs`](https://github.com/Xernerx/docs) | [Docs](https://docs.xernerx.com) | Versioned TypeDoc AST (`docs.json`) and static HTML reference registry powering `docs.xernerx.com`. |

---

## 🤖 Official Discord Applications

- **[Virtue](https://xernerx.com/applications/virtue)** — Next-generation global & per-server Discord leveling bot featuring Text & Voice XP progression, Dynamic Hoist Roles, `/boost` multipliers, automated cycle resets (`daily`, `weekly`, `monthly`, `yearly`), and customizable `/level` rank cards.
- **[To-Do List Bot](https://xernerx.com/applications)** — Collaborative personal & server task boards directly inside Discord.
- **[Metamorphosis](https://xernerx.com/applications)** — Automated ephemeral "Join-to-Create" dynamic voice channels and room management.
- **[Zodiac](https://xernerx.com/applications)** — Daily horoscopes, astrological charts, and server compatibility insights.

---

## ⚖️ Licensing, Security & Governance

Xernerx Studios operates a transparent **two-tier licensing model**:

1. **Tier 1 — [Xernerx Studios Proprietary & SaaS License v1.0](https://xernerx.com/license):** Governs the Xernerx Suite web applications (`*.xernerx.com`), backend gateways, the Xernerx Desktop Client, and official hosted Discord bots (`Virtue`, `To-Do List Bot`, `Metamorphosis`, `Zodiac`).
2. **Tier 2 — [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0):** Governs all public open-source SDKs (`xernerx` & `@xernerx/*`) and developer documentation (`Xernerx/docs`).

- 🔒 **Security Policy & Responsible Disclosure:** [xernerx.com/security](https://xernerx.com/security) (`security@xernerx.com`)
- 📜 **Legal Policies:** [License Overview](https://xernerx.com/license) • [Terms of Service](https://xernerx.com/terms) • [Privacy Policy](https://xernerx.com/privacy) • [Cookie Policy](https://xernerx.com/cookies)
