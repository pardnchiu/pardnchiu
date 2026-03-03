# README

> [!Note]
> 1. Sharing only my independently developed projects.
> 2. My code is my pitch — if it doesn't resonate, no worries.
> 3. Employed at ITRD, unavailable for external projects.

---

## WIP
- [go-kvmesh](https://github.com/pardnchiu/go-kvmesh) — Debian-based virtualization platform with cluster management
- [go-qemu](https://github.com/pardnchiu/go-qemu) — Library offering VM operations built on native QEMU and Cloud-Init

---

## Backend

### Go

#### Services
| Description | Link |
| - | - |
| A Go-based agentic AI platform with intent-to-skill routing, multi-provider LLM dispatch, cross-turn memory, and zero-code REST API tool mounting.<br>![license](https://img.shields.io/github/license/pardnchiu/agenvoy)  | [Agenvoy](https://github.com/pardnchiu/agenvoy) |
| A terminal-based REST API testing tool compatible with VSCode REST Client extension's .http file format. Execute HTTP requests through an intuitive TUI interface and display responses in real-time. | [go-rest-client](https://github.com/pardnchiu/go-rest-client) |
| A unified multi-channel notification hub that delivers messages to Discord, Slack, LINE, and Email through a single REST API. | [go-notify-hub](https://github.com/pardnchiu/go-notify-hub) |
| A CLI tool that syncs local projects to remote servers via rsync/SSH and runs Podman Compose workloads — with a local SQLite deployment registry for container lifecycle tracking.<br>![license](https://img.shields.io/github/license/pardnchiu/go-podrun) | [go-podrun](https://github.com/pardnchiu/go-podrun) |
| A Proxmox VE VM automation REST API built in Go — full lifecycle provisioning via SSE, concurrent IP & CPU architecture auto-allocation, and transparent multi-node cluster routing.<br>![license](https://img.shields.io/github/license/pardnchiu/go-pve-qemu) | [go-pve-qemu](https://github.com/pardnchiu/go-pve-qemu) |
| A lightweight Function-as-a-Service platform that accepts code via HTTP API and executes it securely inside a Bubblewrap sandbox.<br>![license](https://img.shields.io/github/license/pardnchiu/go-faas) | [go-faas](https://github.com/pardnchiu/go-faas) |
| A JSON database system example that combines Redis-style key-value operations and MongoDB-style document query functionality | [JsonDB](https://github.com/pardnchiu/JsonDB) |
| A website monitoring tool offering real-time status checks, SSL certificate monitoring, and email notifications. Includes a TUI interface for convenient status management. | [go-web-monitor](https://github.com/pardnchiu/web-monitor) |
| A terminal-based RSS news aggregator with multi-source support, content extraction, local storage, and intelligent overview features. | [go-rss-reader](https://github.com/pardnchiu/rss-reader) |
| A Go image caching server with on-the-fly processing (resize, blur, format conversion) and multi-layer caching via Nginx + Cloudflare CDN. |  [go-image-server](https://github.com/pardnchiu/demo-go-image-server) |

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

---

## Frontend

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

---

## Production

### Website
- [JOBALL](https://joball.tw) — Expert matching platform in Taiwan

### macOS
- [NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920) — Markdown editor
- [Ninlog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238) — Keyboard and mouse activity tracker

### Chrome Extension
- [C2hat](https://chromewebstore.google.com/detail/c2hat-cross-domain-chat/chngimmfgmkpninihhljpidnieocmhdn) — Cross-domain chat extension

### VSCode Extension
- [NanoMD](https://marketplace.visualstudio.com/items?itemName=pardnchiu.nanomd) — Markdown editor

---

## Discontinued

### iOS
- [JOBALL](https://apps.apple.com/us/app/joball-接洽/id1272878907) — Expert matching platform (Discontinued)
