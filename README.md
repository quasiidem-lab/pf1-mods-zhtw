# PF1 模組合輯 繁體中文

為 Foundry VTT 的 Pathfinder 1e 常用模組提供繁體中文（臺灣）介面。

## 涵蓋範圍

一個模組涵蓋 19 個上游模組，共 3,567 條字串。

| 語系檔 | 條數 | 對應模組 |
|---|---:|---|
| `StatblockConverter.json` | 1186 | Pathfinder 1e Statblock Converter (SBC) |
| `RollBonuses.json` | 586 | Roll Bonuses |
| `CRLNGN_UI.json` | 508 | Carolingian UI |
| `LittleHelper.json` | 348 | Koboldworks – Little Helper |
| `ItemHints.json` | 144 | Koboldworks – Item Hints |
| `loot-sheet.json` | 135 | Loot Sheet |
| `AutomateDamage.json` | 119 | PF1 Automate Damage |
| `ECHPF1.json` | 117 | Enhanced Combat HUD (PF1) |
| `PF1AS.json` | 76 | Pathfinder 1e Alt Sheet（原版） |
| `AdvancedTemplates.json` | 65 | Advanced Templates PF1 |
| `SpellBookGenerator.json` | 59 | Spell Book Generator |
| `HealthOverTime.json` | 56 | Health Over Time |
| `PF1Cooking.json` | 39 | PF1 Cooking |
| `PF1AR.json` | 35 | PF1E Alt Sheet Reworked |
| `ReadyUp.json` | 24 | Koboldworks – Ready Up |
| `CompanionLink.json` | 20 | Koboldworks – Companion Link |
| `AuraShare.json` | 18 | Aura Share |
| `NAS.json` | 16 | Nevela's Automation Suite（狀態標籤） |
| `spellcasterutility.json` | 16 | Spellcaster Utility |

未安裝的模組不受影響——Foundry 只會載入用得到的鍵。

## 安裝

Foundry 的 **Add-on Modules → Install Module**，貼上 manifest URL：

```
https://github.com/quasiidem-lab/pf1-mods-zhtw/releases/latest/download/module.json
```

安裝後啟用模組，並將介面語言設為繁體中文（`zh-tw`）。

## 搭配使用

本模組只翻**模組介面**。另需搭配：

- **PF1 系統介面** → [`pf1-zhtw`](https://github.com/quasiidem-lab/pf1-zhtw)
- **Foundry 核心介面** → [`foundry-core-zh-tw`](https://gitlab.com/fvtt-zh_TW/foundry-core-zh-tw)

## 翻譯方式

多數語系檔的譯文以上游既有的簡體譯稿為基礎，經 OpenCC（`s2tw`）字形轉換，
再套用臺灣電腦術語校正表（`设置→設定`、`模块→模組`、`加载→載入`、`默认→預設`
等約 60 組），並將中文句中的半形括號轉為全形。

轉換過程會保護變數（`{name}`）、HTML 標籤、`@Command` 語法與 URL，確保不被
字形轉換破壞。

`NAS.json`、`PF1AR.json` 與 `PF1AS.json` 無既有中文譯稿，為對照英文原文的新譯。

## 譯名一致性

PF1 遊戲術語與 [`pf1-zhtw`](https://github.com/quasiidem-lab/pf1-zhtw) 保持一致。

一個已知的刻意差異：Nevela's Automation Suite 另外註冊了一個 `squeezed` 狀態，
與 PF1 系統原生的 `squeezing` 並存（兩者由該模組依通道寬度自動二擇一套用）。
為避免狀態列出現兩個同名項目，前者譯為「擠壓（NAS）」，後者維持「擠壓」。

## 授權

GNU General Public License v3.0（見 `LICENSE`）。

各語系檔的來源與其原始授權詳見 [`NOTICE.md`](NOTICE.md)。

## 作者

果園瑪莉卡
