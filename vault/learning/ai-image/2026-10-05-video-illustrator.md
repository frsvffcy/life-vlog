---
title: Video Illustrator：把旁白與素材變成宣傳片的開源 Agent Skill
published: 2026-10-05
platform: threads
author: effusioncreatives
source: https://www.threads.com/@effusioncreatives/post/DeI74I1E6je
tags: [AI產圖, Agent Skill, 影片生成, Video Illustrator, 開源]
---

# Video Illustrator：把旁白與素材變成宣傳片的開源 Agent Skill

effusioncreatives 分享一個免費開源的 Agent Skill「Video Illustrator」，主張不需高價委外製作形象宣傳片。使用者可用自己的旁白加上真實素材（書封、Logo、截圖原封不動），做成 20 到 60 秒的宣傳片或概念說明片，可選剪紙、水墨、像素風等風格，並在自己的電腦上渲染出 MP4。MIT 授權，不收費。[Threads 原貼文](https://www.threads.com/@effusioncreatives/post/DeI74I1E6je)

## 工具與資源

- Video Illustrator GitHub Repository：https://github.com/axtonliu/video-illustrator
- 作者：Axton Liu（axtonliu）
- 授權：程式碼與文件為 MIT；展示影片、預覽及其中素材不因此獲授權重用，請參閱專案說明。

## 作者示範圖

尚未確認主貼文是否有圖片或輪播；登入提示阻擋了完整檢查。目前未保存圖片，也未將回文或連結卡片圖片當成主貼文附件。

## 提示詞重點

- **核心概念**：用旁白 + 真實素材 + 指定風格，產出 20–60 秒宣傳片或概念說明片
- **素材處理**：書封、Logo、截圖原封不動，僅縮放、移動、裁切或打光
- **可選風格**：Editorial tech、Cinematic 3D、Cut paper（剪紙）、Ink wash（水墨）、Pixel retro（像素）、Particles（粒子）
- **輸出格式**：MP4 + 可編輯 `scene.html` + `brief.md`（記錄音樂、節拍、素材選擇）
- **渲染方式**：本機執行，不上傳至託管服務；3D 路線使用 three.js
- **安裝需求**：Node.js 20+、FFmpeg/ffprobe、Playwright Chromium
- **設計對象**：Claude Code + Opus 5.5（其他宿主未驗證）
- **音樂與費用**：可自備音樂；專案說明的選用 Lyria 音樂生成需授權且可能收費，編碼代理的模型使用也可能產生費用。

## 自己試作時

1. **安裝環境**：確認 Node.js 20+、FFmpeg/ffprobe 已安裝，並執行 `npm ci` 與 `npx playwright install chromium`。
2. **準備素材**：將旁白放入 `inputs/voice/`，書封/Logo/截圖放入 `inputs/assets/`，品牌資訊放入 `inputs/brand/`。
3. **下指令**：用一句話指定風格與輸出規格，例如「用 video-illustrator 將 ./my-promo 做成剪紙風格的 1920×1080 宣傳片，配上字幕，對齊旁白」。
4. **檢查輸出**：取得 MP4 與 `scene.html`，確認素材未被更動、風格與旁白節奏正確。

## 示範影片

專案 README 收錄各風格的[示範影片連結](https://github.com/axtonliu/video-illustrator#one-narration-six-looks)；影片不下載至保存庫。
