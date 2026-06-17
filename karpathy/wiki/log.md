---
type: log
---

# Wiki 操作日志

## [2026-06-17] setup | LLM Wiki 知识库架构初始化
- 创建目录结构：`karpathy/raw/`（articles, books, papers, media, assets）、`karpathy/wiki/`（sources, entities, concepts, comparisons, overview）
- 创建 `karpathy/wiki/index.md` 内容索引
- 创建 `karpathy/wiki/log.md` 操作日志
- 创建 `90 - 模板/llm-wiki/` 页面模板（5 种类型）
- 创建 `karpathy/CLAUDE.md` Schema 文件

## [2026-06-17] ingest | karpathy/raw/articles/NxCode_Obsidian_AI_第二大腦指南_2026.md → karpathy/wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md
- 新建来源摘要页：`karpathy/wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md`
- 新建实体页（3个）：`实体_Obsidian`、`实体_Claude_Code`、`实体_Notion`
- 新建概念页（4个）：`概念_AI第二大脑`、`概念_上下文工程`、`概念_MCP协议`、`概念_RAG检索增强生成`
- 更新 `karpathy/wiki/index.md`：8个页面条目（1 来源 + 3 实体 + 4 概念）
- 受影响页面总计：8 个新建 + 1 个更新（index.md）
