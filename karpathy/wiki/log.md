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

## [2026-06-18] ingest | GitHub Stars 批量摄入（8 个项目）
- 新建来源摘要页（8个）：`来源_GitHub_Stars_project-based-learning`、`来源_GitHub_Stars_developer-roadmap`、`来源_GitHub_Stars_build-your-own-x`、`来源_GitHub_Stars_freeCodeCamp`、`来源_GitHub_Stars_agency-agents`、`来源_GitHub_Stars_coding-interview-university`、`来源_GitHub_Stars_hello-agents`、`来源_GitHub_Stars_dive-into-llms`
- 新建实体页（1个）：`实体_Karpathy_系列项目`
- 新建概念页（3个）：`概念_项目驱动学习`、`概念_AI_Agent学习路径`、`概念_CS自学体系`
- 同步创建 `GitHub日常学习/obsidian/stars/learning/` 下 8 个学习笔记 + index.md
- 更新 `karpathy/wiki/index.md`：20个页面条目（9 来源 + 4 实体 + 7 概念）
- 受影响页面总计：12 个新建 + 1 个更新（index.md）

## [2026-06-18] ingest | GitHub Stars Python-100-Days
- 新建来源摘要页：`karpathy/wiki/sources/来源_GitHub_Stars_Python-100-Days.md`
- 新建学习笔记：`GitHub日常学习/obsidian/stars/learning/Python-100-Days.md`
- 更新 `karpathy/wiki/index.md`：21个页面条目（10 来源）
- 受影响页面：1 个新建 + 1 个更新（index.md）

## [2026-06-18] ingest | Claude Code 源码泄露事件
- 新建原始来源：`karpathy/raw/articles/ai/Claude_Code_源码泄露分析_2026.md`
- 新建来源摘要页：`karpathy/wiki/sources/来源_Claude_Code_源码泄露_2026.md`
- 更新实体页：`实体_Claude_Code`（补充技术架构、BUDDY/KAIROS等未发布功能）
- 更新 `karpathy/wiki/index.md`：22个页面条目（11 来源）
- 受影响页面：2 个新建 + 2 个更新

## [2026-06-18] lint | 链接修复 + 补充缺失页面
- 修复：`概念_AI第二大脑`/`概念_上下文工程` 中 `[[wiki/index.md]]` → `[[../index]]`
- 新建概念页（4个）：`概念_LLM_Wiki`、`概念_本地优先`、`概念_Smart_Connections`、`概念_Obsidian_Copilot`
- 新建实体页（1个）：`实体_Ollama`
- 删除 translations 下多余翻译文件（保留 cn）
- 更新 `karpathy/wiki/index.md`：28个页面条目（11来源 + 5实体 + 11概念 + 1对比 + 1综述）
- 受影响页面：6 新建 + 2 修复 + 1 更新（index.md）

## [2026-06-18] ingest | Markdown AI时代标准沟通语言
- 新建原始来源：`karpathy/raw/articles/methodology/Markdown_AI时代标准语言_2026.md`
- 新建来源摘要：`karpathy/wiki/sources/来源_Markdown_AI时代标准沟通语言_2026.md`
- 更新 `karpathy/wiki/index.md`：29个页面条目（12 来源）
- 受影响页面：2 新建 + 1 更新

## [2026-06-18] refactor | Wiki 文件夹子分类重构
- sources/ → sources/articles/（3篇）+ sources/github-stars/（10篇）
- entities/ → entities/tools/（4个）+ entities/projects/（1个）
- concepts/ → concepts/ai-km/（7个）+ concepts/learning/（2个）+ concepts/plugins/（2个）
- 全局修复所有内部 wikilink + 外部 GitHub日常学习 链接
- 更新 index.md 所有路径
