> My code is my pitch — if it doesn't resonate, no worries.

<table><tr><td valign="top" width="33%">

### Recent
- **[ThreadsMarketing (v0.1.0)](https://github.com/pardnchiu/ThreadsMarketing/releases/tag/v0.1.0)** — Initial release with TUI dashboard, Threads OAuth login flow, and startup token verification.
- **[go-utils (v0.1.3)](https://github.com/pardnchiu/go-utils/releases/tag/v0.1.3)** — Add generic PUT, PATCH, DELETE HTTP methods by extracting a shared `send` helper from the existing POST implementation.
- **[go-utils (v0.1.2)](https://github.com/pardnchiu/go-utils/releases/tag/v0.1.2)** — Add `Init` function with `sync.Once` to keychain package and simplify public API by removing per-call `service`/`fallbackPath` parameters.
- **[go-utils (v0.1.1)](https://github.com/pardnchiu/go-utils/releases/tag/v0.1.1)** — Replace hardcoded service name in keychain package with a caller-provided `service` parameter, changing the public API signature of `Get`, `Set`, and `Delete`.
- **[go-utils (v0.1.0)](https://github.com/pardnchiu/go-utils/releases/tag/v0.1.0)** — Initial release of personal Go utility package with generic HTTP client, atomic file writer, and cross-platform keychain integration.
- **[Agenvoy (v0.18.0)](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.18.0)** — Introduces vim-style TUI navigation with command input mode, consolidates CLI and server into a unified `agen` entrypoint, and migrates session history, error memory, and web/page caches from JSON/filesystem storage to ToriiDB.
- **[ToriiDB (v0.4.3)](https://github.com/pardnchiu/ToriiDB/releases/tag/v0.4.3)** — Switch AOF compaction trigger from line count to byte size with a 1MB floor, so compaction reflects actual disk waste and replay cost instead of record count.
- **[ToriiDB (v0.4.2)](https://github.com/pardnchiu/ToriiDB/releases/tag/v0.4.2)** — STrigger AOF compaction inline on writes when the inflation ratio (AOF lines / live keys) reaches 2x, with a minimum live-key threshold to avoid wasteful rewrites on small databases.
- **[ToriiDB (v0.4.1)](https://github.com/pardnchiu/ToriiDB/releases/tag/v0.4.1)** — SExtract shared `core` struct to enable `Session` support, add lazy DB replay and parallel compaction for faster startup/shutdown, replace channel-based cancellation with `context.Context`, support custom storage path via `New(path)`, and sync Expire/Persist changes to JSON cache files.
- **[ToriiDB (v0.4.0)](https://github.com/pardnchiu/ToriiDB/releases/tag/v0.4.0)** — SAdd NE (not equal) comparison operator, extract a dedicated filter package with an infix expression parser supporting AND/OR/NOT logical operators, and add concurrent slice scan for FIND/QUERY when data exceeds 1024 entries.

</td><td valign="top" width="33%">

### Backend

**Go/Framework**
- **[Agenvoy](https://github.com/pardnchiu/Agenvoy)** — AI agent framework with multi-provider LLM routing

**Go/Infrastructure**
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)** — Proxmox VM lifecycle API with SSE streaming
- **[go-faas](https://github.com/pardnchiu/go-faas)** — FaaS runtime with Bubblewrap sandbox
- **[go-podrun](https://github.com/pardnchiu/go-podrun)** — Container deployment CLI via rsync/SSH

**Go/Service**
- **[go-notify-hub](https://github.com/pardnchiu/go-notify-hub)** — Unified API for Discord / Slack / LINE / Email
- **[go-rest-client](https://github.com/pardnchiu/go-rest-client)** — TUI REST client, `.http` file compatible
- **[go-web-monitor](https://github.com/pardnchiu/web-monitor)** — Uptime + SSL expiry monitor
- **[go-rss-reader](https://github.com/pardnchiu/rss-reader)** — TUI RSS reader with full-text extraction
- **[go-image-server](https://github.com/pardnchiu/demo-go-image-server)** — Four-layer cache, on-the-fly WebP conversion

**Go/Package**
- **[go-utils](https://github.com/pardnchiu/go-utils)** — Personal Go utility functions for rapid development
- **[ToriiDB](https://github.com/pardnchiu/ToriiDB)** — Embedded JSON document DB, zero dependencies
- **[go-sqlite](https://github.com/pardnchiu/go-sqlite)** · **[go-pg](https://github.com/pardnchiu/go-pg)** · **[go-mysql](https://github.com/pardnchiu/go-mysql)** — SQL clients with read-write separation
- **[go-queue](https://github.com/pardnchiu/go-queue)** — Worker pool with priority scheduling
- **[go-scheduler](https://github.com/pardnchiu/go-scheduler)** — Cron scheduler with dependency chains
- **[go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry)** — GeoIP threat scoring + progressive ban
- **[go-jwt](https://github.com/pardnchiu/go-jwt)** — JWT middleware with Redis session + auto-renewal
- **[go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback)** — Redis with auto local-storage failover

**Node.js**
- **[node-image-server](https://github.com/pardnchiu/demo-node-image-server)** — Four-layer cache, WebP default (TypeScript)
- **[node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth)** — ES256 JWT with device fingerprint + revocation
- **[node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool)** — MySQL pool, read-write split + slow query detection

**PHP**
- **[php-async](https://github.com/pardnchiu/php-async)** — Async task runner with dependency graph resolution
- **[php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli)** — PDO MySQL client, auto read-write routing
- **[php-redis-cli](https://github.com/pardnchiu/php-redis-cli)** — Redis client with persistent connections + auto-retry
- **[php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback)** — Redis + filesystem hybrid cache with auto fallback
- **[php-session-fallback](https://github.com/pardnchiu/php-session-fallback)** — Session manager, Redis primary with filesystem fallback
- **[php-mailer](https://github.com/pardnchiu/php-mailer)** — SMTP mailer with multi-recipient + priority sending

</td><td valign="top" width="33%">

### Frontend & Product

#### Frontend

**Framework**
- **[QuickUI](https://quickui.pardn.io)** — Virtual DOM framework on pure JS with reactive binding

**Library**
- **[NanoMD](https://nanomd.pardn.io)** — Split-pane Markdown editor with Mermaid
- **[NanoJSON](https://nanojson.pardn.io)** — Interactive JSON tree editor, zero dependencies
- **[FlexPlyr](https://flexplyr.pardn.io)** — HTML5 / YouTube / Vimeo unified player
- **[RenderJS](https://renderjs.pardn.io)** — Chainable DOM manipulation via prototype extension
- **[pdf2image](https://pdf2image.pardn.io/)** — Client-side PDF to JPG/PNG/WebP

**Swift**
- **[ExSwift](https://github.com/pardnchiu/ExSwift)** — UIKit extension with SwiftUI-style chaining `Refactoring`

**Demo**
- **[demo-web](https://github.com/pardnchiu/demo-web)** — 30+ frontend reproductions
- **[DeskUI](https://github.com/pardnltd/DeskUI)** — Desktop-style windowed web UI
- **[WebUI](https://webui.pardn.io)** — Visual drag-and-drop website builder
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template
- **[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)** — Icon picker for skillicons.dev
- **[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)** — Pure CSS Pokemon Quest recreation
- **[demo-swiftui](https://github.com/pardnchiu/demo-swiftui)** — SwiftUI component reproductions

***

#### Product

**Web**
- **[JOBALL](https://joball.tw)** — Freelance expert marketplace (Taiwan)

**macOS**
- **[NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** — Native Markdown editor with Mermaid
- **[Ninlog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** — Keyboard & mouse activity tracker

**Chrome Extension**
- **[C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — Cross-origin real-time chat

**VS Code Extension**
- **[NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with live preview

**Discontinued**
- **[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)** — Freelance expert marketplace (Taiwan)

</td></tr></table>
