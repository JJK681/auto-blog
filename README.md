# auto-blog

自動發文部落格倉庫。

## 流程

1. Claude 產生文章 → 放到 Notion「文章庫」，狀態設為 **待發布**
2. 每週五 15:00（台北時間）Grok 自動讀取待發布文章
3. Grok 透過 GitHub 把文章寫入 `content/blog/`
4. Replit 偵測到更新後自動重新部署

## 文章格式

檔案路徑：`content/blog/{slug}.md`

```markdown
---
title: "文章標題"
slug: "my-post"
description: "簡短摘要"
tags: ["技術", "教學"]
date: 2026-10-10
---

正文 Markdown…
```

## Notion 資料庫

https://app.notion.com/p/6139f6ceb01544ec9e0650d003b8c62d
