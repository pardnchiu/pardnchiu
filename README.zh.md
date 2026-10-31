最後更新：2026-11-01

# 邱敬幃 Pardn Chiu

> **Show code, not just words——代碼就是我的自介**<br>
> 台灣 · 基礎設施工程<br>
> 從 iOS 起家，精通網站前後端，目前專注在基礎建設
>
> 我的 GitHub 專注於基礎設施與基礎元件<br>
> 核心功能優先，少臃腫、少花俏<br>
> 身為開發者的你，歡迎善加使用這裡的每個工具

**項目需知**

1. 測試檔案與 SKILL repo（含 Python 腳本）皆由 LLM 生成，我只檢查 I/O
2. pardnio 存放封存的 repo，pardnchiu 維護模組與函式庫

---

<a href="https://agenvoy.com/"><img src="https://avatars.githubusercontent.com/u/260084267?s=200&v=4" align="left" width=96 height=96></a>

### [Agenvoy](https://agenvoy.com/)

讓 AI 真正替你做事<br>
以 Go 打造、24 小時運行的本地 AI agent harness，具備自動建工具、MCP 與 Ollama 支援

---

### 後端

<details open>

<summary>Go／AI Agent（6）</summary>

- **[go-llm-router](https://go-llm-router.pardn.io)** — 一個 Agent 介面，串接所有 LLM 供應商
- **[go-browser](https://go-browser.pardn.io)** — 透過 Chrome 擷取網頁內容，輸出 Markdown 或 HTML，直接供 agent 使用
- **[go-bot](https://go-bot.pardn.io)** — 打造適配各聊天平台的機器人
- **[ToriiDB](https://toriidb.pardn.io)** — 內嵌式 JSON KV 儲存，共享 socket daemon 與向量搜尋
- **[KuraDB](https://kuradb.pardn.io)** — 放入檔案，讓你的 agent 幫你搜出來
- （封存）[cim-prototype](https://github.com/pardnio/cim-prototype)

</details>

<details open>

<summary>Go／自架基礎設施（4）</summary>

- **[HakoRun](https://hakorun.pardn.io)** — 自架 FaaS，不需要 Docker 或 Kubernetes
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — 一次 API 呼叫，從雲端映像到可 SSH 登入的 Proxmox VE 虛擬機
- **[PodRun](https://podrun.pardn.io)** — 像在本地執行 docker compose 一樣部署到遠端 Podman 與 k3s
- （封存）[go-image-server](https://go-image-server.pardn.io)

</details>

<details open>

<summary>Go／後端工具組（9）</summary>

- **[go-queue](https://go-queue.pardn.io)** — 永不飢餓的優先度任務佇列
- **[go-scheduler](https://go-scheduler.pardn.io)** — 排程任務，支援相依、逾時與 cron 表達式 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-jwt](https://go-jwt.pardn.io)** — ECDSA JWT，含 Redis 生命週期與裝置綁定 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- （封存）[go-ip-sentry](https://go-ip-sentry.pardn.io)、[go-redis-fallback](https://go-redis-fallback.pardn.io)、[go-web-monitor](https://go-web-monitor.pardn.io)、[go-rss-reader](https://go-rss-reader.pardn.io)、[go-rest-client](https://go-rest-client.pardn.io)、[go-logger](https://github.com/pardnio/go-logger)

</details>

**Node.js（3）**（封存）[node-image-server](https://node-image-server.pardn.io)、[node-jwt-auth](https://node-jwt-auth.pardn.io)、[node-mysql-pool](https://node-mysql-pool.pardn.io)

**PHP（6）**（封存）[php-async](https://github.com/pardnio/php-async)、[php-mysql-cli](https://github.com/pardnio/php-mysql-cli)、[php-redis-cli](https://github.com/pardnio/php-redis-cli)、[php-cache-fallback](https://github.com/pardnio/php-cache-fallback)、[php-session-fallback](https://github.com/pardnio/php-session-fallback)、[php-mailer](https://github.com/pardnio/php-mailer)

**Infra／Shell（1）**（封存）[pdpve](https://github.com/pardnio/pdpve)

---

### 前端

<details open>

<summary>框架／函式庫（6）</summary>

- **[QuickUI](https://quickui.pardn.io)** — 零相依、免建置即可執行的虛擬 DOM 框架
- **[NanoMD](https://nanomd.pardn.io)** — 單一解析器，快速將 Markdown 轉為 AST 與 HTML
- **[NanoJSON](https://nanojson.pardn.io)** — 純 JavaScript 打造的輕量視覺化 JSON 編輯器
- （封存）[FlexPlyr](https://flexplyr.pardn.io)、[RenderJS](https://renderjs.pardn.io)、[pdf2image](https://pdf2image.pardn.io)

</details>

**Demo／網頁（7）**（封存）[demo-web](https://demo-web.pardn.io)、[WebUI](https://pardnio.github.io/WebUI/)、[AdminUI](https://pardnio.github.io/AdminUI/)、[DeskUI](https://pardnio.github.io/DeskUI/)、[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)、[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)、[web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)

**iOS（4）**（封存）[ExSwift](https://github.com/pardnio/ExSwift)、[demo-swiftui](https://github.com/pardnio/demo-swiftui)、[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)、[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)

---

### 產品

<details open>

<summary>已上線（7）</summary>

- **[JOBALL（網頁）](https://joball.tw)** — 台灣自由工作者媒合平台 · **高峰 1 萬名使用者／月瀏覽 34 萬**
- **[C2hat（Chrome 擴充功能）](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — 端對端加密的跨網域聊天擴充，訊息不留存於伺服器
- **[NanoMD（VS Code 擴充功能）](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown 編輯器，分割畫面預覽與 Mermaid 支援
- **[NanoMD（Chrome 擴充功能）](https://chromewebstore.google.com/detail/nanomd/pdklinlfmpobpakengplkhbbneaamijd)** — 直接在 Chrome 中渲染 Markdown 檔案
- （已停止維護）**[NanoMD（macOS）](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** ・ **[Ninlog（macOS）](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** ・ **[JOBALL（iOS）](https://apps.apple.com/us/app/joball-接洽/id1272878907)**

</details>
