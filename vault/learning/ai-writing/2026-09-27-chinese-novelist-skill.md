---
title: Chinese Novelist Skill：AI 中文長篇小說創作工具
published: 2026-09-27
collected: 2026-11-26
platform: threads
author: aigeeknews
source: https://www.threads.com/@aigeeknews/post/Ddx4LwNCc0r
tags: [AI寫作, 中文小說, AI Skill, Agent, MIT]
---

# Chinese Novelist Skill：AI 中文長篇小說創作工具

## 摘要

@aigeeknews 分享開源專案 [chinese-novelist-skill](https://github.com/PenglongHuang/chinese-novelist-skill)，讓 AI Agent 協助從構思與大綱開始，逐章創作 10–50 章的中文長篇小說。[Threads 原貼文](https://www.threads.com/@aigeeknews/post/Ddx4LwNCc0r)

貼文介紹 2.0 版的三層遞進式問答、偏好記憶、中斷續寫，以及自動校驗與修復，目標是改善長篇創作的連貫性。

## 功能與使用方式

- **創作流程：**先透過問答確認題材、人物與故事方向，再產生大綱及寫作計畫，接著逐章寫作、檢查與修訂。
- **寫作模式：**README 列出串行、子 Agent 並行及 Agent Teams 等模式。
- **創作記憶：**保存使用者的題材、視角與文風偏好，供後續創作參考。
- **續寫與檢查：**可偵測中斷進度並續寫；以章節摘要、連貫性檢查及字數檢查協助校驗與修復。自動檢查不等同於保證作品品質。
- **作品瀏覽：**提供本機唯讀小說書房，瀏覽章節進度、正文與創作資料。
- **安裝：**README 提供 `npx skills add PenglongHuang/chinese-novelist-skill`，並列出 Claude Code、Codex CLI、Gemini CLI、Cursor 等 Agent Harness。
- **授權與費用：**專案採 MIT 授權；使用時仍需可用的 Agent 與模型，模型費用依所選服務而定。README 中的 Infistar.cc 贊助與註冊優惠並非使用 Skill 的必要條件。

## 版本與注意事項

- Threads 貼文介紹的是 v2.0；截至 2026-11-26，GitHub README 標示版本為 v2.4.0，請以[專案最新文件](https://github.com/PenglongHuang/chinese-novelist-skill)為準。
- 長篇一致性檢查與修復是 AI 輔助流程，仍宜自行審讀人物、情節與細節。

## 貼文媒體與回覆

- 主貼文附 GitHub 專案連結預覽卡，沒有獨立圖片或影片；預覽縮圖不另存為貼文附件。
- 可見頁面未顯示作者補充回覆或其他實質留言。
