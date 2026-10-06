Last updated: 2026-10-07

# 邱敬幃 Pardn Chiu

> **Show code, not just words — my code is my pitch.**<br>
> Taiwan · Infrastructure Engineering
>
> AI is a tool; your own expertise is what counts.<br>
> Don't use AI to design your architecture.<br>
> Use it to catch bugs and sharpen algorithms — that's what it's actually good at.

***

<a href="https://github.com/agenvoy/Agenvoy"><img src="https://avatars.githubusercontent.com/u/260084267?s=200&v=4" align="left" width=96 height=96></a>

### [Agenvoy](https://github.com/agenvoy/Agenvoy)

Make AI actually work for you<br>
Self-hosted AI agent harness in a single Go binary — writes, sandbox-tests and repairs its own tools, and lets Claude Code, Codex and any MCP client build and share them.

***

### Backend

<details open>

<summary>Go/Service (8)</summary>

- **[KuraDB](https://kuradb.pardn.io)** — DROP FILES IN, LET YOUR AGENT SEARCH THEM OUT
- **[HakoRun](https://hakorun.pardn.io)** — SELF-HOSTED FAAS, NO DOCKER OR KUBERNETES REQUIRED
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — ONE API CALL FROM CLOUD IMAGE TO SSH-READY VM ON PROXMOX VE
- **[PodRun](https://podrun.pardn.io)** — DEPLOY TO REMOTE PODMAN AND K3S LIKE LOCAL DOCKER COMPOSE
- **[go-rest-client](https://go-rest-client.pardn.io)** — RUN YOUR .HTTP FILES RIGHT IN THE TERMINAL
- **[go-web-monitor](https://go-web-monitor.pardn.io)** — KEEP EVERY SITE IN SIGHT, RIGHT FROM YOUR TERMINAL
- **[go-rss-reader](https://go-rss-reader.pardn.io)** — READ THE NEWS, NOT THE NOISE, RIGHT IN YOUR TERMINAL
- **[go-image-server](https://go-image-server.pardn.io)** — RESIZE ONCE, CACHE EVERYWHERE

</details>

<details open>

<summary>Go/Module (12)</summary>

- **[go-llm-router](https://go-llm-router.pardn.io)** — ONE AGENT INTERFACE FOR EVERY LLM PROVIDER
- **[go-sqlkit](https://github.com/pardnchiu/go-sqlkit)** — Unified SQL toolkit for MySQL/MariaDB/SQLite with read-write splitting
- **[go-browser](https://go-browser.pardn.io)** — EXTRACT WEB CONTENT VIA CHROME — MARKDOWN OR HTML, READY FOR AGENTS
- **[go-bot](https://go-bot.pardn.io)** — BUILD BOTS THAT FIT EVERY CHAT PLATFORM
- **[ToriiDB](https://toriidb.pardn.io)** — EMBEDDED JSON KV STORAGE WITH A SHARED SOCKET DAEMON AND VECTOR SEARCH
- **[go-queue](https://go-queue.pardn.io)** — PRIORITY TASKS THAT NEVER STARVE
- **[go-ip-sentry](https://go-ip-sentry.pardn.io)** — STOP MALICIOUS IPS BEFORE THEY REACH YOUR HANDLERS
- **[go-scheduler](https://go-scheduler.pardn.io)** — SCHEDULE TASKS WITH DEPENDENCIES, TIMEOUTS, AND CRON EXPRESSIONS <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-jwt](https://go-jwt.pardn.io)** — ECDSA JWT WITH REDIS LIFECYCLE AND DEVICE BINDING <a href="https://github.com/avelino/awesome-go"><img src="https://awesome.re/mentioned-badge.svg" height="20"></a>
- **[go-redis-fallback](https://go-redis-fallback.pardn.io)** — KEEP READING WHEN REDIS GOES DOWN
- **[go-pkg](https://github.com/pardnchiu/go-pkg)** — Personal Go toolkit: generic HTTP client, policy-aware filesystem, OS-native sandbox
- (Archived) **[go-logger](https://github.com/pardnio/go-logger)** — DEPRECATED — MIGRATE TO LOG/SLOG

</details>


<details open>

<summary>Node.js (3)</summary>

- **[node-image-server](https://node-image-server.pardn.io)** — Multi-tier image cache (browser / Cloudflare Worker / Nginx / local) with WebP/AVIF conversion
- **[node-jwt-auth](https://node-jwt-auth.pardn.io)** — Dual-token JWT auth with device fingerprinting, ES256, and Redis revocation
- **[node-mysql-pool](https://node-mysql-pool.pardn.io)** — MySQL pool with read/write split and a fluent query builder

</details>


<details open>

<summary>PHP (6)</summary>

- **[php-async](https://github.com/pardnio/php-async)** — ReactPHP async task runner with topological dependency sorting
- **[php-mysql-cli](https://github.com/pardnio/php-mysql-cli)** — Chainable MySQL client with read-write routing and retry resilience
- **[php-redis-cli](https://github.com/pardnio/php-redis-cli)** — Redis client over the native extension with persistent multi-DB connections
- **[php-cache-fallback](https://github.com/pardnio/php-cache-fallback)** — Hybrid Redis + filesystem cache with automatic fallback
- **[php-session-fallback](https://github.com/pardnio/php-session-fallback)** — Redis session manager with filesystem fallback and hardening
- **[php-mailer](https://github.com/pardnio/php-mailer)** — PHPMailer SMTP wrapper with rate-limited bulk sending

</details>

<details open>

<summary>Infra/Shell (1)</summary>

- **[pdpve](https://github.com/pardnio/pdpve)** — Bash scripts for Proxmox VE

</details>

***

### Frontend

<details open>

<summary>Framework/Library (6)</summary>

- **[QuickUI](https://quickui.pardn.io)** — A ZERO-DEPENDENCY VIRTUAL DOM FRAMEWORK THAT RUNS WITHOUT A BUILD STEP <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/quickui" height="20">
- **[NanoMD](https://nanomd.pardn.io)** — LIGHTWEIGHT MARKDOWN EDITOR IN PURE JAVASCRIPT <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanomd" height="20">
- **[NanoJSON](https://nanojson.pardn.io)** — A LIGHTWEIGHT VISUAL JSON EDITOR BUILT WITH PURE JAVASCRIPT <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/nanojson" height="20">
- **[FlexPlyr](https://flexplyr.pardn.io)** — ONE PLAYER API FOR HTML5, YOUTUBE AND VIMEO <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/flexplyr" height="20">
- **[RenderJS](https://renderjs.pardn.io)** — EXTEND NATIVE JS PROTOTYPES, RENDER WITHOUT THE OVERHEAD <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/renderjs" height="20">
- **[pdf2image](https://pdf2image.pardn.io)** — TURN ANY PDF INTO IMAGES RIGHT IN THE BROWSER <img src="https://img.shields.io/jsdelivr/npm/hm/@pardnchiu/pdf2image" height="20">

</details>

<details open>

<summary>Demo/Web (7)</summary>

- **[demo-web](https://demo-web.pardn.io)** — 38 HANDCRAFTED FRONTEND PAGES, ZERO BUILD STEP
- **[WebUI](https://webui.pardn.io)** — Visual website builder with modular prebuilt templates (WIP)
- **[AdminUI](https://adminui.pardn.io)** — Admin dashboard template built on QuickUI, NanoMD, NanoJSON, FlexPlyr
- **[DeskUI](https://pardnio.github.io/DeskUI/)** — Desktop-style web UI
- **[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)** — Pokémon Quest characters drawn in pure CSS
- **[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)** — Pick, sort and generate Skill Icons links
- **[web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)** — Admin dashboard template (2022 edition)

</details>

<details open>

<summary>iOS (4)</summary>

- **[ExSwift](https://github.com/pardnio/ExSwift)** — Declarative UIKit extension with fluent chaining syntax
- **[demo-swiftui](https://github.com/pardnio/demo-swiftui)** — SwiftUI components recreating Pinterest-style animated UI
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** — Firebase chat app with QR friend-adding, code-only UIKit
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)** — UIKit finance tracker with monthly views and Font Awesome

</details>

***

### Product

<details open>

- **[JOBALL (Web)](https://joball.tw)** — Freelance expert marketplace (Taiwan) · **peak 10K users / 340K monthly views**
- **[C2hat (Chrome Extension)](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — E2EE cross-domain chat extension with no server-side message storage
- **[NanoMD (VS Code Extension)](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with split-screen preview and Mermaid support
- (Discontinued) **[NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** ・ 
**[Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** ・ 
**[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)**
  
</details>
