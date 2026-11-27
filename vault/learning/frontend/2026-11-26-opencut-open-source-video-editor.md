---
title: OpenCut：開源跨平台影片編輯器
published: null
collected: 2026-11-26
platform: github
author: OpenCut-app
source: https://github.com/OpenCut-app/OpenCut
tags: [前端開發, 開源專案, 影片編輯器, Rust, 跨平台]
---

# OpenCut：開源跨平台影片編輯器

## 摘要

OpenCut 是一款免費開源的 CapCut 替代方案，目標支援網頁、桌面與行動裝置。GitHub 主專案 README 表示目前正在從頭改寫；截至 2026-11-26，README 建議想使用現有版本的讀者前往 [OpenCut Classic](https://github.com/opencut-app/opencut-classic)。[GitHub 專案](https://github.com/OpenCut-app/OpenCut)

## 專案與資源

- [OpenCut GitHub](https://github.com/OpenCut-app/OpenCut)
- [OpenCut Classic（README 指向的現有版本）](https://github.com/opencut-app/opencut-classic)
- [OpenCut 官網](https://opencut.app)
- [新版改寫預覽](https://new.opencut.app)

## 重點

- **定位**：開源影片編輯器，目標支援瀏覽器、桌面與手機。
- **改寫方向**：README 規劃以 Rust 核心支援多平台，並加入 Editor API、第三方外掛、MCP server、headless 批次渲染與編輯器內腳本頁籤。這些是規劃中的功能，不代表目前都已完成。
- **目前可用版本**：README 指出 Classic 是現階段可使用的舊版；官網仍執行 Classic，新版改寫在準備接手前使用 `new.opencut.app`。
- **開發方式**：專案以 `proto` 固定工具版本，並透過 Moon 執行工作；README 列出 `moon run web:dev`、`moon run api:dev`、`moon run desktop:dev` 等開發命令。
- **貢獻狀態**：README 表示新版架構仍在設計，目前尚未準備好接受外部程式碼貢獻。
- **授權**：MIT。

以上狀態依收集當日的 README 記錄；專案改寫進度與可用版本可能變動，使用前請查看最新文件。
