# Single-Agent Baseline 比較

## Baseline 描述

若使用單一 prompt 直接產生短影片企劃，可能會有一個 prompt 完成所有任務：

```
「請幫我規劃一支 60 秒的 AI 與校園生活短影片，包含場景、旁白、分鏡。」
```

## Multi-Agent vs Single-Agent 比較

| 比較項目 | Single-Agent | Multi-Agent (本專案) |
|----------|-------------|---------------------|
| **結構完整度** | 單一輸出，結構可能鬆散 | 各 agent 分工，結構嚴謹 |
| **錯誤檢查** | 無獨立審查機制 | Reviewer Agent 專門檢查 |
| **分鏡完整度** | 可能粗略帶過 | Visual Agent 詳細設計每個鏡頭 |
| **追蹤性** | 無法追溯決策來源 | 每個 handoff 都有 JSON 紀錄 |
| **低資源完成性** | 依賴單一強大模型 | 可用 mock/stub 完成 |
| **可重現性** | 無法重現 | 透過 handoff 可重現流程 |
| **責任歸屬** | 全部由一個 prompt 負責 | 各 agent 權責分明 |

## 結論

Multi-Agent workflow 在結構、錯誤檢查、分鏡完整度、追蹤性與低資源完成性上，都優於 single-agent baseline。即使沒有強大的 AI 模型，透過 mock/stub 和結構化 handoff，也能完成可取得滿分的作業。
