---
name: "coding-interview-university"
full_name: "jwasham/coding-interview-university"
description: "A complete computer science study plan to become a software engineer."
url: "https://github.com/jwasham/coding-interview-university"
language: ""
stars: 352289
forks: 83563
topics: [computer-science, interview, programming-interviews, study-plan, data-structures, algorithms, software-engineering, algorithm, coding-interviews, interview-prep]
source_list: "learning"
starred_at: ""
created: 2026-06-16
tags: [github/stars, interview, algorithms, computer-science]
---

# coding-interview-university

> jwasham/coding-interview-university — ⭐ 352,289 stars

A complete computer science study plan to become a software engineer. 多个月的学习计划，从非 CS 背景到成为大厂软件工程师。

---

## 🎯 学习计划总览

建议每天 8-12 小时，持续 4 个月（或每天 4-6 小时，持续 8 个月）。

---

## 📚 第一阶段：预备知识

- 基础数学（算术、代数）
- 至少一门编程语言基础（Python / Java / C++）
- Markdown / Git 基础

---

## 📚 第二阶段：算法复杂度分析

### Big-O 表示法
```python
# O(1) - 常数时间
arr[0]

# O(log n) - 对数时间
二分查找

# O(n) - 线性时间
for x in arr: print(x)

# O(n log n) - 线性对数时间
归并排序、快速排序

# O(n²) - 平方时间
for x in arr:
    for y in arr: print(x, y)

# O(2ⁿ) - 指数时间
递归求斐波那契数列
```

**核心概念**：
- 时间复杂度和空间复杂度
- 最好、最坏、平均情况分析
- 主定理（Master Theorem）

---

## 📚 第三阶段：数据结构

### 1. 数组（Arrays）
```python
# 静态数组 vs 动态数组
arr = [1, 2, 3, 4, 5]
arr.append(6)  # 动态扩容
arr[2] = 10    # O(1) 随机访问
```

### 2. 链表（Linked Lists）
```python
class ListNode:
    def __init__(self, val=0, next=None):
        self.val = val
        self.next = next

# 操作：插入 O(1)、删除 O(1)、查找 O(n)
# 技巧：快慢指针、虚拟头节点
```

### 3. 栈（Stack）— LIFO
```python
stack = []
stack.append(1)    # push
stack.append(2)
top = stack.pop()  # pop → 2
```

### 4. 队列（Queue）— FIFO
```python
from collections import deque
queue = deque()
queue.append(1)    # 入队
queue.append(2)
front = queue.popleft()  # 出队 → 1
```

### 5. 哈希表（Hash Table）
```python
# 哈希函数 → 索引 → 冲突解决（链表法/开放地址法）
hashmap = {}
hashmap['key'] = 'value'  # 平均 O(1)
# 重点：负载因子、rehash、碰撞解决
```

### 6. 二叉树（Binary Tree）
```python
class TreeNode:
    def __init__(self, val=0, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

# 遍历方式
def inorder(root):       # 左-根-右
    if root:
        inorder(root.left)
        print(root.val)
        inorder(root.right)

def preorder(root):      # 根-左-右
    if root:
        print(root.val)
        preorder(root.left)
        preorder(root.right)

def postorder(root):     # 左-右-根
    if root:
        postorder(root.left)
        postorder(root.right)
        print(root.val)

# BST 特性：左<根<右, 中序遍历有序
```

### 7. 堆（Heap）
```python
import heapq
heap = []
heapq.heappush(heap, 3)  # 最小堆
heapq.heappush(heap, 1)
heapq.heappush(heap, 2)
print(heapq.heappop(heap))  # → 1

# 应用：Top K、中位数查找、Dijkstra
```

### 8. 并查集（Union-Find）
```python
class DSU:
    def __init__(self, n):
        self.parent = list(range(n))
        self.rank = [0] * n
    
    def find(self, x):
        # 路径压缩
        if self.parent[x] != x:
            self.parent[x] = self.find(self.parent[x])
        return self.parent[x]
    
    def union(self, x, y):
        # 按秩合并
        px, py = self.find(x), self.find(y)
        if px == py: return
        if self.rank[px] < self.rank[py]:
            self.parent[px] = py
        elif self.rank[px] > self.rank[py]:
            self.parent[py] = px
        else:
            self.parent[py] = px
            self.rank[px] += 1
```

### 9. 图（Graph）
```python
# 邻接表表示
graph = {
    'A': ['B', 'C'],
    'B': ['A', 'D', 'E'],
    'C': ['A', 'F'],
    'D': ['B'],
    'E': ['B', 'F'],
    'F': ['C', 'E']
}

# BFS - 最短路径
from collections import deque
def bfs(graph, start):
    visited = set([start])
    queue = deque([start])
    while queue:
        node = queue.popleft()
        for neighbor in graph[node]:
            if neighbor not in visited:
                visited.add(neighbor)
                queue.append(neighbor)

# DFS - 连通性、拓扑排序
def dfs(graph, node, visited):
    visited.add(node)
    for neighbor in graph[node]:
        if neighbor not in visited:
            dfs(graph, neighbor, visited)
```

### 10. 字典树（Trie）
```python
class TrieNode:
    def __init__(self):
        self.children = {}
        self.is_end = False

class Trie:
    def __init__(self):
        self.root = TrieNode()
    
    def insert(self, word):
        node = self.root
        for ch in word:
            if ch not in node.children:
                node.children[ch] = TrieNode()
            node = node.children[ch]
        node.is_end = True
    
    def search(self, word):
        node = self.root
        for ch in word:
            if ch not in node.children:
                return False
            node = node.children[ch]
        return node.is_end
```

---

## 📚 第四阶段：算法

### 排序算法
| 算法 | 最优 | 平均 | 最差 | 空间 | 稳定 |
|-----|------|------|------|------|------|
| 冒泡排序 | O(n) | O(n²) | O(n²) | O(1) | ✅ |
| 选择排序 | O(n²) | O(n²) | O(n²) | O(1) | ❌ |
| 插入排序 | O(n) | O(n²) | O(n²) | O(1) | ✅ |
| 归并排序 | O(n log n) | O(n log n) | O(n log n) | O(n) | ✅ |
| 快速排序 | O(n log n) | O(n log n) | O(n²) | O(log n) | ❌ |
| 堆排序 | O(n log n) | O(n log n) | O(n log n) | O(1) | ❌ |
| 计数排序 | O(n+k) | O(n+k) | O(n+k) | O(k) | ✅ |

### 动态规划（DP）
**核心思想**：重叠子问题 + 最优子结构

**经典问题**：
1. **斐波那契数列** — 一维 DP
   ```python
   def fib(n):
       if n <= 1: return n
       dp = [0] * (n + 1)
       dp[1] = 1
       for i in range(2, n + 1):
           dp[i] = dp[i-1] + dp[i-2]
       return dp[n]
   ```
2. **背包问题** — 二维 DP
3. **最长公共子序列（LCS）**
4. **最长递增子序列（LIS）**
5. **编辑距离（Edit Distance）**
6. **爬楼梯 / 不同路径**

### 图算法
- **Dijkstra** — 单源最短路径（正权边）
- **Bellman-Ford** — 单源最短路径（含负权边）
- **Floyd-Warshall** — 全源最短路径
- **A\*** — 启发式搜索
- **Kruskal / Prim** — 最小生成树
- **拓扑排序** — 有向无环图

---

## 📚 第五阶段：高级主题

### 系统设计
- **可扩展性**：垂直 vs 水平扩展
- **负载均衡**：Round Robin, 一致性 Hash
- **缓存**：Redis, CDN, 缓存策略（LRU, LFU）
- **数据库**：分库分表、读写分离、索引优化
- **消息队列**：Kafka, RabbitMQ
- **微服务**：服务拆分、API Gateway

### 面向对象设计
- SOLID 原则
- 设计模式：单例、工厂、观察者、策略
- 常见 OOD 题目：停车场设计、电梯设计

### 并发编程
- 线程 vs 进程 vs 协程
- 锁（互斥锁、读写锁）
- 死锁的四个条件与预防
- `synchronized` / `Lock` / `Semaphore`

---

## 📚 辅助资源

**推荐书籍**：
- 《Cracking the Coding Interview》
- 《Introduction to Algorithms》（CLRS）
- 《The Algorithm Design Manual》
- 《System Design Interview》

**刷题平台**：LeetCode, HackerRank, CodeSignal

**仓库提供的 Cheat Sheets**：
```
extras/cheat sheets/
├── big-o-cheatsheet.pdf       ← 大O速查表
├── python-cheat-sheet-v1.pdf  ← Python语法速查
├── Coding Interview Python Language Essentials.pdf
├── system-design.pdf          ← 系统设计速查
├── Java Fundamentals Cheatsheet.pdf
├── C Reference Card (ANSI) 2.2.pdf
├── Cpp_reference.pdf
├── STL Quick Reference 1.29.pdf
├── bits-cheat-sheet.pdf
└── git-cheat-sheet-education.pdf
```

> 💡 **完整内容**：主 README 包含极其详尽的学习计划（2000+ 行），extras/ 包含速查表格和翻译版本。访问 [GitHub 仓库](https://github.com/jwasham/coding-interview-university) 获取完整内容。

## 个人笔记

<!-- 在这里记录你的学习心得和笔记 -->

## 相关链接

- [[stars/learning/index|📚 全部星标仓库总览]]
