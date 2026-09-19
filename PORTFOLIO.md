# 待辦清單 Web App

這是在 GitHub Copilot 實戰工作坊中完成的待辦清單 Web App。專案以純前端技術實作，並透過 GitHub Copilot Agent Mode、MCP 與 agentic workflow 完成開發與工作流程整理。

## 線上展示

https://<你的帳號>.github.io/<你的repo名稱>/

> 請將上面的佔位網址替換成實際的 GitHub Pages 網址。

## 功能

- 新增待辦事項，空白內容不會新增。
- 勾選待辦事項並標記為完成，完成項目會顯示刪除線並淡化。
- 取消完成狀態，恢復為未完成項目。
- 刪除單筆待辦事項。
- 即時顯示整體未完成項目數量。
- 依「全部」、「未完成」或「已完成」篩選清單。
- 篩選後沒有符合項目時，顯示對應的空清單提示。
- 深色模式與淺色模式切換。
- 使用者未手動選擇主題時，依照作業系統的 `prefers-color-scheme` 設定顯示。
- 將待辦資料與主題偏好保存至瀏覽器 `localStorage`，重新整理後仍可保留。
- 版面置中、卡片式設計，並支援手機螢幕。

## 技術

- 使用 HTML、CSS 與原生 JavaScript。
- 不使用任何框架或套件，沒有 `package.json`，也沒有建置流程。
- 不引用外部 CDN，可離線運作。
- 使用 CSS 變數管理淺色與深色主題配色。
- 使用 `prefers-color-scheme` 偵測作業系統的主題偏好。
- 使用瀏覽器 `localStorage` 保存待辦資料與主題偏好。

## 開發方式

- **GitHub Copilot Agent Mode**：先提供完整需求，讓 Agent Mode 協助建立待辦清單 App，並在後續一次修改多個檔案，加入深色模式與篩選功能。
- **MCP**：透過 `.vscode/mcp.json` 連接 Microsoft Learn 與 GitHub MCP，查詢官方文件並讀取本 repo 的 GitHub issue。
- **Agentic workflow**：建立 `.github/copilot-instructions.md` 定義專案規則，再透過 `.github/prompts/fix-issue.prompt.md` 將讀取 issue、提出計畫、建立分支、修改、驗證、提交、推送與建立 Pull Request 的流程整理成可重複使用的劇本。
- **版本控制**：使用 Git commit、分支與 Pull Request 管理開發過程，並在需要時練習從既有版本還原檔案。

## 我學到什麼

- 如何使用 Agent Mode 從需求開始建立一個可操作的前端 App。
- 如何寫出清楚的需求，讓 AI 能更準確地完成多檔案修改。
- 如何使用 MCP 讓 AI 查詢外部官方文件與 GitHub repository 資訊。
- 如何把重複的 issue 修正流程整理成可版控的 agentic workflow。
- 如何使用 Git 分支、commit、rebase 與 Pull Request 管理修改並保留可回溯的版本。
