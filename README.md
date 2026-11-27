# 生活日誌

把 Threads 上的美食、旅遊與學習資料整理成 Markdown。每篇保留來源連結與文字，圖片存入 Git，影片保留連結。其他平台可以沿用同一份範本，修改 `platform` 欄位即可。

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

GitHub Pages 尚未部署。私人 GitHub repo 的 Pages 網站可能公開，取決於帳戶方案與 Pages 存取設定。啟用前請先決定線上瀏覽所需的存取範圍。
