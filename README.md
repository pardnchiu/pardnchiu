Last updated: 2026-11-18

# Pardn Chiu (邱敬幃)

> **Show code, not just words — my code is my pitch.**<br>
> Taiwan · Infrastructure Engineering<br>
> Started in iOS, expert in web frontend and backend, now focused on infrastructure.

---

<a href="https://agenvoy.com/"><img src="https://avatars.githubusercontent.com/u/260084267?s=200&v=4" align="left" width=96 height=96></a>

### [Agenvoy](https://agenvoy.com/)

**A private AI agent that runs 24/7 as a daemon on your own machine, shipped as a single Go binary.**<br>
Describe a task in one sentence and Agenvoy plans the steps, calls tools, and delivers the result. When no tool fits, it writes a new one, tests it in a sandbox, and keeps it for reuse.

<br clear="left"/>

- **Builds its own tools** — finds a keyless public API or writes a new tool, then shares the same sandboxed tool library with Claude Code, Codex, and any MCP agent
- **Local-first by design** — sessions, memory, and schedules live in SQLite on your disk; credentials stay in the OS keychain; commands run under `sandbox-exec` / `bwrap` with network off by default
- **Automation in one sentence** — natural-language cron schedules that run on your machine and push results to Telegram or Discord, with no inbound ports opened
- **Any model** — 15 LLM providers plus local Ollama / LM Studio, with task-based routing, MCP (stdio/HTTP), image generation, STT, and TTS
- **Visible and controllable** — streaming TUI and Web dashboard, confirmation gates for sensitive paths, and hands-free voice mode with wake word

---

### AI

- **[go-llm-router](https://go-llm-router.pardn.io)** — Unified Go interface for 15 LLM providers. Resolve any model from a `provider@model` string, normalize six reasoning levels across Claude, Gemini, and OpenAI, and fold every vendor's token and cache usage into one shape. Extracted from Agenvoy, which now runs entirely on it.
- **[ToriiDB](https://toriidb.pardn.io)** — Embedded Go JSON key-value store with built-in vector search. The first process on a data directory becomes a shared unix-socket daemon, writes are fsynced to an append log with atomic snapshot compaction, and 17 Redis-style commands run across 16 databases.

### Infrastructure

- **[HakoRun](https://hakorun.pardn.io)** — Self-hosted FaaS without Docker or Kubernetes. Upload a Python, JS, or TS function and call it over HTTP; each run is isolated in Bubblewrap (all namespaces unshared, no network, capabilities dropped), capped by a systemd slice, and streamed back over SSE with timestamp-pinned versions.
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — One API call from an official cloud image to an SSH-ready VM on Proxmox VE. Handles concurrent VMID/IP allocation, detects the cluster-wide common CPU baseline to keep VMs migratable, and dispatches `qm` across nodes over SSH, with every provisioning stage streamed over SSE.

### Libraries

- **[go-queue](https://go-queue.pardn.io)** — Priority task queue with five levels on one min-heap, anti-starvation promotion, a dedicated retry tier, panic isolation, and deadline-bound graceful shutdown.
- **[go-scheduler](https://go-scheduler.pardn.io)** — Cron scheduler with task dependency chains (stop or skip on failure), per-task timeouts, and a min-heap event loop that supports adding and removing tasks at runtime. [![Awesome Go](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-jwt](https://go-jwt.pardn.io)** — ES256 JWT with instant revocation through a Redis JTI whitelist, device-fingerprint binding, and lock-guarded refresh rotation that stays safe across instances. [![Awesome Go](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)

### Frontend

- **[NanoMD](https://nanomd.pardn.io)** — Single-pass TypeScript Markdown parser with a renderer-agnostic JSON AST. Renders a 4 MB document in about 90 ms (1.1–1.3× faster than marked), with on-demand Mermaid / KaTeX / Chart.js and sanitized HTML output.

### Production

- **[JOBALL](https://joball.tw)** — Freelance expert marketplace in Taiwan · **peak 10K users / 340K monthly views**

---

<details>

<summary><strong>More</strong></summary>

**Go / AI Agent**

- [go-browser](https://go-browser.pardn.io)
- [go-bot](https://go-bot.pardn.io)
- [KuraDB](https://kuradb.pardn.io)
- (Archive) [cim-prototype](https://github.com/pardnio/cim-prototype)

**Go / Infra**

- [PodRun](https://podrun.pardn.io)
- (Archive) [go-image-server](https://go-image-server.pardn.io)

**Go / Toolkit** (Archive)

- [go-ip-sentry](https://go-ip-sentry.pardn.io)
- [go-redis-fallback](https://go-redis-fallback.pardn.io)
- [go-web-monitor](https://go-web-monitor.pardn.io)
- [go-rss-reader](https://go-rss-reader.pardn.io)
- [go-rest-client](https://go-rest-client.pardn.io)
- [go-logger](https://github.com/pardnio/go-logger)

**Shipped apps**

- [C2hat (Chrome)](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)
- [NanoMD (VS Code)](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)
- [NanoMD (Chrome)](https://chromewebstore.google.com/detail/nanomd/pdklinlfmpobpakengplkhbbneaamijd)
- (Discontinued) [NanoMD (macOS)](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)
- (Discontinued) [Ninlog (macOS)](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)
- (Discontinued) [JOBALL (iOS)](https://apps.apple.com/us/app/joball-接洽/id1272878907)

**Frontend**

- [QuickUI](https://quickui.pardn.io)
- [NanoJSON](https://nanojson.pardn.io)
- (Archive) [FlexPlyr](https://flexplyr.pardn.io)
- (Archive) [RenderJS](https://renderjs.pardn.io)
- (Archive) [pdf2image](https://pdf2image.pardn.io)
- (Archive) [demo-web](https://demo-web.pardn.io)
- (Archive) [WebUI](https://pardnio.github.io/WebUI/)
- (Archive) [AdminUI](https://pardnio.github.io/AdminUI/)
- (Archive) [DeskUI](https://pardnio.github.io/DeskUI/)
- (Archive) [css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)
- (Archive) [SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)
- (Archive) [web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)

**Node.js** (Archive)

- [node-image-server](https://node-image-server.pardn.io)
- [node-jwt-auth](https://node-jwt-auth.pardn.io)
- [node-mysql-pool](https://node-mysql-pool.pardn.io)

**PHP** (Archive)

- [php-async](https://github.com/pardnio/php-async)
- [php-mysql-cli](https://github.com/pardnio/php-mysql-cli)
- [php-redis-cli](https://github.com/pardnio/php-redis-cli)
- [php-cache-fallback](https://github.com/pardnio/php-cache-fallback)
- [php-session-fallback](https://github.com/pardnio/php-session-fallback)
- [php-mailer](https://github.com/pardnio/php-mailer)

**iOS** (Archive)

- [ExSwift](https://github.com/pardnio/ExSwift)
- [demo-swiftui](https://github.com/pardnio/demo-swiftui)
- [demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)
- [demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)

**Infra / Shell** (Archive)

- [pdpve](https://github.com/pardnio/pdpve)

</details>
