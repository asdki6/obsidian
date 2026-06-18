---
type: concept
tags:
  - llm
  - wiki
  - knowledge-management
  - karpathy
summary: "LLM Wiki 模式——让 LLM 主动维护持久化知识层，而非每次从零检索"
sources:
  - "karpathy/wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md"
created: 2026-06-18
updated: 2026-06-18
---

# 概念_LLM_Wiki

## 定义

**LLM Wiki** 是 Andrej Karpathy 提出的知识管理模式：不是每次查询时用 RAG 从原始文档临时检索，而是让 LLM **增量构建和维护一个持久化的 Wiki 知识层**——知识被编译一次、持续保鲜、可复利增长。

## 核心原理

| 传统 RAG | LLM Wiki |
|----------|----------|
| 每次查询从零拼凑 | 知识预编译、持续保鲜 |
| 无积累 | 持久化产物，可复利增长 |
| 交叉引用每次重发现 | 已预制在 wiki 页面中 |
| 人类维护 wiki（易放弃） | LLM 维护 wiki（零成本） |

## 三层架构
1. **raw/** — 原始来源，只读不可变
2. **wiki/** — LLM 维护的知识层
3. **Schema（CLAUDE.md）** — 告诉 LLM 如何维护 wiki

## 三种操作
- **Ingest**：摄入新来源 → 写摘要 → 更新实体/概念 → 更新索引
- **Query**：基于 wiki 回答 → 若有价值归档为新页面
- **Lint**：健康检查 → 矛盾/过时/孤立 → 生成建议清单

## 在本知识库中的体现

本 vault 的 `karpathy/` 即 LLM Wiki 的完整实现。

## 关联概念
- [[概念_上下文工程]]
- [[概念_AI第二大脑]]
- [[概念_RAG检索增强生成]]
