# wiki/ — 知识层

> 🧠 LLM 全权维护。你读，LLM 写。这是持久化、可复利增长的知识产物。

## 子目录

| 目录 | 页面类型 | 命名格式 | 示例 |
|------|----------|----------|------|
| `sources/` | 来源摘要 | `来源_文章标题.md` | `来源_Obsidian_AI_第二大腦指南_2026.md` |
| `entities/` | 实体页 | `实体_名称.md` | `实体_Obsidian.md` |
| `concepts/` | 概念页 | `概念_名称.md` | `概念_上下文工程.md` |
| `comparisons/` | 对比页 | `对比_A_vs_B.md` | `对比_RAG_vs_Wiki模式.md` |
| `overview/` | 综述页 | `综述_主题.md` | `综述_AI个人知识管理.md` |

## 页面通用规范
- 所有页面必须包含 YAML frontmatter：`type`、`tags`、`summary`、`sources`、`created`、`updated`
- 内部链接使用 Obsidian `[[wikilink]]` 语法
- 中文 + 下划线命名，不包含特殊字符

## 根目录文件
- `index.md` — 内容索引，LLM 每次 Ingest 后更新
- `log.md` — 操作日志，仅追加
