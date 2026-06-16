---
name: "hello-agents"
full_name: "datawhalechina/hello-agents"
description: "📚 《从零开始构建智能体》——从零开始的智能体原理与实践教程"
url: "https://github.com/datawhalechina/hello-agents"
language: "Python"
stars: 59437
forks: 7305
topics: [agent, tutorial, llm, rag]
source_list: "learning"
starred_at: ""
created: 2026-06-16
tags: [github/stars, ai, agent, llm, tutorial, 中文]
---

# hello-agents

> datawhalechina/hello-agents — ⭐ 59,437 stars

📚 《从零开始构建智能体》—— 从零开始的智能体原理与实践教程

---

## 📖 全书概览

**16 章**完整教程，覆盖从智能体基础概念到高级框架开发的完整知识体系。同时提供中英文双语版本。

---

## 🔬 第一章：初识智能体

### 1.1 什么是智能体？

智能体（Agent）被定义为：任何能够通过**传感器**感知环境，并**自主**地通过**执行器**采取**行动**以达成特定目标的实体。

**智能体的四个基本要素**：
- **环境（Environment）**— 智能体所处的外部世界
- **感知（Perception）**— 通过传感器感知环境状态
- **行动（Action）**— 通过执行器对环境施加影响
- **自主性（Autonomy）**— 基于感知和内部状态进行独立决策

### 1.1.1 传统智能体的演进

1. **简单反射智能体** — 条件-动作规则（如自动恒温器）
2. **基于模型的反射智能体** — 拥有内部世界模型，能追踪不可直接感知的状态
3. **基于目标的智能体** — 主动规划行为以达成特定目标（如 GPS 导航）
4. **基于效用的智能体** — 在冲突目标间权衡，最大化期望效用
5. **学习型智能体** — 通过强化学习与环境互动自主改进策略（如 AlphaGo）

### 1.1.2 LLM 驱动的新范式

与传统的差异：
| 维度 | 传统智能体 | LLM 智能体 |
|------|-----------|------------|
| 核心引擎 | 显式编程规则 | 大语言模型 |
| 知识来源 | 工程师构建 | 预训练数据 |
| 交互方式 | 结构化接口 | 自然语言 |
| 泛化能力 | 确定有边界 | 灵活涌现 |
| 推理能力 | 条件逻辑 | 思维链推理 |

**案例 — 智能旅行助手**：用户可以说"规划一次厦门之旅"，LLM Agent 会自动：
1. 将目标分解为子任务：确认偏好 → 查天气 → 制定行程 → 预订
2. 调用外部工具（天气 API、地图 API、预订 API）
3. 根据用户反馈动态修正（如"酒店超预算"→ 重新搜索）

### 1.1.3 智能体的类型

**按感知范围**：完全可观察 vs 部分可观察
**按环境确定性**：确定性 vs 随机性
**按智能体数量**：单智能体 vs 多智能体

---

## 📖 第二章：智能体发展史

回顾智能体从早期符号主义 AI 到现代 LLM Agent 的发展历程，包括：
- 专家系统时代（1960s-1980s）
- 行为主义与 Brooks 的包容架构（1990s）
- Web 智能体与信息检索
- 深度强化学习的突破（DQN, AlphaGo）
- 大语言模型驱动的智能体革命（2022-至今）

---

## 📖 第三章：大语言模型基础

### 3.1 Transformer 核心原理
- 自注意力机制（Self-Attention）
- 多头注意力（Multi-Head Attention）
- 位置编码（Positional Encoding）
- 编码器-解码器架构

### 3.2 预训练范式
- **GPT 系列**：自回归语言模型（从左到右预测）
- **BERT 系列**：掩码语言模型（完形填空）
- **T5**：文本到文本的统一框架

### 3.3 Prompt Engineering
- **零样本（Zero-shot）**：直接给出任务描述
- **少样本（Few-shot）**：提供几个示例后再提问
- **思维链（Chain-of-Thought）**：引导模型展示推理过程
- **指令微调（Instruction Tuning）**

**Prompt 示例**：
```
请判断以下评论的情感是正面还是负面：
评论：这部电影太精彩了，我已经看了三遍！
情感：正面

评论：桌子的一条腿是断的。
情感：
```

### 3.4 In-Context Learning
- 通过示例上下文学习，无需更新模型参数
- 示例数量和质量对效果的影响

---

## 📖 第四章：智能体经典范式构建

### 4.1 ReAct 模式（Reasoning + Acting）
核心思想：将**推理过程**和**行动执行**交替进行，让 LLM 在思考的同时采取行动。

**ReAct 循环**：
```
思考（Thought）→ 行动（Action）→ 观察（Observation）→ 思考（Thought）→ ...
```

**示例**：
```
问题：旧金山的温度是多少？
Thought: 我需要查询旧金山的天气信息。
Action: search_weather("San Francisco")
Observation: 旧金山当前温度 18°C，多云
Thought: 我现在可以回答用户的问题。
Answer: 旧金山的当前温度是 18°C，多云。
```

### 4.2 Plan-and-Solve 模式
- 先制定完整计划，再逐步执行
- 适用于需要长期规划的复杂任务

### 4.3 工具使用（Tool Use）
- Function Calling：将外部函数注册为工具
- 模型自主决定何时调用什么工具
- 工具结果作为观察反馈给模型

### 4.4 记忆系统
- **短期记忆**：上下文窗口内的信息（In-Context Learning）
- **长期记忆**：外部存储（向量数据库）
- **工作记忆**：当前任务相关的状态信息

---

## 📖 第五-八章：框架与开发实践

### 第五章：低代码平台搭建智能体
- Dify / Coze / FastGPT 平台使用
- 可视化工作流编排
- 插件与工具集成

### 第六章：框架开发实践（LangChain / LlamaIndex）
**LangChain 示例**：
```python
from langchain.agents import initialize_agent, Tool
from langchain.llms import OpenAI

# 定义工具
tools = [
    Tool(name="Search", func=search_function, 
         description="搜索信息"),
    Tool(name="Calculator", func=calc_function,
         description="数学计算")
]

# 创建 Agent
llm = OpenAI(temperature=0)
agent = initialize_agent(tools, llm, agent="zero-shot-react-description")
agent.run("计算 2+2 的结果")
```

### 第七章：构建你自己的 Agent 框架
- 核心架构设计
- 工具注册与调度
- 错误处理与重试机制

### 第八章：记忆与检索（RAG）
- **向量数据库**：ChromaDB, FAISS, Milvus
- **文档分块**：Chunk 策略（按段落、按语义）
- **检索增强**：相似度搜索 + 重排序

---

## 📖 第九-十六章：高级主题

### 第九章：多智能体系统
- 通信协议设计
- 任务分配与协作（Orchestrator-Worker）
- 共识与投票机制
- 案例分析：AutoGen, CrewAI

### 第十章：智能体安全与对齐
- Prompt Injection 防护
- 输出过滤与审核
- 行为边界约束

### 第十一-十二章：实战项目
1. **客户服务智能体** — 自动问答 + 工单创建
2. **代码助手智能体** — 代码生成 + 审查 + 重构
3. **数据分析智能体** — 数据查询 → 分析 → 可视化
4. **个人知识助手** — RAG + 对话 + 知识管理

### 第十三-十六章：部署与进阶
- 智能体服务化（FastAPI + Docker）
- 性能监控与日志追踪
- 生产环境最佳实践
- 前沿趋势：多模态 Agent、具身智能

---

## 💻 配套代码

`code/` 目录包含 16 个章节的完整代码实现：
```
code/
├── chapter1/   → 智能体基础示例
├── chapter2/   → 智能体发展史
├── chapter3/   → LLM 调用示例（通义千问、OpenAI、智谱）
├── chapter4/   → ReAct 模式实现
├── chapter5/   → 低代码平台搭建
├── chapter6/   → LangChain/LlamaIndex 开发
├── chapter7/   → 自定义 Agent 框架
├── chapter8/   → RAG 实现
├── chapter9/   → 多智能体系统
├── chapter10/  → 安全与对齐
├── chapter11-16/ → 实战项目
```

> 💡 **完整教程**：在 `docs/` 目录下包含详细的章节文档（中英文），`code/` 目录包含可运行的代码。访问 [GitHub 仓库](https://github.com/datawhalechina/hello-agents) 获取全部内容。

## 个人笔记

<!-- 在这里记录你的学习心得和笔记 -->

## 相关链接

- [[stars/learning/index|📚 全部星标仓库总览]]
- [[stars/learning/agency-agents|agency-agents]]
- [[stars/learning/dive-into-llms|dive-into-llms]]
