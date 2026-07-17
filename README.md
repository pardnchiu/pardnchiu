# 邱敬幃 Pardn Chiu

> My code is my pitch — if it resonates, you're my people.<br>
> Taiwan · AI Infrastructure · Platform Engineering

***

### [Agenvoy](https://github.com/pardnchiu/Agenvoy)
> A personal AI agent that writes its own tools and self-schedules tasks via MCP.

***

### Backend

**Go/Service**
- **[KuraDB](https://github.com/pardnchiu/KuraDB)** — RAG database on SQLite with hybrid keyword + vector search
- **[HakoRun (go-faas)](https://github.com/pardnchiu/HakoRun)** — Sandboxed FaaS platform running Python/JS/TS via Bubblewrap (WIP)
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VM lifecycle REST API with SSE progress streaming
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Deploy CLI over rsync/SSH to Podman Compose or k3s
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST client, VSCode `.http` compatible, with SSE streaming
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — TUI uptime + SSL-expiry monitor with email alerts
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — TUI RSS aggregator with reader-mode extraction and offline store
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Four-layer cache (browser / Cloudflare / Nginx / local) with WebP/AVIF conversion (archived)

**Go/Module**
- **[go-llm-router](https://github.com/pardnchiu/go-llm-router)** — Unified routing across 12+ LLM providers with normalized token usage
- **[ToriiDB](https://github.com/pardnchiu/ToriiDB)** — Embedded DB unifying key-value, JSON query, and vector search
- **[go-pkg](https://github.com/pardnchiu/go-pkg)** — Personal Go toolkit: HTTP, sandbox isolation, document parsing
- **[go-browser](https://github.com/pardnchiu/go-browser)** — CDP browser automation reusing real sessions with stealth anti-detection
- **[go-sqlkit](https://github.com/pardnchiu/go-sqlkit)** — Unified SQL toolkit for MySQL/MariaDB/SQLite with read-write splitting
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with five-level priority heap and anti-starvation promotion
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Min-heap cron scheduler with dependency chains and panic recovery <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-bot](https://github.com/pardnchiu/go-bot)** — Library for Telegram/Discord/LINE bots with native UI and Gemini TTS
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — Redis-backed IP risk scoring with progressive escalating bans
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT auth with Redis lifecycle, ECDSA, and device-fingerprint binding <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis client with three-tier memory/Redis/file fallback and auto-resync

**Node.js**
- **[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** — Multi-tier image cache (browser / Cloudflare Worker / Nginx / local) with WebP/AVIF conversion
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
- **[QuickUI](https://github.com/pardnio/QuickUI)** — Zero-dependency vDOM framework with Proxy reactivity, i18n, lifecycle hooks <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/quickui" height="20">

**Library**
- **[NanoMD](https://github.com/pardnio/NanoMD)** — Dependency-free Markdown editor: split preview, vDOM diffing, Mermaid <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanomd" height="20">
- **[NanoJSON](https://github.com/pardnio/NanoJSON)** — Firebase-style visual JSON tree editor with type switching, zero deps <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanojson" height="20">
- **[FlexPlyr](https://github.com/pardnio/FlexPlyr)** — Unified media player for HTML5 / YouTube / Vimeo, themeable, zero deps <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/flexplyr" height="20">
- **[RenderJS](https://github.com/pardnio/RenderJS)** — Prototype-extending DOM library with chainable syntax and manual `renew()` updates <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/renderjs" height="20">
- **[pdf2image](https://github.com/pardnio/pdf2image)** — Client-side PDF → JPG/PNG/WebP via pdf.js with ZIP batching <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/pdf2image" height="20">

**Demo/Web**
- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend website reproductions, several built on PDRenderKit
- **[WebUI](https://webui.pardn.io)** — Visual website builder with modular prebuilt templates (WIP)
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template built on QuickUI, NanoMD, NanoJSON, FlexPlyr

**Demo/iOS**
- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** — SwiftUI components recreating Pinterest-style animated UI
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** — Firebase chat app with QR friend-adding, code-only UIKit
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)** — UIKit finance tracker with monthly views and Font Awesome

***

### Product

**Web**
- **[JOBALL](https://joball.tw)** — Freelance expert marketplace (Taiwan) · **peak 10K users / 340K monthly views**

**Chrome Extension**
- **[C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — E2EE cross-domain chat extension with no server-side message storage

**VS Code Extension**
- **[NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with split-screen preview and Mermaid support

**Discontinued**
- **[NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** · 
**[Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** · 
**[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)**
