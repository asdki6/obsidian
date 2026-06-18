---
type: concept
tags:
  - MCP
  - protocol
  - AI
  - integration
  - anthropic
summary: "MCP（模型上下文协议）是连接 AI 模型与外部工具/数据源的开放协议，让 Claude Code 等 Agent 可直接读写 Obsidian vault"
sources:
  - "wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md"
created: 2026-06-17
updated: 2026-06-17
---
# 概念_MCP协议

## 定义

**MCP（Model Context Protocol，模型上下文协议）** 是 Anthropic 推出的开放协议，定义了 AI 模型与外部工具、数据源之间的标准接口。它让 AI Agent 能够以结构化的方式访问文件系统、数据库、API 等外部资源。

## 核心原理 / 步骤

### 架构
```
AI Agent (Claude Code) ←→ MCP 协议 ←→ MCP Server ←→ 外部资源
                                          │
                                    ┌─────┼─────┐
                                文件系统   数据库   API
```

- **MCP Server**：暴露特定资源的服务（如 `obsidian-mcp-server` 暴露 Obsidian vault）
- **MCP Client**：AI Agent 端（如 Claude Code）通过协议发现和调用 MCP Server
- **标准化**：所有 MCP Server 使用统一接口，AI 无需为每个工具单独适配

### 在 Obsidian 生态中的应用
1. 安装 `obsidian-mcp-server`（npm 包）
2. 配置 Claude Code 的 `settings.json` 连接到该 MCP Server
3. Claude 即可：阅读笔记、搜索 vault、创建笔记、修改笔记、查找反向链接

### 对比其他集成方式
| 方式 | MCP | 插件 API | RAG 索引 |
|------|-----|---------|---------|
| 访问深度 | 完整读写 | 受限于插件接口 | 只读（检索） |
| 标准化 | ✅ 开放协议 | ❌ 各插件私有 | 部分标准 |
| 维护成本 | 一次配置 | 每个插件单独 | 需更新索引 |
| 适用场景 | Agent 主动维护 | 内嵌辅助 | 检索问答 |

## 应用场景
- **知识库维护**：Claude Code 通过 MCP 直接读写 Obsidian 笔记
- **数据分析**：连接数据库 MCP Server，AI 执行 SQL 查询
- **API 集成**：连接 GitHub/Linear/Slack MCP Server，AI 跨平台执行任务
- **自动化工作流**：多个 MCP Server 串联，AI 编排复杂流程

## 关联概念
- [[概念_上下文工程]]
- [[概念_AI第二大脑]]
- [[概念_LLM_Wiki]]

## 关联实体
- [[../../entities/tools/实体_Claude_Code]]
- [[../../entities/tools/实体_Obsidian]]

## 所属目录
- [[../../concepts/README|concepts/]] · [[../../../README|wiki/]]
