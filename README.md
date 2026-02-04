# Gakumass學園偶像大師漢化（自動更新繁體版翻譯資料）

本專案會自動從上游 GitHub Release 下載 `GakumasTranslationData.zip`，使用 **OpenCC** 轉換為 **繁體中文（zhTW）**，再把結果打包成 `GakumasTranslationData_zhTW.zip` 並發佈到本 repo 的 **Release**。

## 功能
- 取得上游最新 Release（依版本號 tag）
- 下載 `GakumasTranslationData.zip`
- 轉換 `.txt` / `.json` 內容為繁體（預設 `s2twp.json`）
- 發佈 Release（標題格式：`Update: vX.Y.Z`）

## 自動更新規則
- 以「上游 Release 版本號（tag）」判斷是否更新  

## 排程
每 8 小時檢查一次（UTC+8）：
- 00:30 / 08:30 / 16:30

## 手動執行
到 GitHub → **Actions** → 選擇工作流程 → **Run workflow** 即可手動更新。

## 來源
- 上游資料來源：`chinosk6/GakumasTranslationData`
- 轉換工具：OpenCC
