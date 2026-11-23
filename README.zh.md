最後更新：2026-11-24

# 邱敬幃 (Pardn Chiu)

> **Show code, not just words — 代碼就是我的自介**<br>
> 從 iOS 起家，精通網站前後端，目前專注在 AI / 虛擬化基礎建設
>
> 所發布的都是過往經驗，所構思的都是新的架構
>
> 如果我所發布的對你有用，儘管拿去用<br>
> 真正有價值的是打造出來的 know-how，我留著繼續開發

---

<a href="https://agenvoy.com/"><img src="https://avatars.githubusercontent.com/u/260084267?s=200&v=4" align="left" width=96 height=96></a>

### [Agenvoy](https://agenvoy.com/)

**以單一 Go 執行檔交付、在你自己的電腦上以 daemon 24 小時運行的私人 AI agent。**<br>
用一句話描述任務，Agenvoy 就會規劃步驟、呼叫工具並交付結果；沒有合適的工具時，它會自己寫一個、在沙箱中測試，並保留下來重複使用。

<br clear="left"/>

- **自己打造工具** — 找到免金鑰的公開 API 或撰寫新工具，並與 Claude Code、Codex 及任何 MCP agent 共用同一套沙箱化工具庫
- **本地優先** — session、記憶與排程存放在你磁碟上的 SQLite；憑證留在作業系統 keychain；指令在 `sandbox-exec`／`bwrap` 中執行，預設關閉網路
- **一句話自動化** — 用自然語言建立 cron 排程，在你的電腦上執行並把結果推送到 Telegram 或 Discord，不需開放任何對內連接埠
- **任意模型** — 15 家 LLM 供應商加上本地 Ollama／LM Studio，支援依任務路由、MCP（stdio／HTTP）、生圖、語音轉文字與文字轉語音
- **看得見、管得住** — 串流 TUI 與 Web 儀表板、敏感路徑的確認關卡，以及支援喚醒詞的免手持語音模式

---

### AI

- **[go-llm-router](https://go-llm-router.pardn.io)** — 以統一的 Go 介面串接 15 家 LLM 供應商。用 `provider@model` 字串解析任何模型，把 Claude、Gemini、OpenAI 的推理強度正規化為六個等級，並將各家的 token 與快取用量整合成同一種格式。從 Agenvoy 抽離而來，Agenvoy 現已完全建立在它之上。
- **[ToriiDB](https://toriidb.pardn.io)** — 內建向量搜尋的嵌入式 Go JSON 鍵值儲存。第一個開啟資料目錄的程序會成為共用的 unix socket daemon，寫入以 fsync 落盤到追加日誌並以原子快照壓縮，在 16 個資料庫上提供 17 個 Redis 風格指令。

### 基礎設施

- **[HakoRun](https://hakorun.pardn.io)** — 不需要 Docker 或 Kubernetes 的自架 FaaS。上傳 Python、JS 或 TS 函式即可透過 HTTP 呼叫；每次執行都隔離在 Bubblewrap 中（所有 namespace 皆不共用、無網路、移除 capabilities），由 systemd slice 限制資源，並以 SSE 串流回傳，版本以時間戳固定。
- **[QemuRun-pve](https://qemurun-pve.pardn.io)** — 一次 API 呼叫，從官方雲端映像建立可 SSH 登入的 Proxmox VE 虛擬機。處理並行的 VMID／IP 配置，偵測全叢集共通的 CPU 基準讓虛擬機保持可遷移，並透過 SSH 在各節點分派 `qm`，每個建置階段都以 SSE 串流回報。

### 函式庫

- **[go-queue](https://go-queue.pardn.io)** — 以單一 min-heap 承載五個優先等級的任務佇列，具備防飢餓升級、獨立的重試層級、panic 隔離，以及有期限的優雅關閉。
- **[go-scheduler](https://go-scheduler.pardn.io)** — Cron 排程器，支援任務相依鏈（失敗時停止或略過）、各任務逾時，以及可在執行期間新增與移除任務的 min-heap 事件迴圈。 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)
- **[go-jwt](https://go-jwt.pardn.io)** — ES256 JWT，透過 Redis JTI 白名單即時撤銷、綁定裝置指紋，並以鎖保護的 refresh 輪替確保跨實例安全。 [![Awesome Go 收錄](https://awesome.re/mentioned-badge.svg)](https://github.com/avelino/awesome-go)

### 前端

- **[NanoMD](https://nanomd.pardn.io)** — 單次掃描的 TypeScript Markdown 解析器，輸出與渲染器無關的 JSON AST。約 90 ms 渲染 4 MB 文件（比 marked 快 1.1–1.3 倍），按需載入 Mermaid／KaTeX／Chart.js，並輸出經過消毒的 HTML。

### 產品

- **[JOBALL](https://joball.tw)** — 台灣自由工作者媒合平台 · **高峰 1 萬名使用者／月瀏覽 34 萬**

---

<details>

<summary><strong>更多</strong></summary>

**Go／AI Agent**

- [go-browser](https://go-browser.pardn.io)
- [go-bot](https://go-bot.pardn.io)
- [KuraDB](https://kuradb.pardn.io)
- （封存）[cim-prototype](https://github.com/pardnio/cim-prototype)

**Go／基礎設施**

- [PodRun](https://podrun.pardn.io)
- （封存）[go-image-server](https://go-image-server.pardn.io)

**Go／工具組**

- （封存）[go-ip-sentry](https://go-ip-sentry.pardn.io)
- （封存）[go-redis-fallback](https://go-redis-fallback.pardn.io)
- （封存）[go-web-monitor](https://go-web-monitor.pardn.io)
- （封存）[go-rss-reader](https://go-rss-reader.pardn.io)
- （封存）[go-rest-client](https://go-rest-client.pardn.io)
- （封存）[go-logger](https://github.com/pardnio/go-logger)

**已上架應用**

- [C2hat（Chrome）](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn)
- [NanoMD（VS Code）](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd)
- [NanoMD（Chrome）](https://chromewebstore.google.com/detail/nanomd/pdklinlfmpobpakengplkhbbneaamijd)
- （已停止維護）[NanoMD（macOS）](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920)
- （已停止維護）[Ninlog（macOS）](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238)
- （已停止維護）[JOBALL（iOS）](https://apps.apple.com/us/app/joball-接洽/id1272878907)

**前端**

- [QuickUI](https://quickui.pardn.io)
- [NanoJSON](https://nanojson.pardn.io)
- （封存）[FlexPlyr](https://flexplyr.pardn.io)
- （封存）[RenderJS](https://renderjs.pardn.io)
- （封存）[pdf2image](https://pdf2image.pardn.io)
- （封存）[demo-web](https://demo-web.pardn.io)
- （封存）[WebUI](https://pardnio.github.io/WebUI/)
- （封存）[AdminUI](https://pardnio.github.io/AdminUI/)
- （封存）[DeskUI](https://pardnio.github.io/DeskUI/)
- （封存）[css-pokemon-quest](https://pardnio.github.io/css-pokemon-quest/)
- （封存）[SkilliconsPicker](https://pardnio.github.io/SkilliconsPicker/)
- （封存）[web-admin-20220917](https://pardnio.github.io/web-admin-20220917/)

**Node.js**

- （封存）[node-image-server](https://node-image-server.pardn.io)
- （封存）[node-jwt-auth](https://node-jwt-auth.pardn.io)
- （封存）[node-mysql-pool](https://node-mysql-pool.pardn.io)

**PHP**

- （封存）[php-async](https://github.com/pardnio/php-async)
- （封存）[php-mysql-cli](https://github.com/pardnio/php-mysql-cli)
- （封存）[php-redis-cli](https://github.com/pardnio/php-redis-cli)
- （封存）[php-cache-fallback](https://github.com/pardnio/php-cache-fallback)
- （封存）[php-session-fallback](https://github.com/pardnio/php-session-fallback)
- （封存）[php-mailer](https://github.com/pardnio/php-mailer)

**iOS**

- （封存）[ExSwift](https://github.com/pardnio/ExSwift)
- （封存）[demo-swiftui](https://github.com/pardnio/demo-swiftui)
- （封存）[demo-swift-firebase-messaging](https://github.com/pardnio/demo-swift-firebase-messaging)
- （封存）[demo-swift-moneybook](https://github.com/pardnio/demo-swift-moneybook)

**Infra／Shell**

- （封存）[pdpve](https://github.com/pardnio/pdpve)

</details>
