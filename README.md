# README
> [!Note]
> 1. Only sharing my independently developed projects.
> 2. Projects without a LICENSE are considered MIT by default.
> 3. If these are not enough and you need more to assess my ability, then it means I’m not the one you need.
> 4. Employed at ITRD, unavailable for external projects.

## Backend
- Infrastructure & Virtualization
  - (wip) [go-kvmesh](https://github.com/pardnchiu/go-kvmesh): Debian-based virtualization platform with cluster management
  - (wip) [go-k8s](https://github.com/pardnchiu/go-k8s): K8s deployment with Docker Compose translation
  - [go-faas](https://github.com/pardnchiu/go-faas): Serverless function runtime
  - [go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu): PVE qm-based API with Cloud-Init auto-provisioning
- Database
  - [JsonDB](https://github.com/pardnchiu/JsonDB): JSON database with queries and caching
- Service
  - [web-monitor](https://github.com/pardnchiu/web-monitor): Website monitor with Email notification
  - [rss-reader](https://github.com/pardnchiu/rss-reader): RSS reader with LLM summarization
  - [cim-prototype](https://github.com/pardnchiu/cim-prototype): LLM with Cognitive Imperfect Memory system
  - [go-image-server](https://github.com/pardnchiu/demo-go-image-server): Image upload and caching server
  - [node-image-server](https://github.com/pardnchiu/demo-node-image-server): Image upload and caching server
- Package
  - Virtualization
    - [go-qemu](https://github.com/pardnchiu/go-qemu): QEMU management with Cloud-Init auto-provisioning
  - Database Client
    - [go-pg](https://github.com/pardnchiu/go-pg): PostgreSQL client with chained method calls
    - [go-mysql](https://github.com/pardnchiu/go-mysql): MySQL client with chained method calls
    - [node-mysql-pool](https://github.com/pardnchiu/node-mysql-pool): MySQL client with chained method calls
    - [php-mysql-cli](https://github.com/pardnchiu/php-mysql-cli): PDO wrapper for MySQL with chained method calls
  - Cache & Session
    - [go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback): Redis client with graceful fallback
    - [php-redis-cli](https://github.com/pardnchiu/php-redis-cli): Redis client wrapper
    - [php-cache-fallback](https://github.com/pardnchiu/php-cache-fallback): Cache manager with graceful fallback
    - [php-session-fallback](https://github.com/pardnchiu/php-session-fallback): Session manager with graceful fallback
  - Authentication & Security
    - [go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry): IP threat detection with automatic blacklisting
    - [go-jwt](https://github.com/pardnchiu/go-jwt): JWT authentication with auto-renewal
    - [node-jwt-auth](https://github.com/pardnchiu/node-jwt-auth): JWT system with auto-renewal
  - Utilities
    - [go-scheduler](https://github.com/pardnchiu/go-scheduler): Task scheduler with standard cron expressions
    - [go-logger](https://github.com/pardnchiu/go-logger): Logging client with automatic rotation
    - [php-mailer](https://github.com/pardnchiu/php-mailer): PHPMailer wrapper
    - [php-async](https://github.com/pardnchiu/php-async): Async task dependency manager
- Script
  - [pdpve](https://github.com/pardnchiu/pdpve): Proxmox VE scripts
- Worker (Cloudflare)
  - [c2hat-relay](https://github.com/pardnchiu/c2hat-relay): WebSocket relay for E2EE messaging

## Frontend

- Library
  - JavaScript / TypeScript
    - [QuickUI](https://quickui.pardn.io): Lightweight frontend framework
    - [NanoMD](https://nanomd.pardn.io): Markdown editor with real-time preview
    - [NanoJSON](https://nanojson.pardn.io): Firebase-like JSON editor
    - [FlexPlyr](https://flexplyr.pardn.io): Media player with multiple styles
    - [RenderJS](https://renderjs.pardn.io): DOM rendering library
    - [pdf2image](https://pdf2image.pardn.io/): PDF-to-image converter
  - Swift
    - [ExSwift](https://github.com/pardnchiu/ExSwift): Swift extension utilities
- Demo
  - Website
    - [demo-web](https://github.com/pardnchiu/demo-web): Explore over 30 frontend examples
    - [DeskUI](https://github.com/pardnltd/DeskUI): Desktop-style web UI
    - [WebUI](https://webui.pardn.io): Visual website builder
    - [AdminUI](https://adminui.pardn.io): Admin dashboard template
  - iOS
    - [demo-swiftui](https://github.com/pardnchiu/demo-swiftui): Demo with SwiftUI
    - [demo-swift-firebase-messaging](https://github.com/pardnchiu/demo-swift-firebase-messaging): Messaging demo with Firebase and UIKit
    - [demo-swift-moneybook](https://github.com/pardnchiu/demo-swift-moneybook): Moneybook UI demo with UIKit

## Live / Discontinued
- Website
  - [JOBALL](https://joball.tw): Expert matching platform in Taiwan
- macOS
  - [NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920): Markdown editor
  - [Ninlog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238): Keyboard and mouse activity tracker
- iOS
  - <s>[JOBALL](https://appadvice.com/app/joball-e6-8e-a5-e6-b4-bd/1272878907.amp): Expert matching platform (Discontinued)</s>
- Chrome Extension
  - [C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn): Cross-domain chat extension
