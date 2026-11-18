# Episode 1 / Episode 2 素材缺漏複查報告

複查日期：2026-11-18  
分支：`main`

## 最新複查結果

已修正 Repository 中所有圖片檔案名稱尾端重複的 `.png.png`，並重新檢查 Episode 1、Episode 2 劇情引用及 `customimage.txt` 的路徑映射。

| 檢查項目 | 修正前 | 修正後 |
|---|---:|---:|
| `.png.png` 結尾檔案 | 29 | **0** |
| 缺少劇情圖片引用 | 21 | **0** |
| 缺少 BGM | 0 | **0** |
| 缺少 SFX | 0 | **0** |
| `customimage.txt` 無實體檔案的映射 | 29 | **0** |

<badge>Episode 1 和 Episode 2 的劇情素材引用均已找到對應實體檔案。</badge>

## 本次改名內容

共改名 **29 個圖片檔案**，不重新編碼或重新上傳圖片內容，只調整 Git 路徑名稱：

- 5 張劇情插圖：`cut_026` 至 `cut_030`
- 16 張 Episode 2 使用的角色立繪
- 8 張目前未被 Episode 1／2 使用的暗色角色立繪

改名規則：`filename.png.png` → `filename.png`。

## 驗證方式

本次使用 GitHub `main` 分支完整遞迴檔案樹（444 個檔案，API 回傳未截斷），並重新解析：

- `script_frostflower1.txt`：6 Chapters、672 個節點
- `script_frostflower2.txt`：3 Chapters、370 個節點
- `customimage.txt`：340 筆圖片名稱映射

所有劇情中的背景、插圖、角色立繪、BGM 和 SFX 引用均已逐一核對；同時確認所有 `customimage.txt` 映射路徑均能在 Repository 找到對應檔案。

## 結論

**目前 Episode 1 和 Episode 2 在檔案路徑層面已沒有缺少的圖片或音訊素材。**

本次只更改了 29 個圖片檔名及本報告，沒有修改劇情 TXT、`customimage.txt` 的內容或播放器程式碼。此驗證確認的是檔案存在與路徑對應，尚未逐張檢視圖片內容或實際播放測試。

## 本次盤點版本識別

- `script_frostflower1.txt` SHA：`395d7cd5f6a815ca80ef6a3e018128e263ba58e6`
- `script_frostflower2.txt` SHA：`653a60fa2731830b354e7a498bb49a9d7bb8e7ff`
- `customimage.txt` SHA：`d0c4a586666c9ed8e9b0f17a80ef98744a311596`
- Repository tree SHA：`76a36e8e7767fc6fbed06a2f09b86378fb79a86c`
