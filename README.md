# FrostFlower1 Story Player

以 GitHub Pages 執行的互動劇情播放器。首頁先選 Episode，再選 Chapter 才開始播放。

## 專案內容

- `index.html`：完整播放器介面與互動功能。
- `script_frostflower1.txt`：原始劇情 JSON（保留 TXT 格式與欄位）。修改並推送此檔後，部署網站會在重新載入時讀取新內容。
- 遊戲圖片與音效：直接放在 Repository 根目錄，路徑需與 TXT 內的 `background`、`image`、`sound`、`bgm`、`episode_image`、`CustomImage_Name` 等資源路徑相符。

## 自動載入素材

播放器會讀取 GitHub Repository 的遞迴檔案清單，自動建立素材索引；實際圖片／音效按需由 `raw.githubusercontent.com` 載入。你之後把資源放進專案根目錄（或保留 TXT 指定的子目錄結構）並推送後，重新開啟網頁即可自動配對，不需要手動選資料夾。素材支援 PNG/JPG/JPEG/WEBP/GIF、OGG/WAV/MP3/M4A。

注意：GitHub API 未驗證請求有速率限制；若素材清單非常龐大，可能需要改用建置時產生 manifest 的方式。素材檔名與路徑必須和 TXT 相符。

## 啟用 GitHub Pages

1. 開啟 Repository 的 **Settings → Pages**。
2. 在 **Build and deployment** 選擇 **Deploy from a branch**。
3. Branch 選 `main`，資料夾選 `/ (root)`，按 **Save**。
4. 等待部署完成，使用 GitHub Pages 提供的網址。

## 更新劇情與素材

- 修改 `script_frostflower1.txt` 後 commit/push，網站重新載入時會讀取最新內容。
- 圖片與音效依照 TXT 中的相對路徑放入 Repository 根目錄；路徑與檔名請保持一致。
- 不需要重新修改 HTML，也不需要使用者手動匯入素材資料夾。

## 公開內容提醒

此 Repository 為公開專案。請確認你有權公開散布原始遊戲劇情、圖片、音樂及音效，再上傳相關內容。
