Last updated: 2026-10-31

# 邱敬幃 Pardn Chiu

> **Show code, not just words — my code is my pitch.**<br>
> Taiwan · Infrastructure Engineering<br>
> Started in iOS, expert in web frontend and backend, now focused on infrastructure.
>
> My GitHub is all infrastructure and foundational components.<br>
> Core functionality first — less bloat, fewer gimmicks.<br>
> If you're a developer, every tool here is yours to use.

**Project notes**

1. Test files and SKILL repos (including Python scripts) are all LLM-generated; I only review their input/output.
2. pardnio stores archived repos, and pardnchiu maintains modules and libraries.

---

<a href="https://agenvoy.com/"><img src="https://avatars.githubusercontent.com/u/260084267?s=200&v=4" align="left" width=96 height=96></a>

### [Agenvoy](https://agenvoy.com/)

Make AI actually work for you<br>
A local AI agent harness in Go that runs 24/7 with auto-built tools, MCP, and Ollama

---

### Backend

<details open>

<summary>Go/AI Agent (6)</summary>

- **[go-llm-router](https://go-llm-router.pardn.io)** — ONE AGENT INTERFACE FOR EVERY LLM PROVIDER
- **[go-browser](https://go-browser.pardn.io)** — EXTRACT WEB CONTENT VIA CHROME — MARKDOWN OR HTML, READY FOR AGENTS
- **[go-bot](https://go-bot.pardn.io)** — BUILD BOTS THAT FIT EVERY CHAT PLATFORM
- **[ToriiDB](https://toriidb.pardn.io)** — EMBEDDED JSON KV STORAGE WITH A SHARED SOCKET DAEMON AND VECTOR SEARCH
- **[KuraDB](https://kuradb.pardn.io)** — DROP FILES IN, LET YOUR AGENT SEARCH THEM OUT
- **[cim-prototype](https://github.com/pardnio/cim-prototype)** — LLM with a Cognitive Imperfect Memory system that simulates human selective memory for long multi-turn conversations

</details>

<details open>

<summary>Go/Self-hosted Infra (4)</summary>

- **[HakoRun](https://hakorun.pardn.io)** — SELF-HOSTED FAAS, NO DOCKER OR KUBERNETES REQUIRED
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — ONE API CALL FROM CLOUD IMAGE TO SSH-READY VM ON PROXMOX VE
- **[PodRun](https://podrun.pardn.io)** — DEPLOY TO REMOTE PODMAN AND K3S LIKE LOCAL DOCKER COMPOSE
- **[go-image-server](https://go-image-server.pardn.io)** — RESIZE ONCE, CACHE EVERYWHERE

</details>

<details open>

<summary>Go/Backend Toolkit (9)</summary>

- **[go-queue](https://go-queue.pardn.io)** — PRIORITY TASKS THAT NEVER STARVE
- **[go-scheduler](https://go-scheduler.pardn.io)** — SCHEDULE TASKS WITH DEPENDENCIES, TIMEOUTS, AND CRON EXPRESSIONS [![Awesome Go](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-jwt](https://go-jwt.pardn.io)** — ECDSA JWT WITH REDIS LIFECYCLE AND DEVICE BINDING [![Awesome Go](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-ip-sentry](https://go-ip-sentry.pardn.io)** — STOP MALICIOUS IPS BEFORE THEY REACH YOUR HANDLERS
- **[go-redis-fallback](https://go-redis-fallback.pardn.io)** — KEEP READING WHEN REDIS GOES DOWN (KV local storage implementation before ToriiDB)
- (Others) [go-web-monitor](https://go-web-monitor.pardn.io), [go-rss-reader](https://go-rss-reader.pardn.io), [go-rest-client](https://go-rest-client.pardn.io), [go-logger](https://github.com/pardnio/go-logger)

</details>

<details open>

<summary>Node.js (3)</summary>

- **[node-image-server](https://node-image-server.pardn.io)** — RESIZE ONCE, SERVE FROM CACHE EVERYWHERE (earlier Node.js implementation, continued in Go as go-image-server)
- **[node-jwt-auth](https://node-jwt-auth.pardn.io)** — DUAL-TOKEN JWT AUTH BOUND TO EVERY DEVICE (earlier Node.js implementation, continued in Go as go-jwt)
- **[node-mysql-pool](https://node-mysql-pool.pardn.io)** — CHAIN YOUR MYSQL QUERIES ACROSS READ AND WRITE POOLS

</details>

<details open>

<summary>PHP (6)</summary>

- **[php-async](https://github.com/pardnio/php-async)** — DECLARE THE DEPENDENCIES, LET THE PROMISES RUN THEM
- **[php-mysql-cli](https://github.com/pardnio/php-mysql-cli)** — CHAIN YOUR QUERIES, NOT YOUR STRINGS (earlier PHP implementation, continued in Node.js as node-mysql-pool)
- (Others) [php-redis-cli](https://github.com/pardnio/php-redis-cli), [php-cache-fallback](https://github.com/pardnio/php-cache-fallback), [php-session-fallback](https://github.com/pardnio/php-session-fallback), [php-mailer](https://github.com/pardnio/php-mailer)

</details>

<details open>

<summary>Infra/Shell (1)</summary>

- [pdpve](https://github.com/pardnio/pdpve) (earlier Shell implementation, continued in Go as QemuRun-pve)

</details>

---

### Frontend

<details open>

<summary>Framework/Library (6)</summary>

- **[QuickUI](https://quickui.pardn.io)** — A ZERO-DEPENDENCY VIRTUAL DOM FRAMEWORK THAT RUNS WITHOUT A BUILD STEP
- **[NanoMD](https://nanomd.pardn.io)** — FAST MARKDOWN TO AST AND HTML IN ONE PARSER
- **[NanoJSON](https://nanojson.pardn.io)** — A LIGHTWEIGHT VISUAL JSON EDITOR BUILT WITH PURE JAVASCRIPT
- **[FlexPlyr](https://flexplyr.pardn.io)** — ONE PLAYER API FOR HTML5, YOUTUBE AND VIMEO
- **[RenderJS](https://renderjs.pardn.io)** — EXTEND NATIVE JS PROTOTYPES, RENDER WITHOUT THE OVERHEAD
- **[pdf2image](https://pdf2image.pardn.io)** — TURN ANY PDF INTO IMAGES RIGHT IN THE BROWSER

</details>

<details open>

<summary>Demo/Web (7)</summary>

- **[demo-web](https://demo-web.pardn.io)** — 38 HANDCRAFTED FRONTEND PAGES, ZERO BUILD STEP
- **[WebUI](https://pardnio.github.io/WebUI/)** — PICK A TEMPLATE, CLICK TO EDIT, SHIP A PAGE
- (Others) [AdminUI](https://pardnio.github.io/AdminUI/), [DeskUI](https://pardnio.github.io/DeskUI/), [css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/), [SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/), [web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)

</details>

<details open>

<summary>iOS (4)</summary>

- **[ExSwift](https://github.com/pardnio/ExSwift)** — Declarative UIKit extension with fluent chaining syntax
- **[demo-swiftui](https://github.com/pardnio/demo-swiftui)** — SwiftUI components recreating Pinterest-style animated UI
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** — REAL-TIME CHAT ON IOS, BUILT WITH PURE CODE AND FIREBASE
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)** — BUILD A WHOLE UIKIT BOOKKEEPING APP IN CHAINS

</details>

---

### Product

<details open>

<summary>Shipped (7)</summary>

- **[JOBALL (Web)](https://joball.tw)** — Freelance expert marketplace (Taiwan) · **peak 10K users / 340K monthly views**
- **[C2hat (Chrome Extension)](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — E2EE cross-domain chat extension with no server-side message storage
- **[NanoMD (VS Code Extension)](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown editor with split-screen preview and Mermaid support
- **[NanoMD (Chrome Extension)](https://chromewebstore.google.com/detail/nanomd/pdklinlfmpobpakengplkhbbneaamijd)** — Renders Markdown files right in Chrome
- (Discontinued) **[NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** ・
  **[Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** ・
  **[JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)**

</details>
