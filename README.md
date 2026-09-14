# VMware Workstation 中文化語言包（繁體中文・简体中文）

VMware Workstation 中文化語言包下載：繁體中文 (zh-TW) 與簡體中文 (zh-CN)，含 `vmware.vmsg` 與 MUI DLL（`vmappsdk` / `vmui`），下載後按安裝方法複製到安裝目錄即可使用。

> 本包由法語官方語言包翻譯產生，DLL 採等長 patch，檔案大小與原文完全一致。

## 下載（主推繁體中文）

請到右側 **Releases** 下載對應版本的 zip（一包即一套，含 3 個檔 + 安裝說明）：

| 版本 | zh-TW 繁體中文（主推） | zh-CN 简体中文 |
|---|---|---|
| 26H1-25388281 | `26H1-25388281-zh_TW.zip` | `26H1-25388281-zh_CN.zip` |

每包內容：`zh_<語系>/` 資料夾（含 `vmappsdk`、`vmui`、`vmware.vmsg`）+ `安裝說明.txt`，解壓後把資料夾整個複製進 `messages` 即可。

## 安裝方法（不用重啟，用捷徑參數切換語系）

1. 解壓 zip，把 `zh_TW/`（或 `zh_CN/`）整個資料夾複製到 VMware Workstation 安裝目錄的 `messages` 資料夾內（建議先備份原檔）。此步不用關閉 Workstation。
2. 在 Workstation 捷徑按右鍵 > 內容，在「目標」最後空一格加上 `--locale <語系>`：
   - 繁體中文：`"C:\Program Files\VMware\VMware Workstation\vmware.exe" --locale zh_TW`
   - 简体中文：`"C:\Program Files\VMware\VMware Workstation\vmware.exe" --locale zh_CN`
3. 用該捷徑啟動即為中文；不加參數啟動則維持原語系（可各建一個捷徑並存）。

> 注意：語言包與版本綁定，版本不符請勿混用；升級 Workstation 後請回來抓新版。

## 適用版本

- `26H1-25388281`（詳見各 Release 說明）

## 檔案說明

- `messages/zh_TW/vmware.vmsg`、`messages/zh_CN/vmware.vmsg`：介面字串（純文字，隨 repo 供預覽校對）
- DLL 只隨 Release 發布，不進 git（見 `.gitignore`）

## 自行產生語言包

想自己跑翻譯流程（換來源語系、修術語、跟新版），請見技能 repo：`opencode-vmware-mui-skill`（含抽取 / 翻譯記憶 / 等長 patch / 檢查腳本）。

## 版權聲明

- 本 repo 的文件與說明採 MIT 授權（見 `LICENSE`）。
- DLL / vmsg 譯文衍生自 VMware 官方檔案，版權屬 Broadcom / VMware，使用需自備正版 VMware Workstation，僅供學習研究。詳見 `NOTICE.md`。

## English

Chinese (Traditional `zh-TW` and Simplified `zh-CN`) language packs for VMware Workstation. Download the zip matching your build from Releases, back up the originals, copy the 3 files into the installed `messages` folder, and restart. See `NOTICE.md` for license terms.
