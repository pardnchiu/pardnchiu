最後更新：2026-10-25

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
- **[cim-prototype](https://github.com/pardnchiu/cim-prototype)** — 具備認知不完美記憶系統的 LLM，模擬人類選擇性記憶以應對長時間多輪對話

</details>

<details open>

<summary>Go／自架基礎設施（4）</summary>

- **[HakoRun](https://hakorun.pardn.io)** — 自架 FaaS，不需要 Docker 或 Kubernetes
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — 一次 API 呼叫，從雲端映像到可 SSH 登入的 Proxmox VE 虛擬機
- **[PodRun](https://podrun.pardn.io)** — 像在本地執行 docker compose 一樣部署到遠端 Podman 與 k3s
- **[go-image-server](https://go-image-server.pardn.io)** — 縮圖一次，處處快取

</details>

<details open>

<summary>Go／後端工具組（6）</summary>

- **[go-queue](https://go-queue.pardn.io)** — 永不飢餓的優先度任務佇列
- **[go-ip-sentry](https://go-ip-sentry.pardn.io)** — 在惡意 IP 抵達 handler 之前攔下
- **[go-scheduler](https://go-scheduler.pardn.io)** — 排程任務，支援相依、逾時與 cron 表達式 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-jwt](https://go-jwt.pardn.io)** — ECDSA JWT，含 Redis 生命週期與裝置綁定 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-redis-fallback](https://go-redis-fallback.pardn.io)** — Redis 掛了也能繼續讀取（ToriiDB 前身的 KV 本地儲存實作）
- （其他）[go-logger](https://github.com/pardnio/go-logger)

</details>

<details open>

<summary>Node.js（3）</summary>

- **[node-image-server](https://node-image-server.pardn.io)** — 縮圖一次，處處從快取供應（早期 Node.js 實作，後續以 Go 延續為 go-image-server）
- **[node-jwt-auth](https://node-jwt-auth.pardn.io)** — 綁定每台裝置的雙 token JWT 認證（早期 Node.js 實作，後續以 Go 延續為 go-jwt）
- **[node-mysql-pool](https://node-mysql-pool.pardn.io)** — 以鏈式查詢串接讀寫連線池

</details>

<details open>

<summary>PHP（6）</summary>

- **[php-async](https://github.com/pardnio/php-async)** — 宣告好相依，交給 Promise 去跑
- **[php-mysql-cli](https://github.com/pardnio/php-mysql-cli)** — 串起查詢，而不是串字串（早期 PHP 實作，後續以 Node.js 延續為 node-mysql-pool）
- （其他）[php-redis-cli](https://github.com/pardnio/php-redis-cli)、[php-cache-fallback](https://github.com/pardnio/php-cache-fallback)、[php-session-fallback](https://github.com/pardnio/php-session-fallback)、[php-mailer](https://github.com/pardnio/php-mailer)

</details>

<details open>

<summary>Infra／Shell（1）</summary>

- [pdpve](https://github.com/pardnio/pdpve)（早期 Shell 實作，後續以 Go 延續為 QemuRun-pve）

</details>

---

### 前端

<details open>

<summary>框架／函式庫（6）</summary>

- **[QuickUI](https://quickui.pardn.io)** — 零相依、免建置即可執行的虛擬 DOM 框架
- **[NanoMD](https://nanomd.pardn.io)** — 單一解析器，快速將 Markdown 轉為 AST 與 HTML
- **[NanoJSON](https://nanojson.pardn.io)** — 純 JavaScript 打造的輕量視覺化 JSON 編輯器
- **[FlexPlyr](https://flexplyr.pardn.io)** — 一套播放器 API，支援 HTML5、YouTube 與 Vimeo
- **[RenderJS](https://renderjs.pardn.io)** — 擴充原生 JS 原型，免額外負擔地渲染
- **[pdf2image](https://pdf2image.pardn.io)** — 在瀏覽器中直接把任何 PDF 轉成圖片

</details>

<details open>

<summary>Demo／網頁（7）</summary>

- **[demo-web](https://demo-web.pardn.io)** — 38 個手工前端頁面，零建置步驟
- **[WebUI](https://pardnio.github.io/WebUI/)** — 挑個版型、點擊編輯，頁面直接上線
- （其他）[AdminUI](https://pardnio.github.io/AdminUI/)、[DeskUI](https://pardnio.github.io/DeskUI/)、[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)、[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)、[web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)

</details>

<details open>

<summary>iOS（4）</summary>

- **[ExSwift](https://github.com/pardnio/ExSwift)** — 宣告式 UIKit 擴充，鏈式語法
- **[demo-swiftui](https://github.com/pardnio/demo-swiftui)** — SwiftUI 元件，重現 Pinterest 風格動態介面
- **[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)** — Firebase 聊天應用，QR 加好友、純程式碼 UIKit
- **[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)** — 用鏈式語法打造一整套 UIKit 記帳 App

</details>

---

### 產品

<details open>

<summary>已上線（6）</summary>

- **[JOBALL（網頁）](https://joball.tw)** — 台灣自由工作者媒合平台 · **高峰 1 萬名使用者／月瀏覽 34 萬**
- **[C2hat（Chrome 擴充功能）](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)** — 端對端加密的跨網域聊天擴充，訊息不留存於伺服器
- **[NanoMD（VS Code 擴充功能）](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)** — Markdown 編輯器，分割畫面預覽與 Mermaid 支援
- （已停止維護）**[NanoMD（macOS）](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)** ・ **[Ninlog（macOS）](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)** ・ **[JOBALL（iOS）](https://apps.apple.com/us/app/joball-接洽/id1272878907)**

</details>
