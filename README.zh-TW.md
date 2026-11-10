# 流光筆記 FlashNote - 讓每一道流光，都有處安放。

> **你只管寫，剩下的交給我。**
> 側邊欄 Markdown 專注創作，所見即所得，圖表公式信手拈來；一鍵直發靜態部落格，長期內容自動沉澱為專欄、彙編成書。每一道流光，都替你安放成章。

[![Release](https://img.shields.io/github/v/release/Aicrosoft/FlashNote?color=blue&label=Latest%20Release)](https://github.com/Aicrosoft/FlashNote/releases)
[![Help Documentation](https://img.shields.io/badge/Docs-%E5%9C%A8%E7%B7%9A%E5%B9%AB%E5%8A%A9%E6%96%87%E6%AA%94-brightgreen)](https://aicrosoft.com/apps/flashnote/help/)
[![License](https://img.shields.io/badge/License-Proprietary-orange)](https://aicrosoft.com/)

📖 **官方在線說明文件**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)  
💬 **問題回報與建議**: [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues)

**多語言文件 (Languages)**:  
[🇨🇳 简体中文](README.zh-CN.md) | [🇺🇸 English](README.en.md) | [🇭🇰 繁體中文](README.zh-TW.md) | [🇯🇵 日本語](README.ja.md)

---

> [!WARNING]
> ⚠️ **桌面版特別提示 (Experimental Preview)**：
> 流光筆記桌面端（macOS / Windows / Linux）目前為**實驗性產品**，基於 Tauri 2.0 跨平台底層架構建置。若您在使用過程中遇到任何問題、異常崩潰或有任何交互改進建議，非常歡迎隨時在 [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) 中提出回報與問題，我們將持續迭代優化！

---

## 🚀 跨平台桌面端下載 (Downloads & Releases)

您可以在 [GitHub Releases](https://github.com/Aicrosoft/FlashNote/releases) 頁面獲取對應作業系統的最新安裝包：

| 作業系統    | 安裝包格式           | 說明                                          |
| :---------- | :------------------- | :-------------------------------------------- |
| **macOS**   | `.dmg` / `.app.zip`  | 蘋果電腦安裝映像檔 / 免安裝應用封裝檔         |
| **Windows** | `.exe` / `.msi`      | 現代化 NSIS 安裝精靈 / 經典 Windows Installer |
| **Linux**   | `.AppImage` / `.deb` | 跨發行版免安裝可攜包 / Debian & Ubuntu 安裝包 |

---

## 🌟 核心功能特性 (Feature Highlights)

### 1. ✍️ 極致純粹的沉浸式 Markdown 創作

- **極速冷啟動與開屏零卡頓**：重構底層資源載入調度與依賴按需延遲載入，徹底根除開啟後前 10 多秒按鈕卡頓假死問題，實現首屏秒級即點即用；
- **所見即所得編輯器**：基於 Tiptap (ProseMirror) 現代核心，即時渲染 Markdown 語法，程式碼高亮、表格、列表、待辦項目開箱即用；
- **打字徹底消除延遲**：標題輸入框與正文採用微觀狀態隔離，連續打字不再頻繁觸發全文件重渲染與磁碟寫入，敲擊 Enter 平滑跳入正文首行；
- **Markdown 標題貼上智慧淨化**：從外部網頁複製標題時，自動剝離前導 `#`、行內反引號、加粗等排版雜訊，游標智慧定位於末尾；
- **KaTeX 數學公式原生排版保真**：全層級自然塊級流排版，支援矩陣 (Matrix)、分段函數 (Cases)、高階積分上下標完美渲染，零遮擋零截斷。

### 2. 🌐 深度網頁剪藏與離線安全儲存

- **論壇全樓層討論完整捕獲**：深度適配技術社群（如 Discourse / LINUX DO 等），點擊剪藏按鈕，自動將視口內加載的樓主主貼與所有參與討論的樓層內容整齊捕獲並導入筆記；
- **右鍵深度摘要，完整保留長文主貼**：右鍵「摘要網頁內容」解除機械字數截斷限制，完整提取主貼全部多級小節、程式碼區塊與高畫質配圖，自動過濾無關評論雜音；
- **網路圖片全自動離線至本地**：每次剪藏網頁內容後，系統自動在後台執行遠端資源一鍵離線，將文章引用的所有網路圖片秒級下載並安全存入本地 OPFS，告別原貼刪圖、圖床失效與防盜鏈攔截。

### 3. 🛡️ 防誤刪安全機制與 Notion 緊湊工作台

- **防誤刪人機工程**：同名清理彈窗將「僅將當前選中文檔移入垃圾桶」設為醒目預設選項，其他副本 100% 完好無損；「全部移入垃圾桶」配有 5 秒可點擊的「撤銷復原」通知，手誤秒級還原；
- **Notion 屬性內聚工作台**：頂部操作列整合：目錄與分類緊湊並列，修改路徑與標籤不再大幅橫移滑鼠；獨立放置「轉為書籍專欄」入口；
- **底部狀態列極簡呼吸設計**：隱去重複標題，以輕量呼吸風格專注於即時字數統計、編輯儲存狀態與網路就緒情況，守護沉浸無擾的寫作環境。

### 4. ☁️ 穩定多端雲同步與 Git 靜態部落格直發

- **大檔案 4MB 分塊串流切片同步**：支援網盤大檔案切片上傳，接入 Precreate MD5 校驗和序列與最終合成機制，徹底杜絕大附件逾時失敗；
- **狀態機中斷自我修復與斷點續傳**：網路波動導致同步中斷時，狀態機自動安全回滾並支援斷點續傳，確保本地沙箱與雲端完全一致；
- **英文短名 (Slug) 智慧消歧**：重名筆記自動追加序號平滑化解全路徑衝突，普通日常隨手記 100% 保護 AI 配額，零浪費 Token；
- **Git 遠端部落格一鍵直發**：支援將文章直連推送至 GitHub、Azure DevOps 等代碼倉庫，一鍵構建靜態部落格，精準標註發布生命週期。

### 5. 📚 專欄長篇與電子書 EPUB 彙編成書

- **專欄彙編成書**：將日常積累的系列文章一鍵編排為章節目錄；
- **標準 EPUB 3.0 / Markdown 打包**：內建專業封面設計與排版模板，一鍵匯出可在各類電子閱讀器中流暢閱讀的標準電子書；
- **純前端離線 PlantUML 轉 Mermaid 引擎**：無需架設 Java 伺服器，純前端秒級轉譯；支援雙模平移縮放預覽與無損 SVG / 2x 高畫質 PNG 匯出。

### 6. 🤖 AI 智慧輔助長篇創作

- **創作生成自動收起**：點擊執行創作生成後，微調卡片立即自動收起，正文區域完整展現打字機式串流生成；
- **生成過程一鍵中止**：AI 正在生成時若再次展開面板，按鈕自動反轉為醒目的紅色「■ 停止生成」，點擊即刻停止；
- **超長篇幅與多文風基調**：支援 5000 字以上史詩長篇與 8000 字以上傳奇長文分小節結構化推進；提供「預設自然、通俗生動、理工嚴謹、商務公文、優美文學、幽默風趣」等 6 種文風基調。

---

## 💬 幫助與技術支援 (Help & Feedback)

- 📖 **官方在線說明文件**: [https://aicrosoft.com/apps/flashnote/help/](https://aicrosoft.com/apps/flashnote/help/)
- 🐞 **問題回報與建議**: 歡迎在 [GitHub Issues](https://github.com/Aicrosoft/FlashNote/issues) 中提交 Bug 報告或體驗建議。
