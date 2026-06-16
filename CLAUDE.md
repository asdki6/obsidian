# Obsidian Vault (GitHub)

这是主 Obsidian 笔记库，纳入 Git 版本控制。

## 核心信息

- **Vault 路径**: `C:\Users\PC\Documents\GitHub\obsidian`
- **版本控制**: Git (已配置 `.gitignore`)
- **Obsidian 插件**:
  - `obsidian-git` — Git 同步
  - `realclaudian` — Claude AI 集成

## 已启用的核心功能

- 日记 (Daily Notes)、模板 (Templates)、画布 (Canvas)
- 关系图谱 (Graph)、反向链接 (Backlinks)、标签面板 (Tags)
- 属性/元数据 (Properties)、书签 (Bookmarks)
- 同步 (Sync)、文件恢复 (File Recovery)
- Bases (数据库视图)

## 笔记规范

- 使用 Obsidian 标准 Markdown 格式
- 内部链接使用 `[[wikilink]]` 语法
- 标签使用 `#tag/subtag` 格式
- 元数据使用 YAML frontmatter (`---` 包裹)
- 附件和图片放在对应笔记的同名子文件夹或 `attachments/` 目录

## 与 Claude Code 协作

- 本文件为 Claude Code 提供 vault 上下文
- `.claude/` 目录存放 Claude Code 的技能、子代理和命令
- `.claudian/` 目录为 realclaudian 插件配置
- 可直接通过 Claude Code 在此目录下创建、编辑、搜索笔记
