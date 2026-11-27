---
title: 用 Claude 製作互動作品集網頁
published: 2026-10-08
collected: 2026-11-20
platform: threads
author: pound0423
source: https://www.threads.com/@pound0423/post/DePMmXgCdya
tags: [前端開發, 作品集, Three.js, AI輔助開發]
---

# 用 Claude 製作互動作品集網頁

## 摘要

@pound0423 分享用 Claude 製作互動作品集網站的提示詞：首頁播放影片，作品頁透過 Three.js 著色器在靜態圖與影片之間轉換。[Threads 原貼文](https://www.threads.com/@pound0423/post/DePMmXgCdya)

作者在[回覆](https://www.threads.com/@pound0423/post/DeQkcGLmQgy)中補充：影片要先生成好，再交給 Claude；提示詞用於製作網頁介面，而非生成影片。

## 內文或摘錄

主貼文提到「Claude Opus 5.5 製作作品集教學」，並分享美式風格作品集、首頁影片及作品展示的構想。

### 作者原始提示詞

[Threads 作者提示詞回覆](https://www.threads.com/@pound0423/post/DePNCeomT5H)

```text
你是一位資深的 WebGL / Three.js 互動前端工程師與創意技術指導。
請用我上傳的素材製作一個作品集網頁：

【首頁】
- 全螢幕循環播放 hero.mp4（靜音自動播放，右下角可開聲音）
- 影片用 Three.js 著色器渲染，加上跟隨滑鼠的互動效果
- 中央大標題 + 一個「進入作品集」按鈕
- 按下後用全螢幕著色器轉場進入作品頁（往下捲動也能進入）

【作品頁】
- 每件作品先顯示靜態原畫（w1.jpg）
- 點一下，從點擊位置開始用著色器轉場變成動態影片（w1.mp4）
- 再點一下回到靜態
- 每件作品有標題、一句簡介、規格（解析度 / 秒數 / fps）、放大觀看按鈕
- 第一件作品放大橫跨整排，其餘兩兩一排

【技術要求】
- Three.js 用 cdnjs 的 r128 版本
- 不支援 WebGL 時，退回一般的圓形展開轉場
- 手機版改為單欄
- 支援鍵盤操作與 prefers-reduced-motion

【風格】
好萊塢史詩奇幻預告片風格：黑底、寬銀幕黑邊、Cinzel 字體、
底片顆粒、變形鏡頭光斑、底片燒穿轉場。
```

### 自己試作時

1. 準備首頁影片、作品圖片和對應影片，確認素材使用權限。
2. 提供素材與提示詞給 Claude，依作品內容調整版面和風格。
3. 測試手機、鍵盤操作、減少動態效果及 WebGL 不支援時的備援；確認使用的 Three.js 版本適合專案。

## 影片

主貼文有一段[作品集示範影片](https://www.threads.com/@pound0423/post/DePMmXgCdya)，僅保留連結，不下載影片。

作者可見回覆包含提示詞與補充文字，未見獨立圖片或影片。頁面提示登入才能查看更多回覆，無法確認是否還有其他補充。
