---
name: "dive-into-llms"
full_name: "Lordog/dive-into-llms"
description: "《动手学大模型Dive into LLMs》系列编程实践教程"
url: "https://github.com/Lordog/dive-into-llms"
language: "Jupyter Notebook"
stars: 40921
forks: 4986
topics: []
source_list: "learning"
starred_at: ""
created: 2026-06-16
tags: [github/stars, llm, deep-learning, tutorial, 中文]
---

# dive-into-llms

> Lordog/dive-into-llms — ⭐ 40,921 stars

《动手学大模型（Dive into LLMs）》系列编程实践教程 — 从代码中深度学习大模型技术

---

## 📖 教程结构

共 **11 章**，每章包含：**README 文档 + Jupyter Notebook 代码 + PDF 讲义**

---

## 🏗️ 第一章：预训练语言模型微调与部署

### 1.1 工具准备：Transformers

使用 Hugging Face Transformers 库进行预训练模型的加载、微调和部署。

**安装**：
```bash
conda create -n llm python=3.9
conda activate llm
pip install transformers
conda install pytorch  # GPU版本
```

### 1.2 微调示例：文本分类（虚假新闻检测）

**数据准备**：Kaggle 虚假推文数据集
**模型选择**：BERT / RoBERTa / DistilBERT

**微调代码框架**：
```python
from transformers import (
    AutoTokenizer, AutoModelForSequenceClassification,
    Trainer, TrainingArguments
)

# 加载预训练模型和分词器
model_name = "bert-base-chinese"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForSequenceClassification.from_pretrained(
    model_name, num_labels=2
)

# 准备训练数据
train_encodings = tokenizer(train_texts, truncation=True, padding=True)
    
# 配置训练参数
training_args = TrainingArguments(
    output_dir="./results",
    num_train_epochs=3,
    per_device_train_batch_size=16,
    evaluation_strategy="epoch",
    save_strategy="epoch",
)

# 训练
trainer = Trainer(
    model=model,
    args=training_args,
    train_dataset=train_dataset,
    eval_dataset=eval_dataset,
)
trainer.train()
```

### 1.3 模型推理与部署
- 使用 Pipeline API 快速推理
- Gradio Spaces 构建交互式 Demo
- 模型导出与服务化

---

## 🏗️ 第二章：大模型提示学习与思维链

### 2.1 LLM API 调用

以**通义千问（Qwen）**为例：
```python
import dashscope

# 普通调用
response = dashscope.Generation.call(
    model='qwen-turbo',
    prompt='用萝卜、土豆、茄子做饭，给我个菜谱。'
)
print(response.output.text)

# 流式调用
responses = dashscope.Generation.call(
    model='qwen-turbo',
    prompt='讲一个有趣的冷笑话',
    stream=True
)
for response in responses:
    print(response.output.text, end='')
```

**其他可用的 API**：OpenAI、智谱 GLM、文心一言、百川

### 2.2 提示工程技巧

**零样本（Zero-shot）**：
```
将以下句子翻译成英文：今天天气真好。
```

**少样本（Few-shot）**：
```
问题：1+1=？
答案：2
问题：3+4=？
答案：7
问题：5+2=？
答案：
```

**思维链（Chain-of-Thought, CoT）**：
```
问题：小明有 5 个苹果，小红有 3 个苹果，他们总共有多少个苹果？
推理：小明有5个苹果，小红有3个苹果，所以总共是 5+3=8 个苹果。
答案：8
```

**自洽性（Self-Consistency）**：多次采样 → 取最一致的回答

### 2.3 高级提示技巧
- **角色扮演**：让模型扮演特定角色
- **格式控制**：指定输出格式（JSON/表格/列表）
- **Few-shot 选择**：动态选择相似的示例

---

## 🏗️ 第三-五章：模型编辑、数学推理与水印

### 第三章：模型编辑
- 知识编辑技术：修改预训练模型中的特定知识
- 模型编辑方法：KE、MEND、ROME

**Notebook**: `dive_edit.ipynb`

### 第四章：数学推理
- 数学问题求解的 prompting 策略
- 工具增强的数学推理

**Notebook**: `sft_math.ipynb`

### 第五章：LLM 水印
- 文本水印技术原理
- 检测与验证方法

**Notebook**: `watermark.ipynb`

---

## 🏗️ 第六-八章：安全、多模态与越狱

### 第六章：对抗攻击与越狱（Jailbreak）
- Prompt Injection 攻击类型
- 越狱提示词示例与防护
- 红队测试方法论

**Notebook**: `dive-jailbreak.ipynb`

### 第七章：隐写术（Steganography）
- LLM 文本隐写的原理
- 编解码方法

**Notebook**: `llm_stega.ipynb`

### 第八章：多模态大模型（MLLM）
- CLIP、BLIP、LLaVA 架构
- 图文理解与生成
- 多模态 Agent

**Notebook**: `mllms.ipynb`

---

## 🏗️ 第九-十一章：Agent、安全与 RLHF

### 第九章：GUI Agent
- 图形界面自动化 Agent
- 屏幕理解与操作

**Notebook**: `GUIagent.ipynb`

### 第十章：LLM 安全与 Agent
- 智能体安全问题
- 工具调用安全
- 数据隐私保护

### 第十一章：RLHF（基于人类反馈的强化学习）
- RLHF 原理：SFT → Reward Model → PPO
- DPO（Direct Preference Optimization）

**Notebook**: `RLHF.ipynb`

```python
# RLHF 流程示意
# Step 1: SFT - 监督微调
# Step 2: 训练 Reward Model
# Step 3: PPO 强化学习优化
#     - 策略模型生成回答
#     - Reward Model 评分
#     - PPO 更新策略
```

---

## 📁 完整仓库结构

```
documents/
├── chapter1/  → 微调与部署 (dive-tuning.ipynb)
├── chapter2/  → 提示学习 (dive-prompting.ipynb)
├── chapter3/  → 模型编辑 (dive_edit.ipynb)
├── chapter4/  → 数学推理 (sft_math.ipynb)
├── chapter5/  → 文本水印 (watermark.ipynb)
├── chapter6/  → 越狱攻击 (dive-jailbreak.ipynb)
├── chapter7/  → 隐写术 (llm_stega.ipynb)
├── chapter8/  → 多模态模型 (mllms.ipynb)
├── chapter9/  → GUI Agent (GUIagent.ipynb)
├── chapter10/ → 安全与Agent (agent.ipynb)
└── chapter11/ → RLHF (RLHF.ipynb)
```

> 💡 **全部教学内容**：每个 chapter 包含 README（教程文档）+ Jupyter Notebook（可运行代码）+ PDF（讲义）。访问 [GitHub 仓库](https://github.com/Lordog/dive-into-llms) 获取完整内容。

## 个人笔记

<!-- 在这里记录你的学习心得和笔记 -->

## 相关链接

- [[stars/learning/index|📚 全部星标仓库总览]]
- [[stars/learning/hello-agents|hello-agents]]
