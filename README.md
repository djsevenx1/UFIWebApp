# UFI Web

Android WebView 客户端，用于访问 UFI-TOOLS 设备管理界面 `http://192.168.43.1:2333`。

## 简介

基于 [djsevenx1/claude-code-mobile](https://github.com/djsevenx1/claude-code-mobile) 改造：

- 包名 `com.ufi.webapp`（原 `com.claudecode.mobile`）
- 移除 token 登录强制（UFI-TOOLS 局域网无鉴权）
- 默认地址预填 `http://192.168.43.1:2333`
- 启动后直接进入 WebView

## 下载

在 [Releases](../../releases) 页面下载最新 `UFIWebApp-v*-release.apk`。

## 包信息

- `applicationId` / `namespace`: `com.ufi.webapp`
- `minSdk`: 26
- `targetSdk`: 34
- `versionName`: 跟随 claude-code-mobile 上游版本

## 项目结构

- `app/src/main/java/com/ufi/webapp/ui/MainActivity.kt` — 主入口 WebView
- `.github/workflows/build.yml` — CI: tag → 编译签名 → 发布
