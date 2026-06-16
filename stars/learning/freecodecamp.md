---
name: "freeCodeCamp"
full_name: "freeCodeCamp/freeCodeCamp"
description: "freeCodeCamp.org's open-source codebase and curriculum. Learn math, programming, and computer science for free."
url: "https://github.com/freeCodeCamp/freeCodeCamp"
language: "TypeScript"
stars: 447872
forks: 44989
topics: [learn-to-code, nonprofits, programming, nodejs, react, d3, careers, education, teachers, javascript]
source_list: "learning"
starred_at: ""
created: 2026-06-16
tags: [github/stars, education, programming, freecodecamp]
---

# freeCodeCamp

> freeCodeCamp/freeCodeCamp — ⭐ 447,872 stars

freeCodeCamp.org 的开源代码库和课程体系。免费学习数学、编程和计算机科学。

---

## 🎓 认证体系（30+ 认证）

每个认证包含约 300 小时的学习内容和 5 个实战项目。

### 1️⃣ 响应式 Web 设计（Responsive Web Design）
- **技术栈**：HTML5, CSS3, Flexbox, CSS Grid
- **项目**：个人作品集、调查表单、产品落地页、技术文档页、个人主页
- ⭐ 推荐入门第一站

### 2️⃣ JavaScript 算法与数据结构
- **技术栈**：JavaScript, ES6+, 正则表达式, OOP, 数据结构
- **项目**：回文检查器、罗马数字转换器、凯撒密码、电话号码验证器、现金收银机
- ⭐ 编程基础核心

### 3️⃣ 前端库（Front End Libraries）
- **技术栈**：React, Redux, jQuery, Bootstrap, Sass
- **项目**：Markdown 预览器、Drum Machine、计算器、番茄时钟、随机语录机

### 4️⃣ 数据可视化（Data Visualization）
- **技术栈**：D3.js, JSON, AJAX
- **项目**：条形图、散点图、热力图、等高线图、Tree Map

### 5️⃣ 后端开发与 API（Backend Development and APIs）
- **技术栈**：Node.js, Express, MongoDB, Mongoose
- **项目**：时间戳微服务、请求头解析器、URL 缩短器、运动追踪器、文件元数据微服务

### 6️⃣ 质量保证（Quality Assurance）
- **技术栈**：Chai, Mocha, 单元测试, 功能测试
- **项目**：指标转换器、问题追踪器、个人图书馆、Sudoku 求解器、American-British 翻译器

### 7️⃣ Python 科学计算（Scientific Computing with Python）
- **技术栈**：Python, 代数
- **项目**：算术格式化器、时间计算器、Budget App、多边形面积计算器、概率计算器

### 8️⃣ Python 数据分析（Data Analysis with Python）
- **技术栈**：Python, NumPy, Pandas, Matplotlib, Seaborn
- **项目**：人口统计数据分析、医学数据可视化、海平面预测

### 9️⃣ 信息安全（Information Security）
- **技术栈**：HelmetJS, Python 安全
- **项目**：股票价格检查器、匿名消息板、端口扫描器、SHA-1 破解器、安全实时多人游戏

### 🔟 Python 机器学习（Machine Learning with Python）
- **技术栈**：TensorFlow, Scikit-learn, 神经网络
- **项目**：石头剪刀布、猫狗分类器、图书推荐引擎、线性回归健康预测器、神经网络短信分类器

### 1️⃣1️⃣ College Algebra with Python
- 代数概念 + Python 实现
- **项目**：算术格式化器、时间计算器、Budget App、多边形面积计算器、概率计算器

### 1️⃣2️⃣ A2 English for Developers
- 面向开发者的英语课程
- 覆盖技术文档阅读、代码审查交流、会议沟通等场景

### 1️⃣3️⃣ Foundational C# with Microsoft
- **技术栈**：C#, .NET
- 与 Microsoft 合作开发的 C# 基础认证

---

## 🗂️ 课程体系结构

```
curriculum/challenges/english/
├── certifications/
│   ├── responsive-web-design.yml       ← 课程大纲定义
│   ├── javascript-algorithms-and-data-structures.yml
│   ├── front-end-development-libraries.yml
│   ├── data-visualization.yml
│   ├── back-end-development-and-apis.yml
│   ├── quality-assurance.yml
│   ├── scientific-computing-with-python.yml
│   ├── data-analysis-with-python.yml
│   ├── information-security.yml
│   ├── machine-learning-with-python.yml
│   ├── college-algebra-with-python.yml
│   ├── a2-english-for-developers.yml
│   ├── foundational-c-sharp-with-microsoft.yml
│   └── ... (含旧版和新版)

├── blocks/               ← 每个认证中的模块/块
│   ├── responsive-web-design/
│   ├── javascript-algorithms/
│   └── ... 
```

每个 `.yml` 文件定义了课程的完整大纲：模块结构、课程顺序、项目要求等。

---

## 🛠️ 技术栈

| 层级 | 技术 |
|------|------|
| **前端** | React, TypeScript, Tailwind CSS |
| **后端** | Node.js, Express |
| **数据库** | MongoDB |
| **测试** | Cypress, Playwright, Jest |
| **工具** | Turbororepo, Vite, Vitest |

---

## 📁 项目结构

```
curriculum/             → 课程内容（核心！）
├── challenges/         → 挑战题目
│   └── english/        → 英文版课程
├── schema/             → 数据模式定义
├── src/                → 课程工具代码
├── dictionaries/       → 多语言字典
├── i18n-curriculum/    → 国际化课程
└── structure/          → 课程结构配置

api/                    → API 服务器
client/                 → React 客户端应用
shared/                 → 共享工具库
tools/                  → 构建和部署工具
```

> 💡 **全部教学内容**：`curriculum/challenges/` 包含数千个交互式编程挑战的源码。每个挑战包含：说明文档、初始代码、测试用例。访问 [freeCodeCamp.org](https://www.freecodecamp.org) 可在线学习，或克隆仓库本地学习。

## 个人笔记

<!-- 在这里记录你的学习心得和笔记 -->

## 相关链接

- [[stars/learning/index|📚 全部星标仓库总览]]
- [[stars/learning/project-based-learning|project-based-learning]]
