# 德州撲克原始碼｜金幣大廳、多玩法與 Unity UI 資料

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [English](README.en.md) · [产品页面](https://niubideren111.github.io/Texas-Holdem-Game-Source-Code/zh-tw/)

以金幣大廳和多玩法進入點為主題的德州撲克專案資料，展示登入、SNG 選場和宝箱等介面。公開程式碼包含 Unity C# 與 Lua UI 适配器、簽名工具和伺服器非同步回呼片段。

**德州撲克原始碼 · 德州原始碼 · 德州金幣大廳原始碼 · Unity扑克原始碼**

## 專案重點

### 大廳與玩法進入點

透過登入、SNG 選場和活動截圖展示行動端大廳的資訊組織。

### Unity 與 Lua UI

LuaOSAListAdapter.cs、LuaOSATableAdapter.cs 和 LuaUIObject.cs 展示列表及 UI 适配。

### 服務回呼與工具

external 中的登入及使用者回呼和 SignatureTool.cs 提供工程閱讀進入點。

## 資料閱讀與核對方式

1. **先確認產品形態**：依序檢視截圖與圖說，確認產品類型和可見功能流程。
2. **再核對檔案證據**：直接開啟下方列出的原始碼或文件，不只依賴功能描述。
3. **檢查可建置範圍**：確認欲執行的部分是否具備相依套件、資源、設定與啟動腳本。
4. **確認授權**：閱讀儲存庫授權；商業素材及完整工程交付應另行取得書面授權。

## 產品截圖

![德州撲克金幣大廳宝箱活動介面](docs/assets/seo/texas-holdem-game-source-code-01.jpg)

![德州撲克 SNG 選場與買入檔位](docs/assets/seo/texas-holdem-game-source-code-02.jpg)

![德州撲克手機號登入介面](docs/assets/seo/texas-holdem-game-source-code-03.jpg)

## 公開原始碼與資料

| 文件 | 说明 |
|---|---|
| [LuaOSAListAdapter.cs](LuaOSAListAdapter.cs) | Lua 列表适配器 |
| [LuaOSATableAdapter.cs](LuaOSATableAdapter.cs) | Lua 表格适配器 |
| [LuaUIObject.cs](LuaUIObject.cs) | Lua UI 對象桥接 |
| [SignatureTool.cs](SignatureTool.cs) | 簽名工具類 |
| [external/AsyncLoginCallback.cpp](external/AsyncLoginCallback.cpp) | 伺服器端登入回呼片段 |

## 開始閱讀

```bash
git clone https://github.com/niubideren111/Texas-Holdem-Game-Source-Code.git
cd Texas-Holdem-Game-Source-Code
```

## 常見問題

### 本專案與私人局專案有何不同？

本頁突出金幣大廳、玩法選擇和 Unity UI 程式碼；私人局專案侧重組局、俱樂部牌桌和場景資料。

### 從哪個文件了解用戶端介面？

從 LuaUIObject.cs 入手，再閱讀列表和表格适配器，了解 C# 與 Lua 介面的連接方式。

## 後續資料完善方向

补充登入到大廳的流程圖、玩法進入點截圖、UI 适配器用法和 Unity 版本說明；獨立列出 SNG/MTT 的實作範圍。 後續更新還應加入版本化相依清單、經過驗證的建置或匯入步驟、簡明架構／產品流程圖，以及能對應真實檔案變更的版本記錄。大型授權資源可放入 GitHub Releases 並提供校驗值，不能提交密鑰、生產位址或使用者資料。

## 相關專案

- [Texas-Hold-em-source-code](https://github.com/niubideren111/Texas-Hold-em-source-code)
- [dezhou-poker-club-source-code](https://github.com/niubideren111/dezhou-poker-club-source-code)
- [Texas-Hold-em-Tournament-Source-Code](https://github.com/niubideren111/Texas-Hold-em-Tournament-Source-Code)

## 資料範圍與授權

公開儲存庫提供 UI 适配程式碼、工具類、伺服器回呼片段及產品截圖；完整用戶端、伺服器端和資料設定透過專案聯絡方式溝通。 公開內容以實際檔案、相依套件與授權為準，不承諾搜尋排名、直接上線或固定效能結果。

- Telegram: [@fox_lovemyself](https://t.me/fox_lovemyself)
- GitHub: [Texas-Holdem-Game-Source-Code](https://github.com/niubideren111/Texas-Holdem-Game-Source-Code)
