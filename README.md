# 🏛️ 法學論文大綱審查工具｜Legal Thesis Outline Reviewer

[![Stars](https://img.shields.io/github/stars/HsinteHuang/legal-thesis-outline?style=flat&color=yellow)](https://github.com/HsinteHuang/legal-thesis-outline/stargazers)
[![Forks](https://img.shields.io/github/forks/HsinteHuang/legal-thesis-outline?style=flat&color=blue)](https://github.com/HsinteHuang/legal-thesis-outline/network/members)
![AI](https://img.shields.io/badge/AI-Claude%20%7C%20Gemini%20(Anthropic%20%7C%20Google)-blueviolet)
![Platform](https://img.shields.io/badge/Platform-claude.ai%20%7C%20ChatGPT%20%7C%20Gemini%20Gem-orange)
![Language](https://img.shields.io/badge/Language-繁體中文-red)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)
![Status](https://img.shields.io/badge/status-active-success)
[![Forked from](https://img.shields.io/badge/Forked%20from-mjib007%2Flegal--thesis--outline-lightgrey)](https://github.com/mjib007/legal-thesis-outline)

> 本開源內容是「論文寫作方法與AI輔助」課程之教材，本課程開設於中正大學高階法律碩士專班。

> 一套專為法律系碩士生設計的 AI 輔助論文大綱審查工具，依據「緒論→理論→制度→比較法→檢討→結論」的學術邏輯，逐層引導修正章節結構。

---

## ✨ 功能特色

- 📐 **架構邏輯檢查**：自動偵測章節順序是否符合法學論文標準框架
- 🔍 **章名焦點審查**：發現空泛章名，提示縮限至論文核心研究範圍
- 🏷️ **章名通用前綴檢查**：發現「理論基礎：」等通用前綴，提示直接以實質內容命名
- 🎭 **文學性副標題偵測**：發現「賦劍篇」、「鑄盾篇」等不符學術規範的副標題，提示以法律用語取代
- 🔗 **章名與節次對應檢查**：確認章名每個核心概念在節次中都有對應承接
- 🏷️ **節名討論對象標示**：同章討論多個制度時，提示節名須標明討論對象
- 📋 **制度介紹順序檢查**：確認全貌介紹節在具體機制節之前
- 📝 **論文題目主從關係檢查**：偵測主副標題是否主從倒置，核心問題應置於主標題
- ⚖️ **上位概念定位診斷**：判斷第二章各節是否真正服務全篇評價框架，避免制度內容錯置
- 🌏 **比較法銜接檢查**：確認外國制度章節與國內檢討章節之間的對話關係
- 🌐 **比較法單一國家提示**：只引用單一國家時，提醒在緒論或前言說明選擇理由
- 🔗 **第五章過渡節檢查**：避免比較法結論與修法建議之間出現邏輯斷層
- 📏 **格式規範檢查**：節名標點統一使用冒號、法條與法令名稱使用全名
- 🎯 **核心方向推測**：收到大綱後，主動從章節矛盾推測2-3個可能研究方向，說明推測依據，再讓學生確認，而非直接問開放式問題
- 💬 **逐步互動引導**：一步一步確認，不會一次給出所有建議讓人不知所措

---

## 📁 專案內容

| 檔案 | 說明 | 適用平台 |
|------|------|----------|
| `SKILL_legal_thesis_outline_updated.md` | Claude 專案 SKILL 版 | Claude.ai 專案功能 |
| `legal_thesis_outline_prompt.md` | 通用 Prompt 版 | ChatGPT、Gemini、Claude 等所有 AI 對話介面 |
| `gemini_gem_prompt.md` | Gemini Gem 專用版 | Google Gemini Gem（含安全規則與角色鎖定） |
| `README.md` | 本說明文件 | — |

---

## 🚀 使用方法

### 方法一：SKILL 版（推薦 Claude.ai 用戶使用）

適合已建立 Claude.ai 專案的使用者，設定一次後自動觸發，不需每次手動貼入。

**步驟：**
1. 進入 [Claude.ai](https://claude.ai)，開啟或建立一個「專案（Project）」
2. 在專案設定中找到「Project Knowledge」或「Custom Instructions」
3. 將 `SKILL_legal_thesis_outline_updated.md` 的內容上傳或貼入
4. 之後在該專案內的對話，只要出現「大綱」、「章節」、「論文架構」等關鍵字，即自動啟動審查流程

> ⚠️ 此版本**僅限 Claude.ai**，其他 AI 平台不支援 SKILL 格式。

---

### 方法二：Prompt 版（跨平台通用）

適合使用任何 AI 對話工具的使用者，包含 ChatGPT、Gemini、Copilot 等。

**步驟：**
1. 開啟 `legal_thesis_outline_prompt.md`，複製全部內容
2. 貼入任何 AI 對話框，送出
3. AI 確認載入後，會主動詢問你的論文題目與大綱
4. 提供資料後，即開始逐步審查

> ⚠️ 每次**新對話**都需要重新貼入，對話結束後不會保留設定。

---

### 方法三：Gemini Gem 版（推薦 Google Gemini 用戶使用）

適合已建立 Gemini Gem 的使用者，設定一次後即可重複使用，並內建安全規則防止角色逸脫。

**步驟：**
1. 進入 [Google Gemini](https://gemini.google.com)，點選「Gems」→「建立新 Gem」
2. 開啟 `gemini_gem_prompt.md`，複製全部內容
3. 貼入 Gem 的「指示」欄位，儲存
4. 之後直接在該 Gem 對話，提供論文題目與大綱即可開始審查

**與通用 Prompt 版的差異：**
- 加入 `<Security_Rules>`：防止使用者套取系統指令，確保角色鎖定
- 加入 `<Interaction_Rules>`：強制逐步引導，不得一次列出所有建議
- 針對 Gemini Gem 環境優化格式與指令結構

> ⚠️ 此版本為 Gemini Gem 格式設計，直接貼入一般對話框亦可使用，但最佳體驗需建立 Gem。

---

## 🧪 測試範例

不確定工具是否正常運作？可以用以下這份**刻意設計有問題的模擬大綱**來測試：

**論文題目：**《個人資料保護法之修正方向研究——以生成式AI蒐集個資為核心》

```
第一章 緒論
  第一節 研究動機與目的
  第二節 研究範圍與限制
  第三節 論文架構

第二章 個人資料保護之理論基礎
  第一節 資訊自決權之憲法依據
  第二節 個人資料保護之立法目的
  第三節 生成式AI與個資保護之交叉問題　　← 問題①

第三章 我國個人資料保護法之現行規範　　　← 問題②
  第一節 蒐集、處理與利用之要件
  第二節 當事人同意原則
  第三節 現行規範之缺漏

第四章 外國立法例比較
  第一節 歐盟GDPR之規範架構
  第二節 美國模式之分散立法
  第三節 比較法小結

第五章 我國制度之檢討與修正建議
  第一節 以歐盟模式為借鏡之可行性　　　　← 問題③
  第二節 修法建議
  第三節 小結

第六章 結論
```

**預設問題說明：**

| 編號 | 位置 | 問題描述 |
|------|------|----------|
| ① | 第二章第三節 | 具體爭議混入純理論章，應移至第三章 |
| ② | 第三章章名 | 章名空泛，涵蓋整部個資法，應縮限至生成式AI蒐集情境 |
| ③ | 第五章第一節 | 直接跳入歐盟模式評估，缺少統整比較法發現的過渡節 |

工具應能主動識別上述三個問題並提出修正建議。

---

## 🗂️ 審查項目總覽

| 審查層次 | 檢查項目 |
|----------|----------|
| 論文題目 | 主從關係是否倒置、核心問題是否置於主標題 |
| 第一層（章） | 章的數量、順序、章名焦點、章名通用前綴、文學性副標題、比較法位置 |
| 第二層（節） | 節的主題服務性、跨章錯置、每章前言與小結是否齊備、章名與節次對應、節名討論對象標示、制度介紹全貌先於細節、節名標點統一、法條全名使用 |
| 上位概念 | 第二章各節是否真正服務全篇評價框架、制度內容是否錯置 |
| 章節對話關係 | 理論→檢討的引用、比較法→修法的銜接、第五章過渡節、單一國家比較須說明選擇理由 |

---

## ⚡ 懶人包：30 秒上手

| 我用什麼 AI？ | 該拿哪個檔案？ | 怎麼用？ |
|--------------|--------------|---------|
| **Claude.ai**（有開專案） | `SKILL_legal_thesis_outline_updated.md` | 貼入專案的 Project Knowledge，之後自動觸發 |
| **Gemini**（想建 Gem） | `gemini_gem_prompt.md` | 建立新 Gem，貼入「使用說明」欄位，儲存後使用 |
| **其他 AI**（ChatGPT、Copilot 等） | `legal_thesis_outline_prompt.md` | 複製全文，直接貼入對話框送出 |

**啟動後只需要提供三件事：**
1. 論文題目
2. 研究動機與核心爭議
3. 現有大綱（有幾章貼幾章）

AI 會一步一步問你，不用一次準備齊全。

---

### 🖥️ 以 Claude Code 或 Antigrvity 為例的完整操作流程

**Step 1｜讀取原始庫**
```
https://github.com/mjib007/legal-thesis-outline
先讀取此庫
```

**Step 2｜載入 Prompt**
```
先讀取 legal_thesis_outline_prompt.md
```

**Step 3｜開始審查**
```
只要把研究大綱傳給你嗎？
```
> 可以！只貼大綱即可，AI 會主動詢問論文題目與研究動機等補充資訊。

**Step 4｜貼上大綱**
```
把大綱複製貼上
```

---

## 📜 授權

本專案以 [MIT License](LICENSE) 開源，歡迎自由使用、修改與分享。
若有改善建議，歡迎提交 Issue 或 Pull Request。

---

## 👥 貢獻者與版權

| 角色 | 姓名 | 貢獻 |
|------|------|------|
| 原作者 | Jackie Chien © 2026 | 工具核心設計、SKILL 版、通用 Prompt 版 |
| 改作者 | Hsinte Huang © 2026 | Gemini Gem 專用版（含安全規則與角色鎖定機制） |

本 Fork 基於原始專案 [mjib007/legal-thesis-outline](https://github.com/mjib007/legal-thesis-outline) 進行擴充，依 MIT License 授權條款改作並重新發布。

---

## 🔗 相關專案

- [📖 原始專案](https://github.com/mjib007/legal-thesis-outline) — Jackie Chien 的原版工具
- [🎓 刑法申論題 AI 教練](https://github.com/mjib007/legal-essay-tutor)
