---
type: concept
tags:
  - obsidian
  - plugin
  - RAG
  - AI
summary: "Smart Connections — Obsidian 最流行的 RAG 对话插件，让 AI 与你的笔记对话"
sources:
  - "karpathy/wiki/sources/来源_Obsidian_AI_第二大腦指南_2026.md"
created: 2026-06-18
updated: 2026-06-18
---

# 概念_Smart_Connections

## 定义

Smart Connections 是 Obsidian 最受欢迎的 AI 插件，使用 RAG（检索增强生成）让用户可以与整个 vault 对话。支持本地模型（Ollama）或云端 API。

## 核心原理
1. 将 vault 中所有笔记索引为向量嵌入
2. 提问时检索最相关笔记
3. 将相关笔记作为上下文发送给 LLM
4. 返回基于「你的」知识的回答

## 与 LLM Wiki 的区别
Smart Connections 是 RAG 模式，LLM Wiki 是主动维护模式，两者互补。

## 关联概念
- [[概念_RAG检索增强生成]]
- [[概念_AI第二大脑]]
- [[概念_LLM_Wiki]]
