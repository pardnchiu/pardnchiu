# 邱敬幃 Pardn Chiu

> Started in iOS development, now focusing on AI Infrastructure · Platform Engineering.<br>
> My code is my pitch — if it resonates, you're my people.

Taiwan · AI Infrastructure · Platform Engineering

***

### [Agenvoy](https://github.com/pardnchiu/Agenvoy)

> Agentic runtime | Multi-provider concurrent dispatch | Self-improving error memory | Pluggable tool extensions | Sandbox execution 

### [ToriiDB](https://github.com/pardnchiu/ToriiDB)

> Embedded JSON database | Redis-style KV | MongoDB-like JSON queries | Inline vector embeddings | AOF persistence 


### [KuraDB](https://github.com/pardnchiu/KuraDB) — (WIP)
> Multi-format ingestion (PDF/Word/PPT/Excel/CSV/Image/Audio-Video/Text) | SQLite-backed | Keyword & vector search 

***

### Recent
- **[go-bot (v0.3.3)](https://github.com/pardnchiu/go-bot/releases/tag/v0.3.3)** — Fixes `Input.ChannelName` always being `""` on Discord. The intent bitmask was missing `IntentGuilds`, so the gateway never delivered `GUILD_CREATE` / `CHANNEL_*` events—`Session.State` had no channel data and `State.Channel(channelID)` always returned not-found, making the v0.3.2 `ChannelName` accessor silently useless. Adding `IntentGuilds` to `Identify.Intents` restores state cache population; `ChannelName` now resolves zero-round-trip as designed.
- **[Agenvoy (v0.23.4)](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.23.4)** — Scheduled-state introspection becomes a first-class tool surface. The runtime now exposes read-only listers for one-shot tasks and recurring crons, closing a discovery gap that previously forced the agent to fall back on filesystem traversal.
- **[go-pkg (v0.12.3)](https://github.com/pardnchiu/go-pkg/releases/tag/v0.12.3)** — Extends `filesystem/parser` with three tabular / binary input handlers: `Image` re-encodes JPEG / PNG / GIF to JPEG base64 data URLs, `CSV` reads CSV / TSV with BOM-aware decoding and 1MB guard, and `XLSX` parses OOXML first sheet via stdlib `archive/zip` + `encoding/xml`. The new APIs all return `(string, error)` — diverging from the existing `(string, []Chunk, error)` shape — because chunking has no meaning for images or rows.
***

<table><tr><td valign="top" width="50%">

### Backend

[![Mentioned in Awesome Go](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go) 
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Cron scheduler with dependency chains
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT middleware with Redis session + auto-renewal

**Go/Infrastructure**
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VM lifecycle API with SSE streaming
- **[go-faas](https://github.com/pardnchiu/go-faas)** — FaaS runtime with Bubblewrap sandbox
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Container deployment CLI via rsync/SSH

**Go/Service**
- **[ThreadsMarketing](https://github.com/pardnchiu/ThreadsMarketing)** — AI marketing agent for Threads, built on Agenvoy with DNA-driven content loop `WIP`
- **[go-notify-hub](https://github.com/pardnchiu/go-notify-hub)** — Unified API for Discord / Slack / LINE / Email
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST client, `.http` file compatible
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — Uptime + SSL expiry monitor
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — TUI RSS reader with full-text extraction
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Four-layer cache, on-the-fly WebP conversion

**Go/Package**
- **[go-bot](https://github.com/pardnchiu/go-bot)** 
- **[go-pkg](https://github.com/pardnchiu/go-pkg)** — Personal Go utility functions for rapid development
- **[go-sqlite](https://github.com/pardnchiu/go-sqlite)** · **[go-pg](https://github.com/pardnchiu/go-pg)** · **[go-mysql](https://github.com/pardnchiu/go-mysql)** — SQL clients with read-write separation
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with priority scheduling
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — GeoIP threat scoring + progressive ban
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis with auto local-storage failover

**Node.js**
- **[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** · 
**[node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth)** · 
**[node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool)**

**PHP**
- **[php-async](https://github.com/pardnchiu/php-async)** · 
**[php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli)** · 
**[php-redis-cli](https://github.com/pardnchiu/php-redis-cli)** · 
**[php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback)** · 
**[php-session-fallback](https://github.com/pardnchiu/php-session-fallback)** · 
**[php-mailer](https://github.com/pardnchiu/php-mailer)**

</td><td valign="top" width="50%">

### Frontend

**Framework**
- **[QuickUI](https://quickui.pardn.io)** — Virtual DOM framework on pure JS with reactive binding · **20K+/mo**

**Library**
- **[NanoMD](https://nanomd.pardn.io)** — Split-pane Markdown editor with Mermaid · **20K+/mo**
- **[NanoJSON](https://nanojson.pardn.io)** — Interactive JSON tree editor, zero dependencies · **20K+/mo**
- **[FlexPlyr](https://flexplyr.pardn.io)** — HTML5 / YouTube / Vimeo unified player · **20K+/mo**
- **[RenderJS](https://renderjs.pardn.io)** — Chainable DOM manipulation via prototype extension · **20K+/mo**
- **[pdf2image](https://pdf2image.pardn.io/)** — Client-side PDF to JPG/PNG/WebP · **1K+/mo**

**Demo/Web**
- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend reproductions
- **[WebUI](https://webui.pardn.io)** — Visual drag-and-drop website builder
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template

**Demo/iOS**
- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** 
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)**
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)**

</td></tr></table>

***

### Product

**Web**
- **[JOBALL](https://joball.tw)** — Freelance expert marketplace (Taiwan) · **peak 10K users / 340K monthly views**

**Chrome Extension**
- **[C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — E2EE Cross-origin real-time chat

**VS Code Extension**
- **[NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with live preview

**Discontinued**
- **[NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** · 
**[Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** · 
**[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)**
