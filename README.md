# 從前震到主震｜高弘 Honn Kao 演講全紀錄

2026 年 10 月 15 日，中央氣象署。現場記錄與提問：陳達毅。

預定網站網址：https://oceanicdayi.github.io/2026_lecture_honn_kao/

## 內容

- 10 節完整導讀：前震、asperity／G–R、preslip／cascade、工業誘發機制、WCSB 觀測、SI、動態觸發、新成核模型與管理。
- 32 張原始照片（31 張不同照片，包含一張重複上傳），附可搜尋分類、完整尺寸放大與原始檔名。
- 2 段完整影片：約 1 分 14 秒及 2 分 42 秒，轉成適合網頁播放的 H.264 版本；原始音軌內容與時長保留。
- 從兩段影片抽出的 2 個 MP3 音訊檔。這次未收到額外獨立錄音檔。
- 影片時間段跳轉、意旨整理、重點字幕、未校訂自動辨識原稿。
- 6 項現場提問與延伸解釋、現場短記、POE／CER／CLIL 教案、互動公式與可匯出學習筆記。
- 主要研究及相關原始文獻連結。

## GitHub Pages 首次啟用

儲存庫設定 → **Pages** → Source 選 **Deploy from a branch** → Branch 選 **main**、資料夾 **/(root)** → Save。

設定連結：https://github.com/oceanicdayi/2026_lecture_honn_kao/settings/pages

網站已預先產生完整 `index.html`，不需要安裝套件或編譯。根目錄 `.nojekyll` 關閉 Jekyll 處理。

## 本機檢查與更新

```bash
python validate.py
node --check app.js
```

若修改 `content.json` 或 `build.py`：

```bash
python build.py
python validate.py
```

`build.py` 只使用 Python 標準函式庫，重新產生 HTML、照片資料與影片意旨整理。原始照片、已轉碼影音及辨識原稿不會由此覆寫。

## 檔案

- `index.html`、`styles.css`、`app.js`：靜態網站。
- `assets/photos/`：所有照片原始位元組；`assets/thumbs/`：瀏覽縮圖。
- `assets/video/`：網頁播放版；`assets/audio/`：影片音訊；`assets/posters/`：影片預覽。
- `transcripts/`：意旨整理、重點字幕、未校訂 ASR JSON。
- `data/media-manifest.json`：完整媒體對照與來源備註。
- `data/field-notes.json`：現場短記；`content.json`：導讀與科教內容。

原始影片分別約 159 MB、350 MB，超出 GitHub 一般單檔上限，故儲存庫使用保留完整內容的網頁播放版，而非上傳原始影片容器。照片保留原始大小。

## 內容與證據範圍

「92% 有前震」是研究選定的 77 組主震序列中的回溯比例，並非即時預測準確率。低 SI 不等於低危險。可改變破裂條件不等於可指定地震規模。管理建議不等同現行法規。

影音意旨整理與重點字幕不是逐字稿；ASR JSON 含辨識錯字，請以影音核對。照片、投影片與講者內容歸各原作者；本紀錄供回顧、研究及教學使用。

主要論文：Wang et al. (2026), *Science* 393, eaed9893. https://doi.org/10.1126/science.aed9893
