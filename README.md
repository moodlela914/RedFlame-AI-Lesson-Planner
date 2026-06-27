# 紅焰教學：數位與 AI 融入備課助理 Skill

這是一個專為教育工作者設計的 Agent Skill，幫助教師快速生成符合最新數位與 AI 教學指引的結構化教案。

## 💡 使用方式 (部署至 Agent 平台)

1. **建立 Agent**：在您的平台（如 Dify, GPTs, Coze）建立一個新助理。
2. **匯入提示詞**：將本 Repo 中的 `system_prompt.md` 內容貼入 Agent 的 System Prompt / Instructions 區塊。
3. **設定變數**：依據 `agent_config.yaml` 設定三個輸入變數：
   - `{{lesson_duration}}` (節數)
   - `{{grade_and_subject}}` (年級與科目)
   - `{{lesson_topic}}` (課程主題)
4. **掛載知識庫 (RAG)**：請務必在 Agent 的知識庫中上傳以下三份檔案，以確保輸出格式正確：
   - `教案示範檔案.docx`
   - `數位與AI教學指引.pdf`
   - `指引教案格式.docx`

## 🛠 產出內容架構
- 學科核心概念分析
- 常見迷思預測
- 學習目標設定
- 生活情境導入設計
- 小組探究任務規劃
- AI 使用紅黃綠燈評估
- 學生 AI 素養對應表
- 完整師生互動與 AI 融入教案流程表

© 紅焰教學 版權所有