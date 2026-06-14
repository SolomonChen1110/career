# 韋丞個人網站 v1 — GitHub Pages 上線說明

整包檔案：10 個 `.html` 頁面 ＋ `og-default.png`（分享預覽圖）。首頁是 `index.html`。

---

## 三步驟上線

### 第 1 步｜建 repo 並上傳檔案
到 GitHub 點右上「＋ → New repository」，名稱例如 `career-site`，選 **Public**，建立。
進到 repo 後點 **Add file → Upload files**，把這包解壓後的**全部檔案**（10 個 html ＋ `og-default.png`）拖進去，最下方按 **Commit changes**。
※ 請確認 `index.html` 在 repo 的最上層（不要包在資料夾裡）。

### 第 2 步｜開啟 GitHub Pages
repo 上方 **Settings → 左側 Pages**。
Source 選 **Deploy from a branch**，Branch 選 **main**、資料夾選 **/ (root)**，按 **Save**。
等 1–2 分鐘重新整理，頁面上方會出現你的網址，格式是：
`https://你的帳號.github.io/career-site/`
把這個網址記下來，第 3 步要用。

### 第 3 步｜換上正確的網址（讓分享預覽正常）
每個 html 裡有一個佔位字串 `https://USERNAME.github.io/REPO`，要換成第 2 步拿到的真實網址（**結尾不要加斜線**）。
最快做法：在電腦上用編輯器（VS Code、Sublime 等）開資料夾，用「全資料夾取代」把
`https://USERNAME.github.io/REPO`
全部換成例如
`https://你的帳號.github.io/career-site`
存檔後，再上傳一次覆蓋（或用 git push）。
這一步只影響「分享到 FB／LINE／Threads 時的標題、描述與預覽圖」，不影響網站本身能不能開。

---

## 連結現況
- **個人諮詢／預約**：導覽列按鈕與各頁「預約」鈕 → 你的 Google 表單。
- **企業合作**：導覽列與各頁企業鈕 → 你的 Instagram。
- **《主人思維》**：→ 博客來商品頁。
- **Instagram**：→ hermitsolomoncareer。
- **Podcast《工作的人》**：標「即將上線」，上線後把網址給設計者補上即可。

## 之後想改內容
所有文字都直接寫在 html 裡，可用任何文字編輯器開啟修改後重新上傳。若要新增框架深度頁或改版面，回來找我即可。

---

## 關於圖片
- **三套牌卡圖**：直接連到 navicareer.tw（你公司站）的圖檔，部署後會正常顯示。
- **《主人思維》書封**：已用你提供的書封檔 `book-cover.jpg`，自己存在網站內，部署後一定會顯示。
- 想讓所有圖都自己掌握（不依賴外站）：把圖檔放進 repo，再把對應的 `src` 換成本地檔名。
