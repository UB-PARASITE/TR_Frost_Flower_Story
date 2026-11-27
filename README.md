# Frost Flower Story Player

以 GitHub Pages 執行的互動劇情播放器。首頁先選 Episode，再選 Chapter 才開始播放。

## 專案結構

- `index.html`：完整播放器介面與互動功能。
- `Episode 1/`：Episode 1 劇情與 Chapter 導覽。
  - `script_frostflower1.txt`
  - `storyguide_frostflower1.txt`
- `Episode 2/`：Episode 2 劇情與 Chapter 導覽。
  - `script_frostflower2.txt`
  - `storyguide_frostflower2.txt`
- `Ex 1/`：Ex. 1 劇情及專用圖片對照表。
  - `script_frostflowerex1.txt`
  - `customimage2.txt`
- `customimage.txt`：共用圖片名稱／路徑對照表。
- `prewinter2026_schedule.data`：角色介紹資料。
- 遊戲圖片與音效：保留原有子目錄及相對路徑，供各篇劇情共用。

## 自動載入素材

播放器會讀取 GitHub Repository 的遞迴檔案清單，自動建立素材索引；實際圖片／音效按需由 `raw.githubusercontent.com` 載入。劇情及導覽檔案會由各 Episode 資料夾讀取；Ex. 1 的圖片對照表則由 `Ex 1/customimage2.txt` 讀取。

素材支援 PNG/JPG/JPEG/WEBP/GIF、OGG/WAV/MP3/M4A。素材檔名與路徑必須和劇情 TXT 中的設定相符。

## 啟用 GitHub Pages

1. 開啟 Repository 的 **Settings → Pages**。
2. 在 **Build and deployment** 選擇 **Deploy from a branch**。
3. Branch 選 `main`，資料夾選 `/ (root)`，按 **Save**。
4. 等待部署完成，使用 GitHub Pages 提供的網址。

## 更新劇情與素材

- 修改對應資料夾中的劇情或導覽 TXT 並推送後，網站重新載入時會讀取最新內容。
- 圖片與音效仍依照 TXT 中的相對路徑放在原有素材子目錄中，不需要搬動或重新匯入共用素材。
- 若新增 Ex. 1 圖片對照項目，請更新 `Ex 1/customimage2.txt`。
