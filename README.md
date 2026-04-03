> My code is my pitch — if it doesn't resonate, no worries.

## [Agenvoy](https://github.com/pardnchiu/agenvoy) — Agentic framework
Agenvoy is inspired by OpenClaw, built on a Go-based architecture with multi-provider intelligent dispatch and a security-first design.

- **[v0.17.4](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.4)** — Add OpenAI Codex as a standalone OAuth provider (Device Code Flow with auto-refresh, default model `gpt-5.3-codex`). Add `read_image` tool to read local image files as base64 data URLs — supports JPEG, PNG, GIF, WebP up to 10 MB, decoded and re-encoded as JPEG. Restore Yahoo Finance as a native Go tool (`fetch_yahoo_finance`) with concurrent dual-endpoint fetch (query1/query2) replacing the removed JSON API extensions. Fix summary generation reliability by completing the summary workflow before final completion signaling. Fix tool fallback handling for `search_history` and `fetch_google_rss` when models send `query` instead of `keyword`. Fix event logging crashes on tool errors without `Err`. Fix stale `discussion_log` retention by filtering entries older than the oldest active context. Fix nil-safe operations and fill missing CRUD coverage in scheduler task and cron flows. Update news-retrieval system prompt with mandatory fallback windows `1h → 24h → 7d → search_web`. Refactor summary extraction into a dedicated workflow; simplify provider startup paths.
- **[v0.17.3](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.3)** — Add `search_tools` deferred tool loading — agents discover and activate tools on demand using keyword fuzzy search or `select:<name>` direct selection, reducing context overhead on large tool sets. Add `exclude_tools` parameter to `/v1/send` for per-request tool filtering. Add prompt caching across Claude, Gemini, and Copilot providers to reduce latency and token cost. Auto-prompt LLM to record error patterns after successful tool retry. Refactor scheduler into `crons/` / `tasks/` / `script/` sub-packages with file-based state persistence; replace network skill sync with embedded FS copy; overhaul file tools with binary detection and PDF page-range reading.
- **[v0.17.2](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.2)** — Add `call_external_agent`, `verify_with_external_agent`, and `review_result` tools for external delegation and internal priority-model review. Refactor session message assembly into 4 fixed segments (SystemPrompts / OldHistories / UserInput / ToolHistories) with reactive context trimming on context-length errors. Add `model` field to `/v1/send` request to bypass automatic agent selection.
- **[v0.17.1](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.1)** — Fix build break caused by importing the missing `externalAgent` package before it existed in the repository.
- **[v0.17.0](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.0)**  — Full REST API layer with `/v1/send` (SSE + non-SSE), `/v1/key`, `/v1/tools`, `/v1/tool/:name` endpoints. TUI dashboard complete with file browser, session viewer, and live log stream. Discord bot and REST API unified under `cmd/app`. Copilot token migrated to system keychain. Renamed `browser` package to `fetchPage`. Updated `schedule-task` and `script-tool-creator` skills to invoke tools via Agenvoy API instead of direct external calls.

***

## Backend (Go / Node.js / PHP)

<details>

### Go

#### Platform / Infrastructure
- **[go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu)**
  Proxmox VE VM automation REST API — full lifecycle provisioning via SSE, concurrent IP & CPU architecture auto-allocation, and transparent multi-node cluster routing. Successor: [go-kvmesh](https://github.com/pardnchiu/go-kvmesh) `WIP` / [go-qemu](https://github.com/pardnchiu/go-go-qemu) `WIP`

- **[go-faas](https://github.com/pardnchiu/go-faas)** 
  Function-as-a-Service platform that accepts code via HTTP API and executes it securely inside a Bubblewrap sandbox.

- **[go-podrun](https://github.com/pardnchiu/go-podrun)**
   CLI tool that syncs local projects to remote servers via rsync/SSH and runs Podman Compose workloads — with a local SQLite deployment registry for container lifecycle tracking.

#### Services
- [go-notify-hub](https://github.com/pardnchiu/go-notify-hub) — Multi-channel notification hub (Discord, Slack, LINE, Email)
- [go-rest-client](https://github.com/pardnchiu/go-rest-client) — TUI-based REST API tester with .http file compatibility
- [JsonDB](https://github.com/pardnchiu/JsonDB) — JSON database example combining key-value and document query
- [go-web-monitor](https://github.com/pardnchiu/web-monitor) — Website monitor with SSL tracking and email alerts
- [go-rss-reader](https://github.com/pardnchiu/rss-reader) — Terminal RSS aggregator with LLM summarization
- [go-image-server](https://github.com/pardnchiu/demo-go-image-server) — Image caching server with on-the-fly processing and CDN integration

#### Packages
- **SQL Clients** (chainable query builders)
  - [go-sqlite](https://github.com/pardnchiu/go-sqlite) — SQLite
  - [go-pg](https://github.com/pardnchiu/go-pg) — PostgreSQL
  - [go-mysql](https://github.com/pardnchiu/go-mysql) — MySQL / MariaDB
- [go-queue](https://github.com/pardnchiu/go-queue) — Priority-based task queue with automatic timeout promotion
- [go-scheduler](https://github.com/pardnchiu/go-scheduler) — Scheduler with standard cron and task dependencies <img src="https://awesome.re/mentioned-badge.svg" height="16px">
- [go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry) — IP threat detection with automatic blacklisting
- [go-jwt](https://github.com/pardnchiu/go-jwt) — JWT authentication with auto-renewal <img src="https://awesome.re/mentioned-badge.svg" height="16px">
- [go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback) — Redis client with graceful fallback
- [go-logger](https://github.com/pardnchiu/go-logger) — Logging client with automatic rotation

### Node.js

#### Services
- [node-image-server](https://github.com/pardnchiu/demo-node-image-server) — Image upload and caching server

#### Packages
- [node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth) — JWT system with auto-renewal
- [node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool) — MySQL client with chained method calls

### PHP

#### Packages
- [php-async](https://github.com/pardnchiu/php-async) — Async task dependency manager
- [php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli) — PDO wrapper for MySQL with chained method calls
- [php-redis-cli](https://github.com/pardnchiu/php-redis-cli) — Redis client wrapper
- [php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback) — Cache manager with graceful fallback
- [php-session-fallback](https://github.com/pardnchiu/php-session-fallback) — Session manager with graceful fallback
- [php-mailer](https://github.com/pardnchiu/php-mailer) — PHPMailer wrapper

</details>
  
---

## Frontend (Web / Swift)

<details>

### Web (HTML / CSS / JS)

#### Libraries
- [QuickUI](https://quickui.pardn.io) — Lightweight frontend framework
- [NanoMD](https://nanomd.pardn.io) — Markdown editor with real-time preview
- [NanoJSON](https://nanojson.pardn.io) — Firebase-like JSON editor
- [FlexPlyr](https://flexplyr.pardn.io) — Media player with multiple styles
- [RenderJS](https://renderjs.pardn.io) — DOM rendering library
- [pdf2image](https://pdf2image.pardn.io/) — PDF-to-image converter

#### Demos
- [demo-web](https://github.com/pardnchiu/demo-web) — Explore over 30 frontend examples
- [DeskUI](https://github.com/pardnltd/DeskUI) — Desktop-style web UI
- [WebUI](https://webui.pardn.io) — Visual website builder
- [AdminUI](https://adminui.pardn.io) — Admin dashboard template
- [SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/) — Easy way to choose icons from [skillicons.dev](https://skillicons.dev/)
- [css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/) — Pokemon Quest

### Swift (iOS / macOS)

#### Libraries
- [ExSwift](https://github.com/pardnchiu/ExSwift) — Swift extension utilities

#### Demos
- [demo-swiftui](https://github.com/pardnchiu/demo-swiftui) — Demo with SwiftUI
- [demo-swift-firebase-messaging](https://github.com/pardnchiu/demo-swift-firebase-messaging) — Messaging demo with Firebase and UIKit
- [demo-swift-moneybook](https://github.com/pardnchiu/demo-swift-moneybook) — Moneybook UI demo with UIKit

</details>

---

## Production

<details>

### Website
- [JOBALL](https://joball.tw) — Expert matching platform in Taiwan

### macOS
- [NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920) — Markdown editor
- [Ninlog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238) — Keyboard and mouse activity tracker

### Chrome Extension
- [C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn) — Cross-domain chat extension

### VSCode Extension
- [NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd) — Markdown editor

### Discontinued

#### iOS
- [JOBALL](https://apps.apple.com/us/app/joball-接洽/id1272878907) — Expert matching platform (Discontinued)

</details>
