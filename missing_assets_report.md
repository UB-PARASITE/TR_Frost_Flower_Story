# Episode 1 / Episode 2 素材缺漏複查報告

複查日期：2026-11-18  
分支：`main`

## 複查結果摘要

本次重新檢查：

- `script_frostflower1.txt`（6 Chapters、672 個節點）
- `script_frostflower2.txt`（3 Chapters、370 個節點）
- `storyguide_frostflower1.txt`
- `storyguide_frostflower2.txt`
- `customimage.txt`（340 筆圖片名稱對照）
- Repository `main` 分支完整檔案樹（444 個檔案，API 回傳未截斷）

| 項目 | Episode 1 | Episode 2 |
|---|---:|---:|
| 缺少背景圖片 | 0 | 0 |
| 缺少劇情插圖 | 0 | 5 |
| 缺少角色立繪 | 0 | 16 |
| 缺少 BGM | 0 | 0 |
| 缺少音效 SFX | 0 | 0 |
| **目前劇情必需素材缺漏** | **0** | **21 張圖片** |

**與上次盤點相比，原先缺少的 11 張背景圖片、9 首 BGM 及 14 個 SFX 均已找到對應檔案。**  
目前共確認補齊了上次清單中的 34 個必需素材；剩餘 21 個缺漏全部是 Episode 2 圖片。

---

## A. 目前仍缺少的 21 張圖片

### A1. 劇情插圖（5 個）

| 應放置路徑 | Episode 2 使用位置 |
|---|---|
| `gui3/2026_prewinter/storycontents/cut_026.png` | Ch1 Node 57 |
| `gui3/2026_prewinter/storycontents/cut_027.png` | Ch1 Node 111；Ch3 Node 37 |
| `gui3/2026_prewinter/storycontents/cut_028.png` | Ch2 Node 48 |
| `gui3/2026_prewinter/storycontents/cut_029.png` | Ch2 Node 153 |
| `gui3/2026_prewinter/storycontents/cut_030.png` | Ch3 Node 29 |

### A2. 角色立繪（16 個）

以下名稱已存在於 `customimage.txt`，但對照表指定的檔案仍未出現在 Repository。

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

## B. 音效及背景音樂複查

| 類別 | 上次缺少 | 本次仍缺少 | 狀態 |
|---|---:|---:|---|
| BGM | 9 | 0 | <已補齊> |
| SFX | 14 | 0 | <已補齊> |

本次檢查沒有發現 Episode 1 或 Episode 2 仍引用不存在的音訊檔案。

Episode 2 中 3 處 `sound\\off`（Ch1 Node 49、Ch2 Node 92、106）屬於控制標記，不是實際音檔，沒有列入音效缺漏。

---

## C. customimage.txt 另外 8 個未被 Episode 1／2 使用的失效映射

以下 8 筆對照路徑仍然沒有實體檔案，但在 Episode 1、Episode 2 的劇情節點中都沒有引用。它們不計入上述 21 張「目前劇情必需素材」：

- `blank_back_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_back_dark.png`
- `blank_normal2_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal2_dark.png`
- `blank_normal3_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal3_dark.png`
- `blank_normal4_dark` → `gui3/2026_prewinter/storycontents/npcimg/blank_normal4_dark.png`
- `la_crying2_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_crying2_dark.png`
- `la_embarrassed_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_embarrassed_dark.png`
- `la_laugh_dark` → `gui3/2026_prewinter/storycontents/npcimg/la_laugh_dark.png`
- `xn_laugh2_2_dark` → `gui3/2026_prewinter/storycontents/npcimg/xn_laugh2_2_dark.png`

目前 `customimage.txt` 共 340 筆映射，其中 29 筆路徑未找到實體檔案：21 筆被 Episode 2 使用，另 8 筆未被這兩話使用。

---

## D. 結論

- Episode 1：劇情引用的圖片與音訊均已齊全。
- Episode 2：背景、BGM、SFX 均已齊全；仍缺 5 張劇情插圖及 16 張角色立繪。
- 若目標是讓目前 Episode 1、Episode 2 的所有劇情素材都能正常顯示，只需再補上 A 節列出的 21 張圖片。
- 本次只更新盤點報告，沒有修改劇情 TXT、`customimage.txt` 或播放器程式碼。

## E. 本次盤點版本識別

- `script_frostflower1.txt` SHA：`395d7cd5f6a815ca80ef6a3e018128e263ba58e6`
- `script_frostflower2.txt` SHA：`653a60fa2731830b354e7a498bb49a9d7bb8e7ff`
- `customimage.txt` SHA：`d0c4a586666c9ed8e9b0f17a80ef98744a311596`
- Repository tree SHA：`0cbb4ebe41cd277a540f74371966c4a9c181d561`
