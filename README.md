# 邱敬幃 Pardn Chiu

> My code is my pitch — if it resonates, you're my people.<br>
> Taiwan · AI Infrastructure · Platform Engineering

***

### [Agenvoy](https://github.com/pardnchiu/Agenvoy)
> Make AI actually work for you - A personal agent that writes its own tools and repairs itself.

| Category | Package | Description |
| :- | :- | :- |
| Memory Design | **[cim-prototype](https://github.com/pardnio/cim-prototype)** | LLM with Cognitive Imperfect Memory |
| Memory Store | **[ToriiDB](https://github.com/pardnchiu/ToriiDB)** | Embedded KV with JSON query and semantic vector search |
| RAG | **[KuraDB](https://github.com/pardnchiu/KuraDB)** | Multi-format ingestion, SQLite-backed, keyword & vector search |
| Cron / Task | **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** | Scheduler with standard cron and task dependencies |
| Browser Control | **[go-browser](https://github.com/pardnchiu/go-browser)** | Chrome extractor with one-shot fetch and interactive tabs |
| Sandbox / Plug Tool | **[go-faas](https://github.com/pardnchiu/go-faas)** | Function-as-a-Service runtime for Python / JS / TS |
| Messenger | **[go-bot](https://github.com/pardnchiu/go-bot)** | Telegram long polling + Discord WebSocket |

***

### Backend

**Go/Infrastructure**
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VM lifecycle API with SSE streaming
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Container deployment CLI via rsync/SSH

**Go/Service**
- **[go-notify-hub](https://github.com/pardnchiu/go-notify-hub)** — Unified API for Discord / Slack / LINE / Email
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST client, `.http` file compatible
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — Uptime + SSL expiry monitor
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — TUI RSS reader with full-text extraction
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Four-layer cache, on-the-fly WebP conversion

**Go/Package**
- **[go-pkg](https://github.com/pardnchiu/go-pkg)** — Personal Go utility functions for rapid development
- **[go-sqlite](https://github.com/pardnchiu/go-sqlite)** · **[go-pg](https://github.com/pardnchiu/go-pg)** · **[go-mysql](https://github.com/pardnchiu/go-mysql)** — SQL clients with read-write separation
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with priority scheduling
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Cron scheduler with dependency chains <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — GeoIP threat scoring + progressive ban
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT middleware with Redis session + auto-renewal <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
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

***

### Frontend

**Framework**
- **[QuickUI](https://github.com/pardnio/QuickUI)** — Virtual DOM framework on pure JS with reactive binding <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/quickui" height="20">

**Library**
- **[NanoMD](https://github.com/pardnio/NanoMD)** — Split-pane Markdown editor with Mermaid <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanomd" height="20">
- **[NanoJSON](https://github.com/pardnio/NanoJSON)** — Interactive JSON tree editor, zero dependencies <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanojson" height="20">
- **[FlexPlyr](https://github.com/pardnio/FlexPlyr)** — HTML5 / YouTube / Vimeo unified player <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/flexplyr" height="20">
- **[RenderJS](https://github.com/pardnio/RendeJS)** — Chainable DOM manipulation via prototype extension <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/renderjs" height="20">
- **[pdf2image](https://github.com/pardnio/pdf2image)** — Client-side PDF to JPG/PNG/WebP <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/pdf2image" height="20">

**Demo/Web**
- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend reproductions
- **[WebUI](https://webui.pardn.io)** — Visual drag-and-drop website builder
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template

**Demo/iOS**
- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** 
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)**
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)**

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
