---
type: source
tags:
  - claude-code
  - source-leak
  - anthropic
  - security
summary: "2026年3月 Claude Code 512K行TypeScript源码因npm打包失误意外公开，揭示BUDDY/KAIROS/Undercover等未发布功能"
sources:
  - "karpathy/raw/articles/ai/Claude_Code_源码泄露分析_2026.md"
created: 2026-06-18
updated: 2026-06-18
---

# 来源_Claude_Code_源码泄露_2026

## 来源信息
- **标题**：Claude Code 源码泄露事件
- **日期**：2026-03-31
- **发现者**：Chaofan Shou (@Fried_rice)
- **原因**：npm source map 打包失误，暴露 R2 存储桶中的未混淆源码

## 核心要点

1. **泄露规模空前**：~1,900 个 TS/TSX 文件，512K+ 行代码，40+ Agent 工具，85+ Slash 命令
2. **BUDDY 虚拟伙伴**：18 种 AI 宠物，5 维属性，原计划 2026.4 发布
3. **KAIROS 自主 Agent**：主动监控 + 夜间"做梦"整理记忆，仍在内部测试
4. **Undercover Mode**：Anthropic 员工自动隐藏 AI 身份
5. **技术架构**：TypeScript + Bun + React/Ink + Zod，QueryEngine.ts 达 46K 行
6. **三层上下文压缩**：reactive → micro → trimmed

## 关联实体
- [[../entities/实体_Claude_Code]]

## 关联概念
- [[../concepts/概念_MCP协议]]
- [[../concepts/概念_上下文工程]]
- [[../concepts/概念_AI_Agent学习路径]]

## 关联文件
- 原始分析：[[karpathy/raw/articles/ai/Claude_Code_源码泄露分析_2026.md]]

## 所属目录
- [[README|sources/]] · [[../README|wiki/]]
