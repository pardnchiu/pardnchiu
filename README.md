> Started in iOS development, now focusing on AI Infrastructure · Platform Engineering.
>
> My code is my pitch — if it resonates, you're my people.

***

### [Agenvoy](https://github.com/pardnchiu/Agenvoy) — AI Agent Framework

> A Go agent runtime built from the standard library up, zero framework dependencies. Ships with intelligent multi-provider routing across 7 LLM backends, [OS-native sandbox](https://github.com/pardnchiu/go-faas), [built-in scheduler](https://github.com/pardnchiu/go-scheduler), a purpose-built [embedded database](https://github.com/pardnchiu/ToriiDB), and tool extensions in Python / JavaScript / REST API — drop a JSON spec and any HTTP endpoint becomes a callable tool.

### [ToriiDB](https://github.com/pardnchiu/ToriiDB) — Embedded JSON/Vector Database

> A four-in-one embedded database in pure Go — KV cache (Redis-style), document DB (MongoDB-style JSON queries), vector DB (OpenAI embeddings with cosine top-K), and local persistence (AOF + JSON snapshots with in-memory parsed cache) — packed into a single import. Embeddings live inline on each key and share the same AOF and compaction paths as KV values, no secondary index engine, no separate vector store. Aimed at Go projects that want to collapse a Redis + MongoDB + Pinecone stack into one binary instead of running three services behind the network.

***

<table><tr><td valign="top" width="33%">

### Recent
- **[Agenvoy (v0.19.5)](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.19.5)** — Extends `read_file` with CSV/TSV dispatch, disables its `alreadyCall` cache to stop stale post-edit reads, and splits the file / error-memory toolset into dedicated `fileReader` / `fileWriter` / `errorMemory` packages under `internal/filesystem/`.
- **[go-utils (v0.7.1)](https://github.com/pardnchiu/go-utils/releases/tag/v0.7.1)** — Reworks `sandbox.Wrap` into a context-aware, option-driven API returning `*exec.Cmd`, and adds first-class CPU, memory, network, capability, and filesystem-bind controls on both macOS (seatbelt) and Linux (bubblewrap + systemd-run).
- **[ToriiDB (v0.5.1)](https://github.com/pardnchiu/ToriiDB/releases/tag/v0.5.1)** — Add OS keychain as a secondary source for `OPENAI_API_KEY`. Lookup order is env (including `.env`) first, keychain fallback second — darwin uses `security`, linux uses `secret-tool`, other platforms read `$HOME/.secrets`.
- **[ThreadsMarketing (v0.1.0)](https://github.com/pardnchiu/ThreadsMarketing/releases/tag/v0.1.0)** — Initial release with TUI dashboard, Threads OAuth login flow, and startup token verification.

***

### Product

**Web**
- **[JOBALL](https://joball.tw)** — Freelance expert marketplace (Taiwan) · **peak 10K users / 340K monthly views**

**Chrome Extension**
- **[C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — E2EE Cross-origin real-time chat

**VS Code Extension**
- **[NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with live preview

**Discontinued**<br>
**[NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** · 
**[Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** · 
**[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)**

</td><td valign="top" width="33%">

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
- **[go-utils](https://github.com/pardnchiu/go-utils)** — Personal Go utility functions for rapid development
- **[go-sqlite](https://github.com/pardnchiu/go-sqlite)** · **[go-pg](https://github.com/pardnchiu/go-pg)** · **[go-mysql](https://github.com/pardnchiu/go-mysql)** — SQL clients with read-write separation
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with priority scheduling
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — GeoIP threat scoring + progressive ban
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis with auto local-storage failover

**Node.js**<br>
**[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** · 
**[node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth)** · 
**[node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool)**

**PHP**<br>
**[php-async](https://github.com/pardnchiu/php-async)** · 
**[php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli)** · 
**[php-redis-cli](https://github.com/pardnchiu/php-redis-cli)** · 
**[php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback)** · 
**[php-session-fallback](https://github.com/pardnchiu/php-session-fallback)** · 
**[php-mailer](https://github.com/pardnchiu/php-mailer)**

</td><td valign="top" width="33%">

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

**Demo/iOS**<br>
**[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** · 
**[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** · 
**[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)**

</td></tr></table>
