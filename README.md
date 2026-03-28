## [Agenvoy](https://github.com/pardnchiu/agenvoy) — Agentic framework
Agenvoy is inspired by OpenClaw, built on a Go-based architecture with multi-provider intelligent dispatch and a security-first design.

- **[v0.17.0](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.17.0)**  — Full REST API layer with `/v1/send` (SSE + non-SSE), `/v1/key`, `/v1/tools`, `/v1/tool/:name` endpoints. TUI dashboard complete with file browser, session viewer, and live log stream. Discord bot and REST API unified under `cmd/app`. Copilot token migrated to system keychain. Renamed `browser` package to `fetchPage`. Updated `schedule-task` and `script-tool-creator` skills to invoke tools via Agenvoy API instead of direct external calls.
- **[v0.16.1](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.16.1)** — Bundled Threads (publish text/image/carousel, quota, token refresh) and yt-dlp (video info, download) script tool extensions with cross-platform `install_threads.sh` / `install_youtube.sh`. Refactor `toolAdapter` into `api/` and `script/` sub-packages; move session management to `internal/session`; split filesystem into single-responsibility files. Fix Darwin sandbox keychain directory access. Restrict tool call throttle to `api_` prefix; improve `AbsPath` tilde expansion and exclude logic deduplication.
- **[v0.16.0](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.16.0)** — Script tool runtime (`scriptAdapter`): drop a `tool.json` + `script.js`/`script.py` into `~/.config/agenvoy/script_tools/` and it is auto-discovered as a `script_`-prefixed tool; stdin/stdout JSON protocol mirrors API tool contract. Refactor `tools/apis/adapter` → `apiAdapter`, `tools/apis` → `tools/api`. Add `skill_git_commit`, `skill_git_log`, `skill_git_rollback` for skill-internal versioning. Copilot token auto-relogin on 401. Fix Discord file upload failure for non-ASCII filenames; add 10MB pre-upload size guard with user-facing warning.
- **[v0.15.2](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.15.2)** — Add YouTube metadata fetch tool (`analyze_youtube`); Discord Modal-based API key management (`/add-gemini`, `/add-openai`, `/add-claude`, `/add-nim`); per-model token usage tracking via `usageManager`; configurable reasoning level across all providers; browser iteration limits and same-domain link traversal now configurable via `MAX_TOOL_ITERATIONS`, `MAX_SKILL_ITERATIONS`, `MAX_EMPTY_RESPONSES`; fix Makefile pass-through args
- **[v0.15.1](https://github.com/pardnchiu/Agenvoy/releases/tag/v0.15.1)** — Fix Copilot Claude/Gemini image validation failure: all uploaded images are decoded and re-encoded as JPEG (`image.Decode` + `jpeg.Encode`, supporting PNG/GIF/WebP sources), `ImageURL` gains `detail` field; summary regex split from one monolithic expression into three independent patterns (fenced block, `<summary>` tag, `[summary]` bracket); system prompts moved after history to improve model instruction adherence; Discord prompt takes priority over base system prompt

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
