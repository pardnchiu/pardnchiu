> My code is my pitch — if it doesn't resonate, no worries.

## Backend

### Go

#### Framework

- **[Agenvoy](https://github.com/pardnchiu/Agenvoy)** — AI agent framework with cross-session error memory, multi-provider LLM routing (Copilot / OpenAI / Codex / Claude / Gemini / Nvidia), drop-in script/API tool extensions, and OS-native sandbox. TUI dashboard unifies CLI, Discord bot, and REST API.

#### Infrastructure

- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VE VM automation REST API. SSE-streamed full lifecycle provisioning, concurrent IP/VMID allocation, CPU architecture auto-detection, and transparent multi-node cluster routing with live migration.
  Successor: [go-kvmesh](https://github.com/pardnchiu/go-kvmesh) `WIP` / [go-qemu](https://github.com/pardnchiu/go-qemu) `WIP`
- **[go-faas](https://github.com/pardnchiu/go-faas)** — FaaS runtime for Python/JS/TS. Bubblewrap namespace sandbox, Redis-backed script versioning, and systemd slice resource control per execution.
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Remote container deployment CLI via rsync/SSH. Dual runtime targeting (Podman Compose / k3s), SQLite deployment registry with UID tracking.

#### Service

- **[go-notify-hub](https://github.com/pardnchiu/go-notify-hub)** — Multi-channel notification hub (Discord / Slack / LINE / Email) with unified REST API, built-in Discord/LINE bot engine, and runtime channel management.
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST API tester, compatible with VSCode `.http` file format. SSE streaming, file auto-reload, JSON formatting.
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — Website uptime monitor with SSL tracking, response time measurement, auto-retry, and email alerts. TUI interface.
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — Terminal RSS aggregator with goquery full-article extraction, SQLite offline storage, and TUI interface. LLM summarization `Planned`.
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Image caching server with four-layer cache (browser → CDN → Nginx → backend), default WebP output, on-the-fly format conversion, and parameterized resize.

#### Package

- **[ToriiDB](https://github.com/pardnchiu/ToriiDB)** — Embedded JSON document database in pure Go, zero dependencies. Redis-like KV with TTL + MongoDB-like conditional queries (FIND/QUERY with logical operators and dot-notation). AOF persistence, auto-chunked concurrent scan above 1024 entries.
- **SQL Clients** — Chainable query builders with read-write separation and struct auto-binding:
  [go-sqlite](https://github.com/pardnchiu/go-sqlite) (WAL, single-writer + read pool) · [go-pg](https://github.com/pardnchiu/go-pg) (ILIKE, ON CONFLICT, RETURNING) · [go-mysql](https://github.com/pardnchiu/go-mysql)
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Priority-based task queue with configurable workers, preset task profiles, and graceful shutdown.
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Cron scheduler with min-heap ordering, task dependency chains, per-dependency timeout, and panic recovery. [![Mentioned in Awesome Go](https://awesome.re/mentioned-badge.svg)](https://awesome.re)
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — IP threat detection middleware with GeoIP lookup, three-tier scoring, per-tier rate limiting, and progressive ban escalation.
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT middleware with Redis session storage, custom auth validation, and auto-renewal. [![Mentioned in Awesome Go](https://awesome.re/mentioned-badge.svg)](https://awesome.re)
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis client with automatic local-storage fallback and transparent reconnection recovery.
- **[go-logger](https://github.com/pardnchiu/go-logger)** — Structured logging via `log/slog` with 8 levels, auto-rotation, and backup management.

---

### Node.js

#### Service

- **[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** — Image upload/caching server (TypeScript). Four-layer cache, WebP default, on-the-fly conversion.

#### Package

- **[node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth)** — Dual-token JWT (Access + Refresh) with ES256, device fingerprinting, Redis-backed revocation, and version-controlled refresh.
- **[node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool)** — MySQL client with read-write pool separation, chainable builder, JOIN/UPSERT support, and slow query detection.

---

### PHP

#### Package

- **[php-async](https://github.com/pardnchiu/php-async)** — ReactPHP-based async task runner with dependency graph resolution via topological sort.
- **[php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli)** — PDO MySQL client with chainable syntax, auto read-write routing, and slow query monitoring.
- **[php-redis-cli](https://github.com/pardnchiu/php-redis-cli)** — Redis client wrapper with persistent connections, multi-database support, and auto-retry.
- **[php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback)** — Redis + filesystem hybrid cache with automatic fallback and HTML/text minification.
- **[php-session-fallback](https://github.com/pardnchiu/php-session-fallback)** — Session manager with Redis primary and filesystem fallback, 7-day lifetime, and auto GC.
- **[php-mailer](https://github.com/pardnchiu/php-mailer)** — PHPMailer wrapper with env-driven SMTP config, multi-recipient, priority, and bulk sending.

---

## Frontend

### JavaScript

#### Framework

- **[QuickUI](https://quickui.pardn.io)** — Lightweight frontend framework on pure JS. Virtual DOM diff/patch, declarative templates (`:for`, `:if`/`:else`, `{{value}}`), reactive data binding, and built-in i18n.

#### Library

- **[NanoMD](https://nanomd.pardn.io)** — Pure JS Markdown library with split-screen editing, sync scrolling, and three independent components (Editor/Viewer/Parser). Mermaid support.
- **[NanoJSON](https://nanojson.pardn.io)** — Zero-dependency JSON visual editor. Tree display with collapsible nodes, live type switching, lifecycle hooks, and import from object/File/URL.
- **[FlexPlyr](https://flexplyr.pardn.io)** — Modular media player for HTML5/YouTube/Vimeo. Customizable controls, multiple themes, zero dependencies.
- **[RenderJS](https://renderjs.pardn.io)** — JS prototype extension library for chainable DOM manipulation and data processing.
- **[pdf2image](https://pdf2image.pardn.io/)** — Client-side PDF to image converter (pdf.js). JPG/PNG/WebP output with optional ZIP packaging.

#### Demo

- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend reproductions (blogs, social UI, smart clock, etc.). All designs are reproductions, not original.
- **[DeskUI](https://github.com/pardnltd/DeskUI)** — Desktop-style windowed web UI built with QuickUI/RenderJS.
- **[WebUI](https://webui.pardn.io)** — Visual drag-and-drop website builder.
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template.
- **[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)** — Icon picker for [skillicons.dev](https://skillicons.dev/).
- **[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)** — Pure CSS Pokemon Quest recreation.

---

### Swift

#### Library

- **[ExSwift](https://github.com/pardnchiu/ExSwift)** — UIKit extension library with SwiftUI-style chainable syntax (UIView → ExZStack, UILabel → ExText, etc.). `Refactoring`

#### Demo

- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** — SwiftUI component reproductions from Pinterest designs, with YouTube demos.
- **[demo-swift-firebase-messaging](https://github.com/pardnchiu/demo-swift-firebase-messaging)** — Firebase messaging app with QR code friend-adding and dark mode. UIKit + ExSwift.
- **[demo-swift-moneybook](https://github.com/pardnchiu/demo-swift-moneybook)** — Expense tracking UI with monthly/daily views. UIKit + ExSwift.

---

## Product

### Web
- **[JOBALL](https://joball.tw)** — Expert matching platform in Taiwan.

### macOS
- **[NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** — Native Markdown editor with Mermaid support.
- **[Ninlog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** — Keyboard and mouse activity tracker.

### Chrome Extension
- **[C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — Cross-domain real-time chat.

### VS Code Extension
- **[NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with real-time preview.

### Discontinued
- **[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)** — Expert matching platform. *Discontinued.*
