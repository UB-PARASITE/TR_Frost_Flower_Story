# Episode 1 / Episode 2 素材缺漏盤點

盤點日期：2026-11-18  
分支：`main`

## 盤點範圍與結論

本報告比對以下檔案，並以 GitHub Repository 的完整遞迴檔案清單（380 個檔案，API 回傳未截斷）檢查實際存在的檔案：

- `script_frostflower1.txt`、`script_frostflower2.txt`
- `storyguide_frostflower1.txt`、`storyguide_frostflower2.txt`
- `customimage.txt`（340 筆圖片名稱對照）
- Repository `main` 分支內的所有檔案路徑

| 項目 | Episode 1 | Episode 2 |
|---|---:|---:|
| Chapter | 6 | 3 |
| 劇情節點 | 672 | 370 |
| 缺少圖片 | 0 | 32 |
| 缺少 BGM | 0 | 9 |
| 缺少音效 | 0 | 14 |

**目前需要補齊 55 個實體素材檔案：32 張圖片、9 首 BGM、14 個音效。**  
Episode 1 的劇情引用均可找到對應檔案；目前缺漏集中在 Episode 2。

路徑大小寫以播放器的實際處理方式為準：`fileURL()` 會將路徑轉成小寫，因此下列「應放置路徑」均列出小寫形式。請使用完整相對路徑上傳，避免只上傳同名但位於不同資料夾的檔案。

---

## A. 缺少圖片（32 個）

### A1. 場景背景（11 個）

| 應放置路徑 | Episode 2 使用位置 |
|---|---|
| `gui3/2026_prewinter/storycontents/bg015.png` | Ch1 Node 101；Ch3 Node 28 |
| `gui3/2026_prewinter/storycontents/bg016.png` | Ch1 Node 119 |
| `gui3/2026_prewinter/storycontents/bg017.png` | Ch2 Node 92、100、106、116 |
| `gui3/2026_prewinter/storycontents/bg018.png` | Ch2 Node 126 |
| `gui3/2026_prewinter/storycontents/bg019.png` | Ch2 Node 150、154、155、159 |
| `gui3/2026_prewinter/storycontents/bg020.png` | Ch2 Node 103 |
| `gui3/2026_prewinter/storycontents/bg021.png` | Ch2 Node 169 |
| `gui3/2026_prewinter/storycontents/bg022.png` | Ch3 Node 1、29 |
| `gui3/2026_prewinter/storycontents/bg023.png` | Ch3 Node 51 |
| `gui3/2026_prewinter/storycontents/bg024.png` | Ch3 Node 56、69 |
| `gui3/2026_prewinter/storycontents/bg025.png` | Ch2 Node 2 |

### A2. 劇情插圖（5 個）

| 應放置路徑 | Episode 2 使用位置 |
|---|---|
| `gui3/2026_prewinter/storycontents/cut_026.png` | Ch1 Node 57 |
| `gui3/2026_prewinter/storycontents/cut_027.png` | Ch1 Node 111；Ch3 Node 37 |
| `gui3/2026_prewinter/storycontents/cut_028.png` | Ch2 Node 48 |
| `gui3/2026_prewinter/storycontents/cut_029.png` | Ch2 Node 153 |
| `gui3/2026_prewinter/storycontents/cut_030.png` | Ch3 Node 29 |

### A3. 角色立繪（16 個）

這些名稱已存在於 `customimage.txt`，但對照表指定的圖片檔案在 Repository 中找不到。

| 素材名稱 | 應放置路徑 | Episode 2 使用位置 |
|---|---|---|
| `blank_back` | `gui3/2026_prewinter/storycontents/npcimg/blank_back.png` | Ch3 Node 49 |
| `blank_normal2` | `gui3/2026_prewinter/storycontents/npcimg/blank_normal2.png` | Ch3 Node 20、43 |
| `blank_normal3` | `gui3/2026_prewinter/storycontents/npcimg/blank_normal3.png` | Ch3 Node 26 |
| `blank_normal4` | `gui3/2026_prewinter/storycontents/npcimg/blank_normal4.png` | Ch3 Node 17、21、27、33 |
| `ce_smiling2_sweat` | `gui3/2026_prewinter/storycontents/npcimg/ce_smiling2_sweat.png` | Ch1 Node 78 |
| `ce_smiling2_sweat_dark` | `gui3/2026_prewinter/storycontents/npcimg/ce_smiling2_sweat_dark.png` | Ch1 Node 79 |
| `la_crying2` | `gui3/2026_prewinter/storycontents/npcimg/la_crying2.png` | Ch1 Node 74 |
| `la_embarrassed` | `gui3/2026_prewinter/storycontents/npcimg/la_embarrassed.png` | Ch1 Node 52 |
| `la_laugh` | `gui3/2026_prewinter/storycontents/npcimg/la_laugh.png` | Ch1 Node 54 |
| `la_normal` | `gui3/2026_prewinter/storycontents/npcimg/la_normal.png` | Ch1 Node 72 |
| `la_normal_dark` | `gui3/2026_prewinter/storycontents/npcimg/la_normal_dark.png` | Ch1 Node 73 |
| `la_surprised` | `gui3/2026_prewinter/storycontents/npcimg/la_surprised.png` | Ch1 Node 82、83、97 |
| `la_surprised_dark` | `gui3/2026_prewinter/storycontents/npcimg/la_surprised_dark.png` | Ch1 Node 84、98、99 |
| `xn_gun` | `gui3/2026_prewinter/storycontents/npcimg/xn_gun.png` | Ch2 Node 94、96、98 |
| `xn_gun_dark` | `gui3/2026_prewinter/storycontents/npcimg/xn_gun_dark.png` | Ch2 Node 95、97、99 |
| `xn_laugh2_2` | `gui3/2026_prewinter/storycontents/npcimg/xn_laugh2_2.png` | Ch2 Node 15 |

---

## B. 缺少音效（23 個）

### B1. 背景音樂 BGM（9 個）

| 應放置路徑 | Episode 2 使用位置 |
|---|---|
| `sound/bgm/training_bownavi_slide.ogg` | Ch1 Node 1 |
| `sound/bgm/wishstone_upbeatguitar.ogg` | Ch1 Node 43 |
| `sound/bgm/wishstone_love.ogg` | Ch1 Node 57 |
| `sound/bgm/item_training_emotion_island.ogg` | Ch1 Node 101 |
| `sound/bgm/wishstone_beyondstars.ogg` | Ch2 Node 1 |
| `sound/bgm/park/bgm-horror-park-.ogg` | Ch2 Node 14 |
| `sound/bgm/wishstone_rain.ogg` | Ch2 Node 92、126 |
| `sound/bgm/wishstone_pianoversion.ogg` | Ch2 Node 106 |
| `sound/bgm/wishstone_strangematter.ogg` | Ch3 Node 2、17 |

### B2. 劇情音效 SFX（14 個）

| 應放置路徑 | Episode 2 使用位置 |
|---|---|
| `sound/wishstone_shining.wav` | Ch1 Node 6、95 |
| `sound/wishstone_effect4.wav` | Ch1 Node 7、26；Ch2 Node 82 |
| `sound/wishstone_brokenglass.wav` | Ch2 Node 7、150 |
| `sound/wishstone_falldown2.wav` | Ch2 Node 11 |
| `sound/wishstone_sword.wav` | Ch2 Node 22 |
| `sound/wishstone_magic.wav` | Ch2 Node 32 |
| `sound/wishstone_effect13.wav` | Ch2 Node 81 |
| `sound/wishstone_wind.wav` | Ch2 Node 90 |
| `sound/wishstone_seaside.wav` | Ch2 Node 103、169 |
| `sound/wishstone_bush.wav` | Ch2 Node 119、124 |
| `sound/wishstone_cave.wav` | Ch3 Node 50 |
| `sound/wishstone_magictwinkle.wav` | Ch3 Node 55 |
| `sound/wishstone_jaildoor.wav` | Ch3 Node 57 |
| `sound/wishstone_jaildoor2.wav` | Ch3 Node 64 |

### B3. 特殊標記（不列入缺少音效）

Episode 2 另有 3 處將 `sound` 設為 `sound\\off`：Ch1 Node 49、Ch2 Node 92、106。這看起來是停止／關閉音效的控制標記，不是應上傳的音檔，因此沒有列入 14 個 SFX。

---

## C. customimage.txt 中另外 8 個尚未被 Episode 1／2 引用的缺檔映射

以下映射也指向不存在的圖片，但在本次兩份劇情檔的 `ImgList` 中沒有找到引用。若將來劇情使用這些名稱，仍需補檔：

- `blank_back_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_back_dark.png`
- `blank_normal2_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal2_dark.png`
- `blank_normal3_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal3_dark.png`
- `blank_normal4_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal4_dark.png`
- `la_crying2_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_crying2_dark.png`
- `la_embarrassed_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_embarrassed_dark.png`
- `la_laugh_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_laugh_dark.png`
- `xn_laugh2_2_dark` → `gui3/2026_prewinter/storycontents/npcimg/xn_laugh2_2_dark.png`

---

## D. 補檔優先順序建議

1. **先補 A1 背景與 A2 劇情插圖**：缺少時會直接影響場景和關鍵劇情畫面。
2. **再補 A3 角色立繪**：缺少時對應角色可能無法顯示。
3. **最後補 B1／B2 音訊**：缺少時相應節點不會有預期音樂或音效。

補檔後再次執行相同路徑檢查，預期 A、B 的缺漏數應降為 0。這份盤點沒有修改任何劇情內容、素材路徑或播放器程式碼。
