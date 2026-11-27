# 生活日誌

把 Threads 上的美食、旅遊與學習資料整理成 Markdown。每篇保留來源連結與文字，圖片存入 Git，影片保留連結。其他平台可以沿用同一份範本，修改 `platform` 欄位即可。

## 在瀏覽器閱讀

任何人都可直接開啟網站，用分類導覽或頁首搜尋找筆記。網站由 GitHub `main` 分支的 `vault/` 建置，包含收件匣、分類筆記和圖片附件。推送相關更新後，GitHub Actions 會自動重新建置與發布。[生活日誌](https://frsvffcy.github.io/life-vlog/)

## 在 Obsidian 開啟

```sh
git clone https://github.com/frsvffcy/life-vlog.git
```

1. 在 Obsidian 選「開啟資料夾為保存庫」，開啟 clone 下來的 `life-vlog/vault`。
2. 在「檔案與連結」將新附件位置設為 `attachments`，連結格式選「檔案的相對路徑」，並關閉 Wikilinks。
3. 安裝社群外掛 **Git** 後，在 Obsidian 使用外掛的 Pull、Commit、Push 命令同步。Git repo 在保存庫的上一層。也可以從 clone 的目錄執行 Git 指令。

## 收錄貼文

將 [範本](templates/entry.md) 複製到 `vault/inbox/`，用 `YYYY-MM-DD-短標題.md` 命名。填寫來源網址、摘要與文字，把圖片實體檔放入 `vault/attachments/`，在筆記內用 Markdown 相對路徑引用。整理時將筆記移到對應分類，並在該分類首頁加入連結。索引遵循分類層級的單一路徑：上層首頁只連到下一層首頁，不重複列出文章；文章列在最末層分類首頁，依發布日期由新到舊排列，並同步 MkDocs 導覽。

## 預覽與搜尋

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
mkdocs serve
```

在瀏覽器開啟 [本機預覽](http://127.0.0.1:8000/)。MkDocs 會從 `vault/` 建置網站，並產生全文搜尋索引。

## GitHub Pages 操作紀錄

### 2026-11-27 啟用公開網站

1. 在 **Settings → General → Danger Zone** 確認 repository 已是 **Public**。
2. 在 **Settings → Pages → Build and deployment** 將 **Source** 設為 **GitHub Actions**。GitHub 確認已儲存，**Enforce HTTPS** 已勾選。[Pages 設定](https://github.com/frsvffcy/life-vlog/settings/pages)
3. 新增 [Pages 工作流程](.github/workflows/pages.yml)。當 `main` 的筆記、附件、建置設定、相依套件或工作流程有更新時，MkDocs 用 `mkdocs build --strict` 建置，再部署 `site/`。也可在 **Actions** 選 **Deploy life-vlog to GitHub Pages → Run workflow**，指定 `main` 手動發布。
4. 首次部署的 `build` 和 `deploy` 均成功，**Settings → Pages** 顯示網站已上線。[首次部署紀錄](https://github.com/frsvffcy/life-vlog/actions/runs/45949673266)
5. 本機建置確認 67 份 Markdown 都有對應網頁並收錄於搜尋索引，121 張 JPG 與原始檔一致。用未登入的 HTTPS 請求確認首頁、學習分類、AI 產圖分類、海報筆記及其五張原圖均可讀取，公開搜尋索引也涵蓋同一批 67 個頁面。另在 Chrome 實測分類導覽及中文搜尋「旅遊藝術海報」。[海報筆記](https://frsvffcy.github.io/life-vlog/learning/ai-image/2026-10-06-gjirokaster-travel-poster/)
