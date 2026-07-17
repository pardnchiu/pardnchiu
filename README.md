# 邱敬幃 Pardn Chiu

> My code is my pitch — if it resonates, you're my people.<br>
> Taiwan · AI Infrastructure · Platform Engineering

***

### [Agenvoy](https://github.com/pardnchiu/Agenvoy)
> Make AI actually work for you — a personal agent that writes its own tools and repairs itself.

***

### Backend

**Go/Service**
- **[KuraDB](https://github.com/pardnchiu/KuraDB)** — Multi-format document store on SQLite with hybrid keyword + vector search
- **[HakoRun (go-faas)](https://github.com/pardnchiu/HakoRun)** — Lightweight MCP-Server for agents to create APIs
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VM lifecycle REST API with SSE progress streaming
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Deploy CLI over rsync/SSH to Podman Compose or k3s, SQLite registry
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST client, VSCode `.http` compatible, with SSE streaming
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — TUI uptime + SSL-expiry monitor with concurrent checks and email alerts
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — TUI RSS aggregator with reader-mode extraction and offline SQLite store
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Four-layer cache (browser / Cloudflare / Nginx / local) with on-the-fly parameterized WebP/AVIF conversion

**Go/Module**
- **[go-llm-router](https://github.com/pardnchiu/go-llm-router)** — Unified routing across 12+ LLM providers (Claude, OpenAI, Gemini, Grok, DeepSeek...) with normalized token usage and OAuth support
- **[ToriiDB](https://github.com/pardnchiu/ToriiDB)** — Embedded DB unifying key-value, JSON query, and inline vector search
- **[go-pkg](https://github.com/pardnchiu/go-pkg)** — Personal Go toolkit: HTTP, sandbox isolation, multi-format document parsing
- **[go-browser](https://github.com/pardnchiu/go-browser)** — Chrome DevTools Protocol extractor reusing real logged-in sessions
- **[go-sqlkit](https://github.com/pardnchiu/go-sqlkit)** — Rewrite consolidating the three drivers below into one SQL toolkit with read-write separation
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with five-level priority heap and anti-starvation promotion
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Min-heap cron scheduler with dependency chains and panic recovery <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-bot](https://github.com/pardnchiu/go-bot)** — Rewritten as a drop-in importable library for interactive Telegram / Discord / LINE bots, with Gemini TTS voice
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — Redis-backed IP threat scoring with geo-anomaly progressive ban
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT auth with Redis lifecycle, ECDSA, and device-fingerprint binding <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis client with three-tier memory/Redis/file fallback and auto-resync

**Node.js**
- **[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** — Four-layer cache (browser / Cloudflare Worker / Nginx / local) with parameterized WebP conversion
- **[node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth)** — Dual-token JWT auth with device fingerprinting, ES256, and Redis revocation
- **[node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool)** — MySQL pool with read/write split and a fluent query builder

**PHP**
- **[php-async](https://github.com/pardnchiu/php-async)** — ReactPHP async task runner with topological dependency sorting
- **[php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli)** — Chainable MySQL client with read-write routing and retry resilience
- **[php-redis-cli](https://github.com/pardnchiu/php-redis-cli)** — Redis client over the native extension with persistent multi-DB connections
- **[php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback)** — Hybrid Redis + filesystem cache with automatic fallback
- **[php-session-fallback](https://github.com/pardnchiu/php-session-fallback)** — Redis session manager with filesystem fallback and hardening
- **[php-mailer](https://github.com/pardnchiu/php-mailer)** — PHPMailer SMTP wrapper with rate-limited bulk sending

***

### Frontend

**Framework**
- **[QuickUI](https://github.com/pardnio/QuickUI)** — Zero-dependency virtual-DOM framework with Proxy reactivity, i18n, lifecycle hooks <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/quickui" height="20">

**Library**
- **[NanoMD](https://github.com/pardnio/NanoMD)** — Dependency-free Markdown editor: split preview, vDOM diffing, Mermaid <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanomd" height="20">
- **[NanoJSON](https://github.com/pardnio/NanoJSON)** — Firebase-style visual JSON tree editor with live type switching, zero deps <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanojson" height="20">
- **[FlexPlyr](https://github.com/pardnio/FlexPlyr)** — Unified media player for HTML5 / YouTube / Vimeo, themeable, zero deps <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/flexplyr" height="20">
- **[RenderJS](https://github.com/pardnio/RenderJS)** — Prototype-extending DOM library with chainable syntax and reactive templates <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/renderjs" height="20">
- **[pdf2image](https://github.com/pardnio/pdf2image)** — Client-side PDF → JPG/PNG/WebP via pdf.js with ZIP batching <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/pdf2image" height="20">

**Demo/Web**
- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend website reproductions, several built on PDRenderKit
- **[WebUI](https://webui.pardn.io)** — Visual drag-and-drop website builder
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template

**Demo/iOS**
- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** — SwiftUI components recreating Pinterest-style animated UI
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** — Firebase chat app with QR friend-adding, code-only UIKit
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)** — UIKit finance tracker with monthly views and Font Awesome

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
