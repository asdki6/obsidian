# raw/ — 原始来源层

> 📌 只读不可变。LLM 从此层读取但不修改。这是你的真实来源（source of truth）。

## 子目录与分类规则

| 来源类型 | 存放位置 | 命名格式 | 示例 |
|----------|----------|----------|------|
| 网页文章、博客 | `articles/<主题>/` | `来源_主题_年份.md` | `articles/ai/NxCode_Obsidian_AI_第二大腦指南_2026.md` |
| 书籍笔记、微信读书 | `books/<类型>/` | `书名.md` | `books/fiction/白鹿原.md` |
| 研究论文、报告 | `papers/<领域>/` | `作者_年份_标题.md` | `papers/ai/Vaswani_2017_Attention.md` |
| 图片、截图、图表 | `media/<类型>/` | 描述性文件名 | `media/diagrams/架构图.png` |
| Obsidian 下载附件 | `assets/` | 自动生成 | Obsidian 绑定快捷键自动下载 |

---

## 子分类

### articles/ — 网页文章、博客

| 目录 | 覆盖范围 |
|------|----------|
| `ai/` | AI、大模型、机器学习、深度学习 |
| `tech/` | 技术、编程、工程、架构（非 AI 类） |
| `methodology/` | 方法论、思维框架、知识管理、效率 |
| `business/` | 商业、创业、产品、营销、管理 |
| `psychology/` | 心理学、认知科学、行为科学、神经科学 |
| `philosophy/` | 哲学、思想史、伦理学 |
| `design/` | 设计、UX、用户体验、视觉设计 |
| `health/` | 健康、医学、生物、营养 |
| `finance/` | 投资、经济、理财、金融 |
| `society/` | 社会、政治、历史、文化、教育 |
| `science/` | 物理、数学、化学、自然科学 |

### books/ — 书籍笔记、微信读书划线

| 目录 | 覆盖范围 |
|------|----------|
| `fiction/` | 小说、文学 |
| `non-fiction/` | 散文、随笔、纪实 |
| `tech/` | 技术、编程、计算机 |
| `business/` | 商业、管理、经济、投资 |
| `psychology/` | 心理学、自我提升、认知 |
| `philosophy/` | 哲学、思想 |
| `biography/` | 传记、回忆录、人物 |
| `science/` | 自然科学、科普 |
| `history/` | 历史、文明 |

### papers/ — 学术论文、研究报告

| 目录 | 覆盖范围 |
|------|----------|
| `ai/` | AI、机器学习、NLP、CV |
| `cs/` | 计算机科学、系统、网络 |
| `cognitive-science/` | 认知科学、心理学 |
| `other/` | 其他领域 |

### media/ — 图片、截图、图表

| 目录 | 覆盖范围 |
|------|----------|
| `images/` | 图片、插图 |
| `screenshots/` | 屏幕截图 |
| `diagrams/` | 图表、架构图、流程图 |
| `photos/` | 照片 |

### assets/ — Obsidian 下载附件
Obsidian 绑定快捷键自动下载，无需手动管理。
