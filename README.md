# 紅焰教學：數位與 AI 融入備課助理 (AntiGravity Skill)

這是一個專為教育工作者設計、並原生支援 **AntiGravity** 平台架構的 Agent Skill。旨在協助教師快速生成符合最新《數位與 AI 教學指引》的結構化教案，結合教育洞察與 AI 應用，讓備課過程更精準、有溫度。

## 💡 AntiGravity 部署指南

要讓此 Skill 在 AntiGravity 順利運行，請依照以下步驟進行環境配置：

1. **建立 Agent / Skill**：在 AntiGravity 工作區中新建一個 Agent 專案或 Skill 模組。
2. **匯入核心配置**：
   - 讀取本 Repo 的 `agent_config.yaml` 來建立系統變數（Inputs）。
   - 將 `system_prompt.md` 的完整內容直接貼入 AntiGravity 的 System Prompt 欄位。
3. **確認輸入變數 (Inputs)**：請確保 AntiGravity 介面中已綁定以下三個必填變數：
   - `{{lesson_duration}}` (課程節數，例如：一節)
   - `{{grade_and_subject}}` (年級與科目，例如：八年級地理課)
   - `{{lesson_topic}}` (課程主題，例如：都市熱島)
4. **掛載 RAG 知識庫**：**最重要的一步！** 請在 AntiGravity 的 Knowledge Base (RAG) 模組中，確實上傳並啟用以下三份核心檔案，否則無法保證輸出格式的精準度：
   - `教案示範檔案.docx`
   - `數位與AI教學指引.pdf`
   - `指引教案格式.docx`

## 🛠 核心產出架構

本 Agent 執行後將自動生成以下結構化內容：
- 學科核心概念分析
- 常見迷思預測與認知衝突
- 素養導向的學習目標設定
- 生活情境導入設計
- 小組探究任務規劃
- AI 使用紅黃綠燈評估規範
- 學生 AI 素養對應表
- 完整師生互動與 AI 融入教案流程表

---
© 紅焰教學 版權所有 歡迎使用
