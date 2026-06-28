# Final Agentic Short Video Project

## 專案名稱
AI 輔助校園生活宣傳短影片 — 多代理人協作流程

## 組員
蕭友翰

## 使用平台
Hermes Agent

---

## 專案簡介

本專案使用 Hermes Agent 設計一個受控式多代理人短影片製作 workflow，主題為「AI 與校園生活」，透過 AI 生成的圖片搭配剪輯工具，完成一支 60 秒可播放的短影片。

## 主題說明
- **目標觀眾**：高中生、大一新生、一般觀眾
- **核心訊息**：用 60 秒呈現 AI 如何融入大學校園生活，展現學習、創作、互動的可能性
- **影片長度**：60 秒（55-65 秒範圍）

## 如何閱讀本 Repo

| 資料夾 | 內容 |
|--------|------|
| `agents/` | 各 agent 的角色描述、prompt、輸入輸出格式 |
| `handoff/` | agent 之間的 JSON 交接資料 |
| `traces/` | execution trace 與執行紀錄 |
| `outputs/` | 最終短影片、字幕檔、素材來源表 |
| `baseline/` | single-agent baseline 比較 |
| `report/` | 專案報告 PDF |

## 零付費 token 可完成性聲明

本專案可在不購買任何商業 LLM token 的情況下完成：
- 使用 mock/stub agent outputs 展示多代理人分工
- 使用 AI 圖片生成工具（免費額度）製作影片素材
- 使用免費剪輯工具（如 DaVinci Resolve、CapCut）完成影片剪輯
- 使用免費 TTS 工具或人工錄製旁白

若使用付費 API，將於報告中揭露，並說明其非完成作業的必要條件。

## 素材來源與授權

- 圖片：AI 生成（Microsoft Designer + DeeVid，見 outputs/asset_sources.md）
- 音樂/音效：免費音樂庫（標註來源）
- 字幕/旁白：自製

## 加分項目

本專案 **未選擇** 國立臺南大學資訊工程學系形象宣傳影片加分項目。
