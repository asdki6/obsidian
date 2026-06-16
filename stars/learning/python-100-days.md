---
name: "Python-100-Days"
full_name: "jackfrued/Python-100-Days"
description: "Python - 100天从新手到大师"
url: "https://github.com/jackfrued/Python-100-Days"
language: "Jupyter Notebook"
stars: 183392
forks: 55665
topics: []
source_list: "learning"
starred_at: ""
created: 2026-06-16
tags: [github/stars, python, tutorial, 中文, 编程入门]
---

# Python-100-Days

> jackfrued/Python-100-Days — ⭐ 183,392 stars

作者：骆昊 (jackfrued) | 从零基础到 Python 大师的 100 天完整学习路线

---

## 📋 课程总览

包含 10 个阶段、100 天的 Python 教学，覆盖从基础语法到 AI 机器学习的完整知识体系。

---

## 📚 Day 01-20：Python 语言基础

### Day 01-03：初识 Python 与编程基础
**Python 简介**：Python 由吉多·范罗苏姆（Guido von Rossum）于1989年发明，是目前最受欢迎的编程语言之一。

**Python 特点**：
- 简单优雅，容易上手
- 开源，拥有强大的社区和生态圈
- 胶水语言，可以黏合其他语言
- 跨平台，可在多种操作系统上运行
- 缺点是执行效率低（解释型语言通病）

**第一个 Python 程序**：
```python
print('hello, world!')
```

**变量与类型**：
```python
# Python 中的变量不需要声明类型
a = 321
b = 12
print(a + b)    # 333
print(a - b)    # 309
print(a * b)    # 3852
print(a / b)    # 26.75

# type() 函数查看变量类型
print(type(a))  # <class 'int'>
```

### Day 04-05：分支与循环结构
**分支结构**：
```python
# if-elif-else 结构
x = float(input('x = '))
if x > 1:
    y = 3 * x - 5
elif x >= -1:
    y = x + 2
else:
    y = 5 * x + 3
print(f'f({x}) = {y}')
```

**循环结构**：
```python
# for-in 循环
sum = 0
for x in range(2, 101, 2):
    sum += x
print(sum)  # 2550 (2+4+...+100)

# while 循环
import random
answer = random.randint(1, 100)
counter = 0
while True:
    counter += 1
    guess = int(input('请输入你猜的数字: '))
    if guess < answer:
        print('大一点')
    elif guess > answer:
        print('小一点')
    else:
        print('恭喜你猜对了!')
        break
print(f'你总共猜了{counter}次')
```

### Day 06-07：函数与数据结构
**函数**：
```python
# 定义和调用函数
def add(a=0, b=0, c=0):
    return a + b + c

print(add(1, 2, 3))    # 6
print(add(1, 2))       # 3
print(add(a=10, c=20)) # 30
```

**常用数据结构**：
- **列表 list** - 可变序列，可存储任意类型
  ```python
  items = ['Python', 'Java', 'Go', 'Kotlin']
  items.append('Swift')
  items.pop(1)  # 移除 Java
  ```
- **元组 tuple** - 不可变序列
- **字符串 str** - 文本处理
- **集合 set** - 去重、交并补
- **字典 dict** - 键值对存储
  ```python
  scores = {'小明': 95, '小红': 88, '小刚': 78}
  for name, score in scores.items():
      print(f'{name}: {score}')
  ```

### Day 08-10：面向对象编程
```python
class Student:
    """学生类"""
    def __init__(self, name, age):
        self.name = name
        self.age = age
    
    def study(self, course):
        print(f'{self.name}正在学习{course}.')
    
    def play(self):
        print(f'{self.name}正在玩游戏.')

# 创建对象
stu1 = Student('小明', 18)
stu1.study('Python程序设计')
```

### Day 11-15：文件操作与正则
- **读写文件**：open(), with 语句
- **JSON/CSV/Excel 处理**
- **图像处理**：Pillow 库
- **正则表达式**：re 模块

### Day 16-20：进阶内容
- 生成式（推导式）：`[x**2 for x in range(1, 11)]`
- `heapq` 模块：最大/最小的N个元素
- `itertools` 模块：排列组合
- `collections` 模块：Counter, defaultdict, namedtuple
- 装饰器、迭代器、生成器

---

## 📚 Day 21-30：文件处理与常用库

- **Day 21**：文件读写与异常处理
- **Day 22**：对象序列化（pickle/json）
- **Day 23-25**：CSV/Excel 文件操作（openpyxl, xlrd）
- **Day 26**：Word/PPT 文件操作（python-docx）
- **Day 27**：PDF 文件操作（PyPDF2, pdfplumber）
- **Day 28**：图像处理（Pillow 库 — 缩放、裁剪、滤镜等）
- **Day 29**：发送邮件和短信
- **Day 30**：正则表达式

---

## 📚 Day 31-35：Python 进阶与 Linux

**Day 31 - Python 语言进阶**：
```python
# 生成式（推导式）
prices = {'AAPL': 191.88, 'GOOG': 1186.96, 'IBM': 149.24}
# 筛选价格大于100的股票
prices2 = {k: v for k, v in prices.items() if v > 100}

# heapq 堆排序
import heapq
list1 = [34, 25, 12, 99, 87, 63, 58, 78, 88, 92]
print(heapq.nlargest(3, list1))  # [99, 92, 88]
print(heapq.nsmallest(3, list1)) # [12, 25, 34]
```

**Day 32-33**：Web 前端入门（HTML/CSS/JS/Vue.js）
**Day 34-35**：Linux 操作系统（基本命令、VIM、环境搭建）

---

## 📚 Day 36-45：数据库

- **Day 36-37**：关系型数据库与 MySQL 概述、DDL
- **Day 38-39**：DML（增删改）、DQL（查询）
- **Day 40**：DCL（用户权限管理）
- **Day 41**：MySQL 新特性
- **Day 42**：视图、函数和存储过程
- **Day 43**：索引优化
- **Day 44**：Python 操作 MySQL（PyMySQL）
- **Day 45**：Hive 实战
- **扩展**：Redis、MongoDB

---

## 📚 Day 46-60：Django Web 框架

**Day 46**：Django 快速上手
```python
# pip install django
# django-admin startproject demo
# python manage.py runserver

# views.py
from django.http import HttpResponse

def hello(request):
    return HttpResponse('Hello, Django!')
```

**Day 47-48**：模型、静态资源与 Ajax
**Day 49**：Cookie 和 Session
**Day 50**：制作报表
**Day 51-52**：日志、调试工具栏、中间件
**Day 53-55**：前后端分离、DRF（Django REST Framework）
**Day 56-57**：缓存（Redis）与三方平台接入
**Day 58-60**：异步任务（Celery）、单元测试、项目上线

---

## 📚 Day 61-80：爬虫与数据分析

### Day 61-65：网络爬虫
1. **网络数据采集概述**
2. **urllib/requests 库** - 获取网络资源
3. **Beautiful Soup / lxml** - HTML 解析
4. **Python 并发编程** - 多线程、多进程、协程
5. **Selenium** - 动态内容抓取
6. **Scrapy** - 爬虫框架

### Day 66-80：数据分析与可视化
- **NumPy** - 高性能科学计算
  ```python
  import numpy as np
  arr = np.array([1, 2, 3, 4, 5])
  print(arr.mean())  # 3.0
  print(arr.sum())   # 15
  ```
- **Pandas** - 数据处理分析
  ```python
  import pandas as pd
  df = pd.read_csv('data.csv')
  df.describe()       # 统计摘要
  df.groupby('city').mean()  # 分组聚合
  ```
- **Matplotlib / Seaborn** - 数据可视化
  ```python
  import matplotlib.pyplot as plt
  plt.plot([1, 2, 3, 4], [1, 4, 9, 16])
  plt.show()
  ```

---

## 📚 Day 81-100：机器学习与项目实战

### Day 81-90：机器学习
1. 机器学习概述
2. K 最近邻（KNN）算法
3. 决策树与随机森林
4. 朴素贝叶斯
5. 回归模型（线性回归、逻辑回归）
6. K-Means 聚类
7. 集成学习（AdaBoost, XGBoost）
8. 神经网络基础
9. NLP 入门
10. 机器学习实战项目

### Day 91-100：项目与部署
- Docker 容器化
- MySQL 性能优化
- RESTful API 设计
- 电商网站技术要点
- 自动化测试
- 项目部署上线
- 面试准备

---

## 📁 仓库结构

```
Day01-20/     → Python 基础语法（20节）
Day21-30/     → 文件/办公自动化（10节）
Day31-35/     → 进阶 + Web前端 + Linux（5节）
Day36-45/     → 数据库（10节）
Day46-60/     → Django Web开发（15节）
Day61-65/     → 网络爬虫（5节）
Day66-80/     → 数据分析与可视化（15节）
Day81-90/     → 机器学习（10节）
Day91-100/    → 项目实战与部署（10节）
res/          → 资源文件
公开课/       → 配套视频课程
番外篇/       → 扩展主题
```

> 💡 **全部教学内容**：每个 .md 文件都是完整的教程文章，包含代码示例、示意图和实践练习。完整内容请访问：[GitHub 仓库](https://github.com/jackfrued/Python-100-Days)

## 个人笔记

<!-- 在这里记录你的学习心得和笔记 -->

## 相关链接

- [[stars/learning/index|📚 全部星标仓库总览]]
