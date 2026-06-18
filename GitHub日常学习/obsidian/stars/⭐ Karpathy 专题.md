---
tags: [Karpathy, MOC]
created: 2026-06-18
---

# ⭐ Karpathy 学习专题

> Andrej Karpathy — OpenAI 创始成员、前 Tesla AI 总监 — 的教学仓库全集

---

## 🧭 学习路线图

```
第 1 步：micrograd         ← 100 行代码理解"什么是深度学习"
第 2 步：nn-zero-to-hero    ← 8 讲视频，从 micrograd 到 GPT
第 3 步：build-nanogpt      ← 从空文件一步步写出 GPT-2
第 4 步：nanoGPT            ← 极简 GPT 训练代码（300+300 行）
第 5 步：llm.c              ← 纯 C/CUDA 实现，看穿底层
```

## 📦 五个仓库全貌

| 仓库 | 定位 | 核心价值 |
|------|------|---------|
| [[learning/nn-zero-to-hero/_MyLearning/📖 内容摄取\|nn-zero-to-hero]] | 🎓 视频课程 | 8 讲 YouTube + Notebook，理论+代码 |
| [[learning/micrograd/_MyLearning/📖 内容摄取\|micrograd]] | 🧱 最小引擎 | 100 行 Autograd，理解反向传播本质 |
| [[learning/build-nanogpt/_MyLearning/📖 内容摄取\|build-nanogpt]] | 🔨 逐步构建 | 每个 commit 一个步骤，4 小时视频 |
| [[learning/nanoGPT/_MyLearning/📖 内容摄取\|nanoGPT]] | ⚡ 极简训练 | 600 行复现 GPT-2，~$10 训练一次 |
| [[learning/llm.c/_MyLearning/📖 内容摄取\|llm.c]] | 🔬 底层透视 | 纯 C/CUDA，比 PyTorch 快 7%，无黑箱 |

## 🎯 建议从哪开始

| 你的背景 | 推荐起点 |
|---------|---------|
| 零基础 | nn-zero-to-hero 第 1 讲 → micrograd |
| 会用 PyTorch 但不懂原理 | micrograd → backprop 手推 |
| 想理解 Transformer | nn-zero-to-hero 第 7 讲 → build-nanogpt |
| 想训练 GPT | nanoGPT（GPU）或 llm.c（C 爱好者） |
| 想彻底理解底层 | llm.c 的 train_gpt2.c（1000 行纯 C） |

## 🔗 社区资源
- [Zero To Hero Discord](https://discord.gg/3zy8kqD9Cp)
- [GPU MODE Discord](https://discord.gg/gpumode)（llm.c 社区）
- Karpathy YouTube: [@AndrejKarpathy](https://youtube.com/@AndrejKarpathy)
