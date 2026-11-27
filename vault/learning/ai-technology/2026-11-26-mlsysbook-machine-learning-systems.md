---
title: Machine Learning Systems：機器學習系統工程教材
published: null
collected: 2026-11-26
platform: github
author: Harvard Edge
source: https://github.com/harvard-edge/cs249r_book/blob/dev/README/README_zh.md
tags: [AI技術, 機器學習系統, AI工程, TinyTorch, 邊緣AI, 教材]
---

# Machine Learning Systems：機器學習系統工程教材

## 摘要

[Machine Learning Systems](https://mlsysbook.ai) 是一套介紹 AI 系統工程原理與實務的教材及開放學習資源。內容將機器學習模型與支撐其訓練、推論及部署的系統連結，涵蓋效能、硬體、MLOps、隱私、穩健性與可信 AI。[GitHub 中文 README](https://github.com/harvard-edge/cs249r_book/blob/dev/README/README_zh.md)

## 學習路徑

- **READ｜閱讀教材：**建立機器學習系統概念，README 建議從第一章與 Benchmarking 章節開始。
- **BUILD｜動手實作：**透過 [TinyTorch](https://mlsysbook.ai/tinytorch/) 從零實作機器學習框架，逐步接觸 CNN、Transformer 與 MLPerf 基準。
- **DEPLOY｜硬體部署：**使用 [Hardware Kits](https://mlsysbook.ai/kits) 在 Arduino、Raspberry Pi 等邊緣裝置上，實際面對記憶體、功耗、延遲與安全限制。
- **EXPLORE｜系統實驗：**以 Software Co-Labs 探索延遲、記憶體、能耗與成本；README 當時標示為規劃中。

教材將內容分為基礎、設計、效能、部署、可信與前沿等部分，連結模型參數與記憶體限制、推論延遲與硬體加速、模型準確率與量化剪枝，以及隱私與端側學習等議題。

## 資源與狀態

- [線上教材](https://mlsysbook.ai/)
- [中文 README（dev 分支）](https://github.com/harvard-edge/cs249r_book/blob/dev/README/README_zh.md)
- [TinyTorch 入門](https://mlsysbook.ai/tinytorch/getting-started.html)
- [硬體套件](https://mlsysbook.ai/kits)
- README 表示紙本版預計於 2026 年由 MIT Press 出版，第二卷預計於 2027 年夏季推出；這些時程以專案最新公告為準。
- 本筆記依 2026-11-26 查看時的中文 README 整理；教材與學習棧持續更新。

## 授權與引用

- **教材內容：**CC BY-NC-ND 4.0，需署名、限非商業使用，且不得散布改作版本。
- **TinyTorch 程式碼：**Apache 2.0，可依該授權使用、修改與散布。
- 其他元件請分別確認其授權；不要將程式碼授權套用到書籍內容。
- README 提供 IEEE 2024 引用格式；正式引用時請以原頁提供的 BibTeX 為準。
