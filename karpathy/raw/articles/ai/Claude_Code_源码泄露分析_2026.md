# Claude Code 源码泄露事件分析

> 日期：2026-03-31
> 发现者：Chaofan Shou (@Fried_rice)
> 原因：npm 打包错误，source map 暴露了未混淆源码

## 事件概述

Anthropic 的 CLI 工具 Claude Code 的完整 TypeScript 源码因 npm 打包失误被公开。版本 `@anthropic-ai/claude-code@2.1.88` 的 `.npmignore` 未排除 source map 文件（`main.js.map`），导致可追溯到 R2 存储桶中的 TypeScript 源码。Anthropic 确认这是"人为发布打包错误，非安全漏洞"。

## 泄露规模

| 指标 | 数值 |
|------|------|
| TypeScript/TSX 文件 | ~1,900 |
| 代码行数 | 512,000+ |
| Agent 工具 | 40+ |
| Slash 命令 | 85+ |
| React/Ink UI 组件 | ~140 |
| Feature Flags | 44-108 |

## 重大发现

### BUDDY — 虚拟伙伴
未发布的 AI 宠物功能：18 种物种（鸭子、龙、蝾螈、水豚等），5 个属性（DEBUGGING、PATIENCE、CHAOS、WISDOM、SNARK），基于用户 ID 哈希分配。

### KAIROS — 自主 Agent
未发布的持久化助手：主动监控和行动、每日追加日志、夜间"做梦"整理记忆、当前仅内部 feature flag 控制。

### Undercover Mode
Anthropic 员工自动触发：注入"永远不要提及你是 AI"的系统提示、从 git commit 剥离 Co-Authored-By 标记。

### 未发布工具
ULTRAPLAN（30 分钟规划）、Coordinator Mode（多 Agent 并行+邮箱）、VOICE_MODE、WEB_BROWSER_TOOL、DAEMON 后台进程。

## 技术架构

- 语言：TypeScript 6.0+，运行时：Bun → Node.js ≥18
- 终端 UI：React + Ink，验证：Zod
- 核心：QueryEngine.ts（~46,000 行）
- 三层上下文压缩：reactive → micro → trimmed

## 来源
- https://github.com/tornikeo/claude-code
- https://github.com/chauncygu/collection-claude-code-source-code
- https://wavespeed.ai/blog/posts/claude-code-leaked-source-hidden-features/
