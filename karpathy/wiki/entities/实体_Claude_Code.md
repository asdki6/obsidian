---
type: entity
tags:
  - claude
  - AI
  - CLI
  - anthropic
  - MCP
summary: "Claude Code 是 Anthropic 的 CLI AI 编程代理，通过 MCP 协议可直接读写 Obsidian vault，是 AI 知识管理的最强搭档"
sources:
  - "wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md"
created: 2026-06-17
updated: 2026-06-17
---
# 实体_Claude_Code

## 基本信息
- **类型**：软件 / AI Agent CLI 工具
- **开发者**：Anthropic
- **模型**：Claude (Opus / Sonnet / Haiku)
- **官网**：https://claude.ai

## 特征 / 属性

### 核心能力
- **CLI 原生**：在终端中运行，可直接操作文件系统
- **MCP 集成**：通过模型上下文协议连接外部工具和数据源
- **工具使用**：可执行 Bash 命令、读写文件、调用 API
- **长上下文**：支持超长上下文窗口（200K tokens）

### 在 Obsidian 生态中的角色
- 通过 `obsidian-mcp-server` 直接读写 vault 中的 Markdown 文件
- 可跨数百篇笔记进行交叉引用和分析
- 可按用户指令创建、修改、组织笔记
- 结合 Obsidian CLI 可利用 graph、反向链接等元数据

### 与其他 AI 方案对比
- vs Obsidian 插件（Smart Connections/Copilot）：Claude Code 更灵活、可执行复杂多步操作，但需要终端操作
- vs ChatGPT 文件上传：Claude Code 直接操作本地文件，无需上传，隐私更好
- vs 通用 RAG：Claude Code 不只是检索，还能主动维护和更新知识库

## 关键事件
- 2024：Claude Code 发布
- 2025：MCP 协议广泛采用，obsidian-mcp-server 出现
- 2026：Claude Code + Obsidian 成为 AI 第二大脑的主流方案

## 关联概念
- [[../concepts/概念_MCP协议]]
- [[../concepts/概念_AI第二大脑]]
- [[../concepts/概念_上下文工程]]
- [[../concepts/概念_LLM_Wiki]]

## 关联实体
- [[实体_Obsidian]]
- [[实体_Notion]]
- [[实体_Ollama]]

## 备注
- 本 vault 通过 RealClaudian 插件使用 Claude Code（配置：Opus 模型、plan 模式、effort=max）
- [[CLAUDE.md]] 是本 vault 的 Schema 文件，Claude Code 每次会话自动读取
