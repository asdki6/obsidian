---
type: entity
tags:
  - karpathy
  - deep-learning
  - open-source
  - education
summary: "Andrej Karpathy的开源教学项目系列——从micrograd到nanoGPT到llm.c，以最简代码讲透深度学习核心"
sources:
  - "karpathy/wiki/sources/来源_GitHub_Stars_build-your-own-x.md"
created: 2026-06-18
updated: 2026-06-18
---

# 实体_Karpathy_系列项目

## 基本信息
- **类型**：开源项目系列
- **作者**：Andrej Karpathy
- **理念**：用最简洁的代码解释最核心的原理

## 项目列表

| 项目 | 核心教学点 | 代码量 |
|------|-----------|:------:|
| **micrograd** | 自动微分引擎原理 | ~150行 |
| **nanoGPT** | GPT 模型训练全流程 | ~300行 |
| **llm.c** | 纯 C 语言实现 LLM 训练 | ~1000行 |
| **nn-zero-to-hero** | 神经网络从零到精通系列教程 | 配套视频 |
| **build-nanogpt** | 视频教程：跟着写一个 GPT | 视频系列 |

## 学习建议

从 micrograd 到 llm.c 的递进路径：
```
micrograd → nn-zero-to-hero → nanoGPT → llm.c
  (引擎)      (神经网络)       (GPT)     (纯C)
```

## 与 build-your-own-x 的关系

Karpathy 的系列项目是 `build-your-own-x` 哲学的最佳范例——不是读论文，而是自己写一遍。

## 关联概念
- [[../../concepts/learning/概念_项目驱动学习]]
- [[../../concepts/ai-km/概念_LLM_Wiki]]

## 所属目录
- [[../../entities/README|entities/]] · [[../../../README|wiki/]]
