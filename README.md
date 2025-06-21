# Only sharing my personal projects
> [!Note]
> 1. GitHub is only used for sharing independently developed projects.
> 2. Projects without a LICENSE are considered MIT by default.
> 3. Packages for different languages (such as `{golang/nodejs/php}-mysql-pool`）will align their functionality as much as possible.
> 4. Employed at ITRD, unavailable for external projects.
> 5. 臺灣地區 - 非自身公司簽約的部分僅與[**鍵深坊有限公司**](https://findbiz.nat.gov.tw/fts/query/QueryBar/queryInit.do?banNo=00248098)協同開發過一次，僅負責專案（Axonews）中的 iOS 開發<br>
>   其餘皆以自身公司[**帕登國際有限公司**](https://findbiz.nat.gov.tw/fts/query/QueryBar/queryInit.do?banNo=24924502)簽約且獨立開發，無任何外部協作。

> [!Tip]
> Repository Naming Convention
> - **PascalCase**: Independent projects and standalone applications
> - **demo-{language}-{service}**: Complete demonstration projects
> - **{language}-{service}**: Language-specific modules and packages

## Infrastructure
### Database
- Rust
  - [ ] *[JsonDB](https://github.com/pardnchiu/jsondb) - (BACKLOG) JSON Indexed with Query*
  - [ ] *[BlobDB](https://github.com/pardnchiu/blobdb) - (BACKLOG) Picture Indexed with blob Store*

<br>

## Backend
### Package
- Golang
  - [ ] **[pardnchiu/go-cron-job](https://github.com/pardnchiu/go-cron-job) - (WIP) Cron job with flexible timing expressions**
  - [ ] **[pardnchiu/go-logger](https://github.com/pardnchiu/go-logger) - (WIP) Logger with file rotation, multi-level support**
  - [x] [pardnchiu/go-redis-fallback](https://github.com/pardnchiu/go-redis-fallback) - Redis connect with automatic failover
  - [x] [pardnchiu/go-ip-sentry](https://github.com/pardnchiu/go-ip-sentry) - IP threat detection and geolocation analysis
  - [x] [pardnchiu/go-jwt-auth](https://github.com/pardnchiu/go-jwt-auth) - JWT authentication with automatic refresh
  - [x] [pardnchiu/go-mysql-pool](https://github.com/pardnchiu/go-mysql-pool) - Chainable MySQL connection wrapper
- Node.js 
  - [x] [@pardnchiu/jwt-auth](https://www.npmjs.com/package/@pardnchiu/jwt-auth) - JWT authentication package
  - [x] [@pardnchiu/mysql-pool](https://www.npmjs.com/package/@pardnchiu/mysql-pool) - Chainable MySQL connection wrapper
- PHP
  - [x] [pardnchiu/mysql-pool](https://packagist.org/packages/pardnchiu/mysql-pool) - Chainable MySQL connection pool
  - [x] [pardnchiu/async](https://packagist.org/packages/pardnchiu/async) - Asynchronous processing utility wrapper
  - [x] [pardnchiu/redis](https://packagist.org/packages/pardnchiu/redis) - Redis operation wrapper
  - [x] [pardnchiu/cache](https://packagist.org/packages/pardnchiu/cache) - Cache management system
  - [x] [pardnchiu/session](https://packagist.org/packages/pardnchiu/session) - Session management tool
### Demo
- Golang
  - [ ] **[SSO Server](https://github.com/pardnchiu/demo-golang-sso-server) - (WIP) Single sign-on server with OAuth2**
  - [x] [Image Server](https://github.com/pardnchiu/demo-golang-image-server) -  Image processing and caching server
- Node.js
  - [ ] *[E2EE Chat](https://github.com/pardnchiu/demo-nodejs-e2ee-chat) - (BACKLOG) E2E encrypted messaging*
  - [x] [Image Server](https://github.com/pardnchiu/demo-nodejs-image-server) -  Image processing and caching server
  - [ ] *[Presonal Blog](https://github.com/pardnchiu/demo-nodejs-blog) - (Refactoring) Personal Blog with markdown editor*
- PHP
  - [ ] *[Personal Blog](https://github.com/pardnchiu/demo-php-blog) - (Refactoring) Personal Blog with markdown editor*

<br>

## Frontend
### Library
- JavaScript
  - [x] [QuickUI](https://quickui.pardn.io) - Lightweight frontend framework
  - [x] [NanoMD](https://nanomd.pardn.io) - Modular Markdown Editor
  - [x] [NanoJSON](https://nanojson.pardn.io) - Modular JSON Editor
  - [x] [FlexPlyr](https://flexplyr.pardn.io) - Modular Media Player
  - [x] [RenderJS](https://renderjs.pardn.io) - Rendering extension library
  - [x] [pdf2image](https://pardn.io/pdf2image) - PDF to image converter
- Swift
  - [x] [ExSwift](https://github.com/pardnchiu/ExSwift) - Swift extension utilities
### Demo
- Web
  - [x] [DeskUI](https://github.com/pardnltd/DeskUI) - Desktop-style UI interface
  - [x] [Web Template](https://pardn.io/web-template) - up to 40 Web template collection
  - [x] [Website Builder](https://github.com/pardnltd/website-builder) - Visual website builder tool
  - [x] [AdminUI](https://github.com/pardnltd/adminui) - Admin dashboard template
  - [x] [Skill Icons Picker](https://pardnchiu.github.io/skill-icons-picker/) - Picker of Skill Icons
- iOS
  - [x] [SwiftUI Demo](https://github.com/pardnchiu/swiftui-demo) - Component showcase using SwiftUI
  - [x] [Moneybook](https://github.com/pardnchiu/ios-moneybook) - iOS expense tracking app example using Swift/UIKit
  - [x] [Firebase Messaging](https://github.com/pardnchiu/ios-firebase-messaging) - Firebase messaging app example using Swift/Uikit
### More
- [x] [Pokemon Quest](https://github.com/pardnchiu/css-pokemon-quest) - CSS Drawing

<br>

## Tools
- [x] [VIM Config](https://github.com/pardnchiu/vim-config) - VIM editor configuration

<br>

## Live / Discontinued

### Live
- Web
  - [x] [JOBALL](https://joball.tw) - Experts Matching Platform in Taiwan
- macOS
  - [x] [NanoMD](https://apps.apple.com/us/app/nanomd-markdown-%E7%B7%A8%E8%BC%AF%E5%99%A8/id6740427920) - Markdown editor
  - [x] [NinLog](https://apps.apple.com/tw/app/ninlog-%E9%8D%B5%E7%9B%A4%E6%BB%91%E9%BC%A0%E8%BF%BD%E8%B9%A4/id6741706238) - Keyboard/Mouse tracking
### Discontinued
- iOS
  - [ ] <s>[NEEDS](https://appadvice.com/app/e9-96-8b-e7-ae-b1/1460355322.amp) - Social E-commerce App with Blockchain</s>
  - [ ] <s>[JOBALL](https://appadvice.com/app/joball-e6-8e-a5-e6-b4-bd/1272878907.amp) - Experts Matching Platform App</s>

