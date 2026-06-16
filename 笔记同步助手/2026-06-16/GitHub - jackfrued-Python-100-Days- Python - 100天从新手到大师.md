---
author: unknown
source: GitHub
url: https://github.com/jackfrued/Python-100-Days.git
saved: 2026-06-16 15:30:15
tags:
  - 笔记同步助手
id: 75b6b9db-01ac-49d0-b6f3-ec54f929eee9
---

> **作者**：骆昊
> 
> **说明**：如果访问 GitHub 比较慢的话，可以关注我的知乎账号（[**Python-Jack**](https://www.zhihu.com/people/jackfrued)），上面的[“**从零开始学Python**”](https://zhuanlan.zhihu.com/c_1216656665569013760)专栏（对应本项目前 20 天的内容）比较适合初学者，其他的专栏如“[**数据思维和统计思维**](https://www.zhihu.com/column/c_1620074540456964096)”、“[**基于Python的数据分析**](https://www.zhihu.com/column/c_1217746527315496960)”、“[**说走就走的AI之旅**](https://www.zhihu.com/column/c_1628900668109946880)”等也在持续更新中，欢迎大家关注、点赞和评论。目前免费的 QQ 交流群已经人满为患，消息太杂乱也没有办法一一回复，如果有一起打卡学习或付费咨询的需求，可以加入付费交流群，新用户可以通过下方二维码付费之后添加我的私人微信（微信号：**jackfrued**），然后邀请大家进入付费学习打卡群，添加微信时请备注好自己的称呼和需求，我会为大家提供力所能及的帮助。
> 
> ![[笔记同步助手/images/a363f4eee52cce122d8d1af6073bace1_MD5.png|Image]]
> 
> 本项目对应的部分视频已经同步到 [Bilibili](https://space.bilibili.com/1177252794)，有兴趣的小伙伴可以点赞、投币、关注，一键三连支持一下！

### Python应用领域和职业发展分析

[](#python应用领域和职业发展分析)

简单的说，Python是一个“优雅”、“明确”、“简单”的编程语言。

-   学习曲线低，非专业人士也能上手
-   开源系统，拥有强大的生态圈
-   解释型语言，完美的平台可移植性
-   动态类型语言，支持面向对象和函数式编程
-   代码规范程度高，可读性强

Python在以下领域都有用武之地。

-   后端开发 - Python / Java / Go / PHP
-   DevOps - Python / Shell / Ruby
-   数据采集 - Python / C++ / Java
-   量化交易 - Python / C++ / R
-   数据科学 - Python / R / Julia / Matlab
-   机器学习 - Python / R / C++ / Julia
-   自动化测试 - Python / Shell

作为一名Python开发者，根据个人的喜好和职业规划，可以选择的就业领域也非常多。

-   Python后端开发工程师（服务器、云平台、数据接口）
-   Python运维工程师（自动化运维、SRE、DevOps）
-   Python数据分析师（数据分析、商业智能、数字化运营）
-   Python数据科学家（机器学习、深度学习、算法专家）
-   Python爬虫工程师（不推荐此赛道！！！）
-   Python测试工程师（自动化测试、测试开发）

> **说明**：目前，**数据科学赛道是非常热门的方向**，因为不管是互联网行业还是传统行业都已经积累了大量的数据，各行各业都需要数据科学家从已有的数据中发现更多的商业价值，从而为企业的决策提供数据的支撑，这就是所谓的数据驱动决策。

给初学者的几个建议：

-   **Make English as your working language.** （让英语成为你的工作语言）
-   **Practice makes perfect.** （熟能生巧）
-   **All experience comes from the mistakes you've made.** （所有的经验都源于犯过的错误）
-   **Don't be a freeloader.** （学会分享，不要只当伸手党）
-   **Embrace AI to boost your productivity.**（拥抱AI，提升效率）

### Day01～20 - Python语言基础

[](#day0120---python语言基础)

#### Day01 - [初识Python](/jackfrued/Python-100-Days/blob/master/Day01-20/01.%E5%88%9D%E8%AF%86Python.md)

[](#day01---初识python)

1.  Python简介
    -   Python编年史
    -   Python优缺点
    -   Python应用领域
2.  安装Python环境
    -   Windows环境
    -   macOS环境

#### Day02 - [第一个Python程序](/jackfrued/Python-100-Days/blob/master/Day01-20/02.%E7%AC%AC%E4%B8%80%E4%B8%AAPython%E7%A8%8B%E5%BA%8F.md)

[](#day02---第一个python程序)

1.  编写代码的工具
2.  你好世界
3.  注释你的代码

#### Day03 - [Python语言中的变量](/jackfrued/Python-100-Days/blob/master/Day01-20/03.Python%E8%AF%AD%E8%A8%80%E4%B8%AD%E7%9A%84%E5%8F%98%E9%87%8F.md)

[](#day03---python语言中的变量)

1.  一些常识
2.  变量和类型
3.  变量命名
4.  变量的使用

#### Day04 - [Python语言中的运算符](/jackfrued/Python-100-Days/blob/master/Day01-20/04.Python%E8%AF%AD%E8%A8%80%E4%B8%AD%E7%9A%84%E8%BF%90%E7%AE%97%E7%AC%A6.md)

[](#day04---python语言中的运算符)

1.  算术运算符
2.  赋值运算符
3.  比较运算符和逻辑运算符
4.  运算符和表达式应用
    -   华氏和摄氏温度转换
    -   计算圆的周长和面积
    -   判断闰年

#### Day05 - [分支结构](/jackfrued/Python-100-Days/blob/master/Day01-20/05.%E5%88%86%E6%94%AF%E7%BB%93%E6%9E%84.md)

[](#day05---分支结构)

1.  使用if和else构造分支结构
2.  使用match和case构造分支结构
3.  分支结构的应用
    -   分段函数求值
    -   百分制成绩转换成等级
    -   计算三角形的周长和面积

#### Day06 - [循环结构](/jackfrued/Python-100-Days/blob/master/Day01-20/06.%E5%BE%AA%E7%8E%AF%E7%BB%93%E6%9E%84.md)

[](#day06---循环结构)

1.  for-in循环
2.  while循环
3.  break和continue
4.  嵌套的循环结构
5.  循环结构的应用
    -   判断素数
    -   最大公约数
    -   猜数字游戏

#### Day07 - [分支和循环结构实战](/jackfrued/Python-100-Days/blob/master/Day01-20/07.%E5%88%86%E6%94%AF%E5%92%8C%E5%BE%AA%E7%8E%AF%E7%BB%93%E6%9E%84%E5%AE%9E%E6%88%98.md)

[](#day07---分支和循环结构实战)

1.  例子1：100以内的素数
2.  例子2：斐波那契数列
3.  例子3：寻找水仙花数
4.  例子4：百钱百鸡问题
5.  例子5：CRAPS赌博游戏

#### Day08 - [常用数据结构之列表-1](/jackfrued/Python-100-Days/blob/master/Day01-20/08.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E5%88%97%E8%A1%A8-1.md)

[](#day08---常用数据结构之列表-1)

1.  创建列表
2.  列表的运算
3.  元素的遍历

#### Day09 - [常用数据结构之列表-2](/jackfrued/Python-100-Days/blob/master/Day01-20/09.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E5%88%97%E8%A1%A8-2.md)

[](#day09---常用数据结构之列表-2)

1.  列表的方法
    -   添加和删除元素
    -   元素位置和频次
    -   元素排序和反转
2.  列表生成式
3.  嵌套列表
4.  列表的应用

#### Day10 - [常用数据结构之元组](/jackfrued/Python-100-Days/blob/master/Day01-20/10.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E5%85%83%E7%BB%84.md)

[](#day10---常用数据结构之元组)

1.  元组的定义和运算
2.  打包和解包操作
3.  交换变量的值
4.  元组和列表的比较

#### Day11 - [常用数据结构之字符串](/jackfrued/Python-100-Days/blob/master/Day01-20/11.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E5%AD%97%E7%AC%A6%E4%B8%B2.md)

[](#day11---常用数据结构之字符串)

1.  字符串的定义
    -   转义字符
    -   原始字符串
    -   字符的特殊表示
2.  字符串的运算
    -   拼接和重复
    -   比较运算
    -   成员运算
    -   获取字符串长度
    -   索引和切片
3.  字符的遍历
4.  字符串的方法
    -   大小写相关操作
    -   查找操作
    -   性质判断
    -   格式化
    -   修剪操作
    -   替换操作
    -   拆分与合并
    -   编码与解码
    -   其他方法

#### Day12 - [常用数据结构之集合](/jackfrued/Python-100-Days/blob/master/Day01-20/12.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E9%9B%86%E5%90%88.md)

[](#day12---常用数据结构之集合)

1.  创建集合
2.  元素的变量
3.  集合的运算
    -   成员运算
    -   二元运算
    -   比较运算
4.  集合的方法
5.  不可变集合

#### Day13 - [常用数据结构之字典](/jackfrued/Python-100-Days/blob/master/Day01-20/13.%E5%B8%B8%E7%94%A8%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B9%8B%E5%AD%97%E5%85%B8.md)

[](#day13---常用数据结构之字典)

1.  创建和使用字典
2.  字典的运算
3.  字典的方法
4.  字典的应用

#### Day14 - [函数和模块](/jackfrued/Python-100-Days/blob/master/Day01-20/14.%E5%87%BD%E6%95%B0%E5%92%8C%E6%A8%A1%E5%9D%97.md)

[](#day14---函数和模块)

1.  定义函数
2.  函数的参数
    -   位置参数和关键字参数
    -   参数的默认值
    -   可变参数
3.  用模块管理函数
4.  标准库中的模块和函数

#### Day15 - [函数应用实战](/jackfrued/Python-100-Days/blob/master/Day01-20/15.%E5%87%BD%E6%95%B0%E5%BA%94%E7%94%A8%E5%AE%9E%E6%88%98.md)

[](#day15---函数应用实战)

1.  例子1：随机验证码
2.  例子2：判断素数
3.  例子3：最大公约数和最小公倍数
4.  例子4：数据统计
5.  例子5：双色球随机选号

#### Day16 - [函数使用进阶](/jackfrued/Python-100-Days/blob/master/Day01-20/16.%E5%87%BD%E6%95%B0%E4%BD%BF%E7%94%A8%E8%BF%9B%E9%98%B6.md)

[](#day16---函数使用进阶)

1.  高阶函数
2.  Lambda函数
3.  偏函数

#### Day17 - [函数高级应用](/jackfrued/Python-100-Days/blob/master/Day01-20/17.%E5%87%BD%E6%95%B0%E9%AB%98%E7%BA%A7%E5%BA%94%E7%94%A8.md)

[](#day17---函数高级应用)

1.  装饰器
2.  递归调用

#### Day18 - [面向对象编程入门](/jackfrued/Python-100-Days/blob/master/Day01-20/18.%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8B%E5%85%A5%E9%97%A8.md)

[](#day18---面向对象编程入门)

1.  类和对象
2.  定义类
3.  创建和使用对象
4.  初始化方法
5.  面向对象的支柱
6.  面向对象案例
    -   例子1：数字时钟
    -   例子2：平面上的点

#### Day19 - [面向对象编程进阶](/jackfrued/Python-100-Days/blob/master/Day01-20/19.%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8B%E8%BF%9B%E9%98%B6.md)

[](#day19---面向对象编程进阶)

1.  可见性和属性装饰器
2.  动态属性
3.  静态方法和类方法
4.  继承和多态

#### Day20 - [面向对象编程应用](/jackfrued/Python-100-Days/blob/master/Day01-20/20.%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8B%E5%BA%94%E7%94%A8.md)

[](#day20---面向对象编程应用)

1.  扑克游戏
2.  工资结算系统

### Day21～30 - Python语言应用

[](#day2130---python语言应用)

#### Day21 - [文件读写和异常处理](/jackfrued/Python-100-Days/blob/master/Day21-30/21.%E6%96%87%E4%BB%B6%E8%AF%BB%E5%86%99%E5%92%8C%E5%BC%82%E5%B8%B8%E5%A4%84%E7%90%86.md)

[](#day21---文件读写和异常处理)

1.  打开和关闭文件
2.  读写文本文件
3.  异常处理机制
4.  上下文管理器语法
5.  读写二进制文件

#### Day22 - [对象的序列化和反序列化](/jackfrued/Python-100-Days/blob/master/Day21-30/22.%E5%AF%B9%E8%B1%A1%E7%9A%84%E5%BA%8F%E5%88%97%E5%8C%96%E5%92%8C%E5%8F%8D%E5%BA%8F%E5%88%97%E5%8C%96.md)

[](#day22---对象的序列化和反序列化)

1.  JSON概述
2.  读写JSON格式的数据
3.  包管理工具pip
4.  使用网络API获取数据

#### Day23 - [Python读写CSV文件](/jackfrued/Python-100-Days/blob/master/23.Python%E8%AF%BB%E5%86%99CSV%E6%96%87%E4%BB%B6.md)

[](#day23---python读写csv文件)

1.  CSV文件介绍
2.  将数据写入CSV文件
3.  从CSV文件读取数据

#### Day24 - [Python读写Excel文件-1](/jackfrued/Python-100-Days/blob/master/Day21-30/24.%E7%94%A8Python%E8%AF%BB%E5%86%99Excel%E6%96%87%E4%BB%B6-1.md)

[](#day24---python读写excel文件-1)

1.  Excel简介
2.  读Excel文件
3.  写Excel文件
4.  调整样式
5.  公式计算

#### Day25 - [Python读写Excel文件-2](/jackfrued/Python-100-Days/blob/master/Day21-30/25.Python%E8%AF%BB%E5%86%99Excel%E6%96%87%E4%BB%B6-2.md)

[](#day25---python读写excel文件-2)

1.  Excel简介
2.  读Excel文件
3.  写Excel文件
4.  调整样式
5.  生成统计图表

#### Day26 - [Python操作Word和PowerPoint文件](/jackfrued/Python-100-Days/blob/master/Day21-30/26.Python%E6%93%8D%E4%BD%9CWord%E5%92%8CPowerPoint%E6%96%87%E4%BB%B6.md)

[](#day26---python操作word和powerpoint文件)

1.  操作Word文档
2.  生成PowerPoint

#### Day27 - [Python操作PDF文件](/jackfrued/Python-100-Days/blob/master/Day21-30/27.Python%E6%93%8D%E4%BD%9CPDF%E6%96%87%E4%BB%B6.md)

[](#day27---python操作pdf文件)

1.  从PDF中提取文本
2.  旋转和叠加页面
3.  加密PDF文件
4.  批量添加水印
5.  创建PDF文件

#### Day28 - [Python处理图像](/jackfrued/Python-100-Days/blob/master/Day21-30/28.Python%E5%A4%84%E7%90%86%E5%9B%BE%E5%83%8F.md)

[](#day28---python处理图像)

1.  入门知识
2.  用Pillow处理图像
3.  使用Pillow绘图

#### Day29 - [Python发送邮件和短信](/jackfrued/Python-100-Days/blob/master/Day21-30/29.Python%E5%8F%91%E9%80%81%E9%82%AE%E4%BB%B6%E5%92%8C%E7%9F%AD%E4%BF%A1.md)

[](#day29---python发送邮件和短信)

1.  发送电子邮件
2.  发送短信

#### Day30 - [正则表达式的应用](/jackfrued/Python-100-Days/blob/master/Day21-30/30.%E6%AD%A3%E5%88%99%E8%A1%A8%E8%BE%BE%E5%BC%8F%E7%9A%84%E5%BA%94%E7%94%A8.md)

[](#day30---正则表达式的应用)

1.  正则表达式相关知识
2.  Python对正则表达式的支持
    -   例子1：输入验证
    -   例子2：内容提取
    -   例子3：内容替换
    -   例子4：长句拆分

### Day31～35 - 其他相关内容

[](#day3135---其他相关内容)

#### [Python语言进阶](/jackfrued/Python-100-Days/blob/master/Day31-35/31.Python%E8%AF%AD%E8%A8%80%E8%BF%9B%E9%98%B6.md)

[](#python语言进阶)

1.  重要知识点
2.  数据结构和算法
3.  函数的使用方式
4.  面向对象相关知识
5.  迭代器和生成器
6.  并发编程

#### [Web前端入门](/jackfrued/Python-100-Days/blob/master/Day31-35/32-33.Web%E5%89%8D%E7%AB%AF%E5%85%A5%E9%97%A8.md)

[](#web前端入门)

1.  用HTML标签承载页面内容
2.  用CSS渲染页面
3.  用JavaScript处理交互式行为
4.  Vue.js入门
5.  Element的使用
6.  Bootstrap的使用

#### [玩转Linux操作系统](/jackfrued/Python-100-Days/blob/master/Day31-35/34-35.%E7%8E%A9%E8%BD%ACLinux%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F.md)

[](#玩转linux操作系统)

1.  操作系统发展史和Linux概述
2.  Linux基础命令
3.  Linux中的实用程序
4.  Linux的文件系统
5.  Vim编辑器的应用
6.  环境变量和Shell编程
7.  软件的安装和服务的配置
8.  网络访问和管理
9.  其他相关内容

### Day36～45 - 数据库基础和进阶

[](#day3645---数据库基础和进阶)

#### Day36 - [关系型数据库和MySQL概述](/jackfrued/Python-100-Days/blob/master/Day36-45/36.%E5%85%B3%E7%B3%BB%E5%9E%8B%E6%95%B0%E6%8D%AE%E5%BA%93%E5%92%8CMySQL%E6%A6%82%E8%BF%B0.md)

[](#day36---关系型数据库和mysql概述)

1.  关系型数据库概述
2.  MySQL简介
3.  安装MySQL
4.  MySQL基本命令

#### Day37 - [SQL详解之DDL](/jackfrued/Python-100-Days/blob/master/Day36-45/37.SQL%E8%AF%A6%E8%A7%A3%E4%B9%8BDDL.md)

[](#day37---sql详解之ddl)

1.  建库建表
2.  删除表和修改表

#### Day38 - [SQL详解之DML](/jackfrued/Python-100-Days/blob/master/Day36-45/38.SQL%E8%AF%A6%E8%A7%A3%E4%B9%8BDML.md)

[](#day38---sql详解之dml)

1.  insert操作
2.  delete操作
3.  update操作

#### Day39 - [SQL详解之DQL](/jackfrued/Python-100-Days/blob/master/Day36-45/39.SQL%E8%AF%A6%E8%A7%A3%E4%B9%8BDQL.md)

[](#day39---sql详解之dql)

1.  投影和别名
2.  筛选数据
3.  空值处理
4.  去重
5.  排序
6.  聚合函数
7.  嵌套查询
8.  分组操作
9.  表连接
    -   笛卡尔积
    -   内连接
    -   自然连接
    -   外连接
10.  窗口函数
     -   定义窗口
     -   排名函数
     -   取数函数

#### Day40 - [SQL详解之DCL](/jackfrued/Python-100-Days/blob/master/Day36-45/40.SQL%E8%AF%A6%E8%A7%A3%E4%B9%8BDCL.md)

[](#day40---sql详解之dcl)

1.  创建用户
2.  授予权限
3.  召回权限

#### Day41 - [MySQL新特性](/jackfrued/Python-100-Days/blob/master/Day36-45/41.MySQL%E6%96%B0%E7%89%B9%E6%80%A7.md)

[](#day41---mysql新特性)

-   JSON类型
-   窗口函数
-   公共表表达式

#### Day42 - [视图、函数和过程](/jackfrued/Python-100-Days/blob/master/Day36-45/42.%E8%A7%86%E5%9B%BE%E3%80%81%E5%87%BD%E6%95%B0%E5%92%8C%E8%BF%87%E7%A8%8B.md)

[](#day42---视图函数和过程)

1.  视图
    -   使用场景
    -   创建视图
    -   使用限制
2.  函数
    -   内置函数
    -   用户自定义函数（UDF）
3.  过程
    -   创建过程
    -   调用过程

#### Day43 - [索引](/jackfrued/Python-100-Days/blob/master/Day36-45/43.%E7%B4%A2%E5%BC%95.md)

[](#day43---索引)

1.  执行计划
2.  索引的原理
3.  创建索引
    -   普通索引
    -   唯一索引
    -   前缀索引
    -   复合索引
4.  注意事项

#### Day44 - [Python接入MySQL数据库](/jackfrued/Python-100-Days/blob/master/Day36-45/44.Python%E6%8E%A5%E5%85%A5MySQL%E6%95%B0%E6%8D%AE%E5%BA%93.md)

[](#day44---python接入mysql数据库)

1.  安装三方库
2.  创建连接
3.  获取游标
4.  执行SQL语句
5.  通过游标抓取数据
6.  事务提交和回滚
7.  释放连接
8.  编写ETL脚本

#### Day45 - [Hive实战](/jackfrued/Python-100-Days/blob/master/Day36-45/45.Hive%E5%AE%9E%E6%88%98.md)

[](#day45---hive实战)

1.  Hive概述
2.  环境搭建
3.  常用命令
4.  基本语法
5.  建表操作
6.  写入数据
7.  常用函数
8.  分组聚合
9.  抽样操作
10.  排序操作
11.  横向展开
12.  性能优化

### Day46～60 - 实战Django

[](#day4660---实战django)

#### Day46 - [Django快速上手](/jackfrued/Python-100-Days/blob/master/Day46-60/46.Django%E5%BF%AB%E9%80%9F%E4%B8%8A%E6%89%8B.md)

[](#day46---django快速上手)

1.  Web应用工作机制
2.  HTTP请求和响应
3.  Django框架概述
4.  5分钟快速上手

#### Day47 - [深入模型](/jackfrued/Python-100-Days/blob/master/Day46-60/47.%E6%B7%B1%E5%85%A5%E6%A8%A1%E5%9E%8B.md)

[](#day47---深入模型)

1.  关系型数据库配置
2.  使用ORM完成对模型的CRUD操作
3.  管理后台的使用
4.  Django模型最佳实践
5.  模型定义参考

#### Day48 - [静态资源和Ajax请求](/jackfrued/Python-100-Days/blob/master/Day46-60/48.%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90%E5%92%8CAjax%E8%AF%B7%E6%B1%82.md)

[](#day48---静态资源和ajax请求)

1.  加载静态资源
2.  Ajax概述
3.  用Ajax实现投票功能

#### Day49 - [Cookie和Session](/jackfrued/Python-100-Days/blob/master/Day46-60/49.Cookie%E5%92%8CSession.md)

[](#day49---cookie和session)

1.  实现用户跟踪
2.  cookie和session的关系
3.  Django框架对session的支持
4.  视图函数中的cookie读写操作

#### Day50 - [报表和日志](/jackfrued/Python-100-Days/blob/master/Day46-60/50.%E5%88%B6%E4%BD%9C%E6%8A%A5%E8%A1%A8.md)

[](#day50---报表和日志)

1.  通过`HttpResponse`修改响应头
2.  使用`StreamingHttpResponse`处理大文件
3.  使用`xlwt`生成Excel报表
4.  使用`reportlab`生成PDF报表
5.  使用ECharts生成前端图表

#### Day51 - [日志和调试工具栏](/jackfrued/Python-100-Days/blob/master/Day46-60/51.%E6%97%A5%E5%BF%97%E5%92%8C%E8%B0%83%E8%AF%95%E5%B7%A5%E5%85%B7%E6%A0%8F.md)

[](#day51---日志和调试工具栏)

1.  配置日志
2.  配置Django-Debug-Toolbar
3.  优化ORM代码

#### Day52 - [中间件的应用](/jackfrued/Python-100-Days/blob/master/Day46-60/52.%E4%B8%AD%E9%97%B4%E4%BB%B6%E7%9A%84%E5%BA%94%E7%94%A8.md)

[](#day52---中间件的应用)

1.  什么是中间件
2.  Django框架内置的中间件
3.  自定义中间件及其应用场景

#### Day53 - [前后端分离开发入门](/jackfrued/Python-100-Days/blob/master/Day46-60/53.%E5%89%8D%E5%90%8E%E7%AB%AF%E5%88%86%E7%A6%BB%E5%BC%80%E5%8F%91%E5%85%A5%E9%97%A8.md)

[](#day53---前后端分离开发入门)

1.  返回JSON格式的数据
2.  用Vue.js渲染页面

#### Day54 - [RESTful架构和DRF入门](/jackfrued/Python-100-Days/blob/master/Day46-60/54.RESTful%E6%9E%B6%E6%9E%84%E5%92%8CDRF%E5%85%A5%E9%97%A8.md)

[](#day54---restful架构和drf入门)

1.  REST概述
2.  DRF库使用入门
3.  前后端分离开发
4.  JWT的应用

#### Day55 - [RESTful架构和DRF进阶](/jackfrued/Python-100-Days/blob/master/Day46-60/55.RESTful%E6%9E%B6%E6%9E%84%E5%92%8CDRF%E8%BF%9B%E9%98%B6.md)

[](#day55---restful架构和drf进阶)

1.  使用CBV
2.  数据分页
3.  数据筛选

#### Day56 - [使用缓存](/jackfrued/Python-100-Days/blob/master/Day46-60/56.%E4%BD%BF%E7%94%A8%E7%BC%93%E5%AD%98.md)

[](#day56---使用缓存)

1.  网站优化第一定律
2.  在Django项目中使用Redis提供缓存服务
3.  在视图函数中读写缓存
4.  使用装饰器实现页面缓存
5.  为数据接口提供缓存服务

#### Day57 - [接入三方平台](/jackfrued/Python-100-Days/blob/master/Day46-60/57.%E6%8E%A5%E5%85%A5%E4%B8%89%E6%96%B9%E5%B9%B3%E5%8F%B0.md)

[](#day57---接入三方平台)

1.  文件上传表单控件和图片文件预览
2.  服务器端如何处理上传的文件

#### Day58 - [异步任务和定时任务](/jackfrued/Python-100-Days/blob/master/Day46-60/58.%E5%BC%82%E6%AD%A5%E4%BB%BB%E5%8A%A1%E5%92%8C%E5%AE%9A%E6%97%B6%E4%BB%BB%E5%8A%A1.md)

[](#day58---异步任务和定时任务)

1.  网站优化第二定律
2.  配置消息队列服务
3.  在项目中使用Celery实现任务异步化
4.  在项目中使用Celery实现定时任务

#### Day59 - [单元测试](/jackfrued/Python-100-Days/blob/master/Day46-60/59.%E5%8D%95%E5%85%83%E6%B5%8B%E8%AF%95.md)

[](#day59---单元测试)

#### Day60 - [项目上线](/jackfrued/Python-100-Days/blob/master/Day46-60/60.%E9%A1%B9%E7%9B%AE%E4%B8%8A%E7%BA%BF.md)

[](#day60---项目上线)

1.  Python中的单元测试
2.  Django框架对单元测试的支持
3.  使用版本控制系统
4.  配置和使用uWSGI
5.  动静分离和Nginx配置
6.  配置HTTPS
7.  配置域名解析

### Day61～65 - 网络数据采集

[](#day6165---网络数据采集)

#### Day61 - [网络数据采集概述](/jackfrued/Python-100-Days/blob/master/Day61-65/61.%E7%BD%91%E7%BB%9C%E6%95%B0%E6%8D%AE%E9%87%87%E9%9B%86%E6%A6%82%E8%BF%B0.md)

[](#day61---网络数据采集概述)

1.  网络爬虫的概念及其应用领域
2.  网络爬虫的合法性探讨
3.  开发网络爬虫的相关工具
4.  一个爬虫程序的构成

#### Day62 - 数据抓取和解析

[](#day62---数据抓取和解析)

1.  [使用`requests`三方库实现数据抓取](/jackfrued/Python-100-Days/blob/master/Day61-65/62.%E7%94%A8Python%E8%8E%B7%E5%8F%96%E7%BD%91%E7%BB%9C%E8%B5%84%E6%BA%90-1.md)
2.  [页面解析的三种方式](/jackfrued/Python-100-Days/blob/master/Day61-65/62.%E7%94%A8Python%E8%A7%A3%E6%9E%90HTML%E9%A1%B5%E9%9D%A2-2.md)
    -   正则表达式解析
    -   XPath解析
    -   CSS选择器解析

#### Day63 - Python中的并发编程

[](#day63---python中的并发编程)

1.  [多线程](/jackfrued/Python-100-Days/blob/master/Day61-65/63.Python%E4%B8%AD%E7%9A%84%E5%B9%B6%E5%8F%91%E7%BC%96%E7%A8%8B-1.md)
2.  [多进程](/jackfrued/Python-100-Days/blob/master/Day61-65/63.Python%E4%B8%AD%E7%9A%84%E5%B9%B6%E5%8F%91%E7%BC%96%E7%A8%8B-2.md)
3.  [异步I/O](/jackfrued/Python-100-Days/blob/master/Day61-65/63.Python%E4%B8%AD%E7%9A%84%E5%B9%B6%E5%8F%91%E7%BC%96%E7%A8%8B-3.md)

#### Day64 - [使用Selenium抓取网页动态内容](/jackfrued/Python-100-Days/blob/master/Day61-65/64.%E4%BD%BF%E7%94%A8Selenium%E6%8A%93%E5%8F%96%E7%BD%91%E9%A1%B5%E5%8A%A8%E6%80%81%E5%86%85%E5%AE%B9.md)

[](#day64---使用selenium抓取网页动态内容)

1.  安装Selenium
2.  加载页面
3.  查找元素和模拟用户行为
4.  隐式等待和显示等待
5.  执行JavaScript代码
6.  Selenium反爬破解
7.  设置无头浏览器

#### Day65 - [爬虫框架Scrapy简介](/jackfrued/Python-100-Days/blob/master/Day61-65/65.%E7%88%AC%E8%99%AB%E6%A1%86%E6%9E%B6Scrapy%E7%AE%80%E4%BB%8B.md)

[](#day65---爬虫框架scrapy简介)

1.  Scrapy核心组件
2.  Scrapy工作流程
3.  安装Scrapy和创建项目
4.  编写蜘蛛程序
5.  编写中间件和管道程序
6.  Scrapy配置文件

### Day66～80 - Python数据分析

[](#day6680---python数据分析)

#### Day66 - [数据分析概述](/jackfrued/Python-100-Days/blob/master/Day66-80/66.%E6%95%B0%E6%8D%AE%E5%88%86%E6%9E%90%E6%A6%82%E8%BF%B0.md)

[](#day66---数据分析概述)

1.  数据分析师的职责
2.  数据分析师的技能栈
3.  数据分析相关库

#### Day67 - [环境准备](/jackfrued/Python-100-Days/blob/master/Day66-80/67.%E7%8E%AF%E5%A2%83%E5%87%86%E5%A4%87.md)

[](#day67---环境准备)

1.  安装和使用anaconda
    -   conda相关命令
2.  安装和使用jupyter-lab
    -   安装和启动
    -   使用小技巧

#### Day68 - [NumPy的应用-1](/jackfrued/Python-100-Days/blob/master/Day66-80/68.NumPy%E7%9A%84%E5%BA%94%E7%94%A8-1.md)

[](#day68---numpy的应用-1)

1.  创建数组对象
2.  数组对象的属性
3.  数组对象的索引运算
    -   普通索引
    -   花式索引
    -   布尔索引
    -   切片索引
4.  案例：使用数组处理图像

#### Day69 - [NumPy的应用-2](/jackfrued/Python-100-Days/blob/master/Day66-80/69.NumPy%E7%9A%84%E5%BA%94%E7%94%A8-2.md)

[](#day69---numpy的应用-2)

1.  数组对象的相关方法
    -   获取描述性统计信息
    -   其他相关方法

#### Day70 - [NumPy的应用-3](/jackfrued/Python-100-Days/blob/master/Day66-80/70.NumPy%E7%9A%84%E5%BA%94%E7%94%A8-3.md)

[](#day70---numpy的应用-3)

1.  数组的运算
    -   数组跟标量的运算
    -   数组跟数组的运算
2.  通用一元函数
3.  通用二元函数
4.  广播机制
5.  Numpy常用函数

#### Day71 - [NumPy的应用-4](/jackfrued/Python-100-Days/blob/master/Day66-80/71.NumPy%E7%9A%84%E5%BA%94%E7%94%A8-4.md)

[](#day71---numpy的应用-4)

1.  向量
2.  行列式
3.  矩阵
4.  多项式

#### Day72 - [深入浅出pandas-1](/jackfrued/Python-100-Days/blob/master/Day66-80/72.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-1.md)

[](#day72---深入浅出pandas-1)

1.  创建Series对象
2.  Series对象的运算
3.  Series对象的属性和方法

#### Day73 - [深入浅出pandas-2](/jackfrued/Python-100-Days/blob/master/Day66-80/73.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-2.md)

[](#day73---深入浅出pandas-2)

1.  创建DataFrame对象
2.  DataFrame对象的属性和方法
3.  读写DataFrame中的数据

#### Day74 - [深入浅出pandas-3](/jackfrued/Python-100-Days/blob/master/Day66-80/74.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-3.md)

[](#day74---深入浅出pandas-3)

1.  数据重塑
    -   数据拼接
    -   数据合并
2.  数据清洗
    -   缺失值
    -   重复值
    -   异常值
    -   预处理

#### Day75 - [深入浅出pandas-4](/jackfrued/Python-100-Days/blob/master/Day66-80/75.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-4.md)

[](#day75---深入浅出pandas-4)

1.  数据透视
    -   获取描述性统计信息
    -   排序和头部值
    -   分组聚合
    -   透视表和交叉表
2.  数据呈现

#### Day76 - [深入浅出pandas-5](/jackfrued/Python-100-Days/blob/master/Day66-80/76.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-5.md)

[](#day76---深入浅出pandas-5)

1.  计算同比环比
2.  窗口计算
3.  相关性判定

#### Day77 - [深入浅出pandas-6](/jackfrued/Python-100-Days/blob/master/Day66-80/77.%E6%B7%B1%E5%85%A5%E6%B5%85%E5%87%BApandas-6.md)

[](#day77---深入浅出pandas-6)

1.  索引的使用
    -   范围索引
    -   分类索引
    -   多级索引
    -   间隔索引
    -   日期时间索引

#### Day78 - [数据可视化-1](/jackfrued/Python-100-Days/blob/master/Day66-80/78.%E6%95%B0%E6%8D%AE%E5%8F%AF%E8%A7%86%E5%8C%96-1.md)

[](#day78---数据可视化-1)

1.  安装和导入matplotlib
2.  创建画布
3.  创建坐标系
4.  绘制图表
    -   折线图
    -   散点图
    -   柱状图
    -   饼状图
    -   直方图
    -   箱线图
5.  显示和保存图表

#### Day79 - [数据可视化-2](/jackfrued/Python-100-Days/blob/master/Day66-80/79.%E6%95%B0%E6%8D%AE%E5%8F%AF%E8%A7%86%E5%8C%96-2.md)

[](#day79---数据可视化-2)

1.  高阶图表
    -   气泡图
    -   面积图
    -   雷达图
    -   玫瑰图
    -   3D图表

#### Day80 - [数据可视化-3](/jackfrued/Python-100-Days/blob/master/Day66-80/80.%E6%95%B0%E6%8D%AE%E5%8F%AF%E8%A7%86%E5%8C%96-3.md)

[](#day80---数据可视化-3)

1.  Seaborn
2.  Pyecharts

### Day81～90 - 机器学习

[](#day8190---机器学习)

#### Day81 - [浅谈机器学习](/jackfrued/Python-100-Days/blob/master/Day81-90/81.%E6%B5%85%E8%B0%88%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0.md)

[](#day81---浅谈机器学习)

1.  人工智能发展史
2.  什么是机器学习
3.  机器学习应用领域
4.  机器学习的分类
5.  机器学习的步骤
6.  第一次机器学习

#### Day82 - [k最近邻算法](/jackfrued/Python-100-Days/blob/master/Day81-90/82.k%E6%9C%80%E8%BF%91%E9%82%BB%E7%AE%97%E6%B3%95.md)

[](#day82---k最近邻算法)

1.  距离的度量
2.  数据集介绍
3.  kNN分类的实现
4.  模型评估
5.  参数调优
6.  kNN回归的实现

#### Day83 - [决策树和随机森林](/jackfrued/Python-100-Days/blob/master/Day81-90/83.%E5%86%B3%E7%AD%96%E6%A0%91%E5%92%8C%E9%9A%8F%E6%9C%BA%E6%A3%AE%E6%9E%97.md)

[](#day83---决策树和随机森林)

1.  决策树的构建
    -   特征选择
    -   数据分裂
    -   树的剪枝
2.  实现决策树模型
3.  随机森林概述

#### Day84 - [朴素贝叶斯算法](/jackfrued/Python-100-Days/blob/master/Day81-90/84.%E6%9C%B4%E7%B4%A0%E8%B4%9D%E5%8F%B6%E6%96%AF%E7%AE%97%E6%B3%95.md)

[](#day84---朴素贝叶斯算法)

1.  贝叶斯定理
2.  朴素贝叶斯
3.  算法原理
    -   训练阶段
    -   预测阶段
    -   代码实现
4.  算法优缺点

#### Day85 - [回归模型](/jackfrued/Python-100-Days/blob/master/Day81-90/85.%E5%9B%9E%E5%BD%92%E6%A8%A1%E5%9E%8B.md)

[](#day85---回归模型)

1.  回归模型的分类
2.  回归系数的计算
3.  新数据集介绍
4.  线性回归代码实现
5.  回归模型的评估
6.  引入正则化项
7.  线性回归另一种实现
8.  多项式回归
9.  逻辑回归

#### Day86 - [K-Means聚类算法](/jackfrued/Python-100-Days/blob/master/Day81-90/86.K-Means%E8%81%9A%E7%B1%BB%E7%AE%97%E6%B3%95.md)

[](#day86---k-means聚类算法)

1.  算法原理
2.  数学描述
3.  代码实现

#### Day87 - [集成学习算法](/jackfrued/Python-100-Days/blob/master/Day81-90/87.%E9%9B%86%E6%88%90%E5%AD%A6%E4%B9%A0%E7%AE%97%E6%B3%95.md)

[](#day87---集成学习算法)

1.  算法分类
2.  AdaBoost
3.  GBDT
4.  XGBoost
5.  LightGBM

#### Day88 - [神经网络模型](/jackfrued/Python-100-Days/blob/master/Day81-90/88.%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%E6%A8%A1%E5%9E%8B.md)

[](#day88---神经网络模型)

1.  基本构成
2.  工作原理
3.  代码实现
4.  模型优缺点

#### Day89 - [自然语言处理入门](/jackfrued/Python-100-Days/blob/master/Day81-90/89.%E8%87%AA%E7%84%B6%E8%AF%AD%E8%A8%80%E5%A4%84%E7%90%86%E5%85%A5%E9%97%A8.md)

[](#day89---自然语言处理入门)

1.  词袋模型
2.  词向量
3.  NPLM和RNN
4.  Seq2Seq
5.  Transformer

#### Day90 - [机器学习实战](/jackfrued/Python-100-Days/blob/master/Day81-90/90.%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E5%AE%9E%E6%88%98.md)

[](#day90---机器学习实战)

1.  数据探索
2.  特征工程
3.  模型训练
4.  模型评估
5.  模型部署

### Day91～99 - [团队项目开发](/jackfrued/Python-100-Days/blob/master/Day91-100)

[](#day9199---团队项目开发)

#### 第91天：[团队项目开发的问题和解决方案](/jackfrued/Python-100-Days/blob/master/Day91-100/91.%E5%9B%A2%E9%98%9F%E9%A1%B9%E7%9B%AE%E5%BC%80%E5%8F%91%E7%9A%84%E9%97%AE%E9%A2%98%E5%92%8C%E8%A7%A3%E5%86%B3%E6%96%B9%E6%A1%88.md)

[](#第91天团队项目开发的问题和解决方案)

1.  软件过程模型
    
    -   经典过程模型（瀑布模型）
        
        -   可行性分析（研究做还是不做），输出《可行性分析报告》。
        -   需求分析（研究做什么），输出《需求规格说明书》和产品界面原型图。
        -   概要设计和详细设计，输出概念模型图（ER图）、物理模型图、类图、时序图等。
        -   编码 / 测试。
        -   上线 / 维护。
        
        瀑布模型最大的缺点是无法拥抱需求变化，整套流程结束后才能看到产品，团队士气低落。
        
    -   敏捷开发（Scrum）- 产品所有者、Scrum Master、研发人员 - Sprint
        
        -   产品的Backlog（用户故事、产品原型）。
        -   计划会议（评估和预算）。
        -   日常开发（站立会议、番茄工作法、结对编程、测试先行、代码重构……）。
        -   修复bug（问题描述、重现步骤、测试人员、被指派人）。
        -   发布版本。
        -   评审会议（Showcase，用户需要参与）。
        -   回顾会议（对当前迭代周期做一个总结）。
        
        > 补充：敏捷软件开发宣言
        > 
        > -   **个体和互动** 高于 流程和工具
        > -   **工作的软件** 高于 详尽的文档
        > -   **客户合作** 高于 合同谈判
        > -   **响应变化** 高于 遵循计划
        
        ![[笔记同步助手/images/cfa0b1b2ad16695f3828b8837f991368_MD5.png|Image]]
        
        > 角色：产品所有者（决定做什么，能对需求拍板的人）、团队负责人（解决各种问题，专注如何更好的工作，屏蔽外部对开发团队的影响）、开发团队（项目执行人员，具体指开发人员和测试人员）。
        
        > 准备工作：商业案例和资金、合同、憧憬、初始产品需求、初始发布计划、入股、组建团队。
        
        > 敏捷团队通常人数为8-10人。
        
        > 工作量估算：将开发任务量化，包括原型、Logo设计、UI设计、前端开发等，尽量把每个工作分解到最小任务量，最小任务量标准为工作时间不能超过两天，然后估算总体项目时间。把每个任务都贴在看板上面，看板上分三部分：to do（待完成）、in progress（进行中）和done（已完成）。
        
2.  项目团队组建
    
    -   团队的构成和角色
        
        ![[笔记同步助手/images/44a7089995835b1b3b1875dbad27432e_MD5.png|company_architecture]]
        
    -   编程规范和代码审查（`flake8`、`pylint`）
        
        ![[笔记同步助手/images/557409a29ecce02921076255dcb58e00_MD5.png|Image]]
        
    -   Python中的一些“惯例”（请参考[《Python惯例-如何编写Pythonic的代码》](/jackfrued/Python-100-Days/blob/master/%E7%95%AA%E5%A4%96%E7%AF%87/Python%E7%BC%96%E7%A8%8B%E6%83%AF%E4%BE%8B.md)）
        
    -   影响代码可读性的原因：
        
        -   代码注释太少或者没有注释
        -   代码破坏了语言的最佳实践
        -   反模式编程（意大利面代码、复制-黏贴编程、自负编程、……）
3.  团队开发工具介绍
    
    -   版本控制：Git、Mercury
    -   缺陷管理：[Gitlab](https://about.gitlab.com/)、[Redmine](http://www.redmine.org.cn/)
    -   敏捷闭环工具：[禅道](https://www.zentao.net/)、[JIRA](https://www.atlassian.com/software/jira/features)
    -   持续集成：[Jenkins](https://jenkins.io/)、[Travis-CI](https://travis-ci.org/)
    
    请参考[《团队项目开发的问题和解决方案》](/jackfrued/Python-100-Days/blob/master/Day91-100/91.%E5%9B%A2%E9%98%9F%E9%A1%B9%E7%9B%AE%E5%BC%80%E5%8F%91%E7%9A%84%E9%97%AE%E9%A2%98%E5%92%8C%E8%A7%A3%E5%86%B3%E6%96%B9%E6%A1%88.md)。
    

##### 项目选题和理解业务

[](#项目选题和理解业务)

1.  选题范围设定
    
    -   CMS（用户端）：新闻聚合网站、问答/分享社区、影评/书评网站等。
        
    -   MIS（用户端+管理端）：KMS、KPI考核系统、HRS、CRM系统、供应链系统、仓储管理系统等。
        
    -   App后台（管理端+数据接口）：二手交易类、报刊杂志类、小众电商类、新闻资讯类、旅游类、社交类、阅读类等。
        
    -   其他类型：自身行业背景和工作经验、业务容易理解和把控。
        
2.  需求理解、模块划分和任务分配
    
    -   需求理解：头脑风暴和竞品分析。
    -   模块划分：画思维导图（XMind），每个模块是一个枝节点，每个具体的功能是一个叶节点（用动词表述），需要确保每个叶节点无法再生出新节点，确定每个叶子节点的重要性、优先级和工作量。
    -   任务分配：由项目负责人根据上面的指标为每个团队成员分配任务。
    
    ![[笔记同步助手/images/4273c04003a83af223c2399e6c1e6a37_MD5.png|Image]]
    
3.  制定项目进度表（每日更新）
    
    | 模块 | 功能 | 人员 | 状态 | 完成 | 工时 | 计划开始 | 实际开始 | 计划结束 | 实际结束 | 备注 |
    | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
    | 评论 | 添加评论 | 王大锤 | 正在进行 | 50% | 4 | 2018/8/7 |  | 2018/8/7 |  |  |
    |  | 删除评论 | 王大锤 | 等待 | 0% | 2 | 2018/8/7 |  | 2018/8/7 |  |  |
    |  | 查看评论 | 白元芳 | 正在进行 | 20% | 4 | 2018/8/7 |  | 2018/8/7 |  | 需要进行代码审查 |
    |  | 评论投票 | 白元芳 | 等待 | 0% | 4 | 2018/8/8 |  | 2018/8/8 |  |  |
    
4.  OOAD和数据库设计
    

-   UML（统一建模语言）的类图
    
    ![[笔记同步助手/images/3f866a475e4217292b1a3b93f46792b2_MD5.jpg|uml]]
    
-   通过模型创建表（正向工程），例如在Django项目中可以通过下面的命令创建二维表。
    
    python manage.py makemigrations app
    python manage.py migrate
    
-   使用PowerDesigner绘制物理模型图。
    
    ![[笔记同步助手/images/d6a8538541184bc55670a9cdef3e1d28_MD5.png|Image]]
    
-   通过数据表创建模型（反向工程），例如在Django项目中可以通过下面的命令生成模型。
    
    python manage.py inspectdb \> app/models.py
    

#### 第92天：[Docker容器技术详解](/jackfrued/Python-100-Days/blob/master/Day91-100/92.Docker%E5%AE%B9%E5%99%A8%E6%8A%80%E6%9C%AF%E8%AF%A6%E8%A7%A3.md)

[](#第92天docker容器技术详解)

1.  Docker简介
2.  安装Docker
3.  使用Docker创建容器（Nginx、MySQL、Redis、Gitlab、Jenkins）
4.  构建Docker镜像（Dockerfile的编写和相关指令）
5.  容器编排（Docker-compose）
6.  集群管理（Kubernetes）

#### 第93天：[MySQL性能优化](/jackfrued/Python-100-Days/blob/master/Day91-100/93.MySQL%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96.md)

[](#第93天mysql性能优化)

1.  基本原则
2.  InnoDB引擎
3.  索引的使用和注意事项
4.  数据分区
5.  SQL优化
6.  配置优化
7.  架构优化

#### 第94天：[网络API接口设计](/jackfrued/Python-100-Days/blob/master/Day91-100/94.%E7%BD%91%E7%BB%9CAPI%E6%8E%A5%E5%8F%A3%E8%AE%BE%E8%AE%A1.md)

[](#第94天网络api接口设计)

1.  设计原则
    -   关键问题
    -   其他问题
2.  文档撰写

#### 第95天：\[使用Django开发商业项目\](./Day91-100/95.使用Django开发商业项 目.md)

[](#第95天使用django开发商业项目day91-10095使用django开发商业项目md)

##### 项目开发中的公共问题

[](#项目开发中的公共问题)

1.  数据库的配置（多数据库、主从复制、数据库路由）
2.  缓存的配置（分区缓存、键设置、超时设置、主从复制、故障恢复（哨兵））
3.  日志的配置
4.  分析和调试（Django-Debug-ToolBar）
5.  好用的Python模块（日期计算、图像处理、数据加密、三方API）

##### REST API设计

[](#rest-api设计)

1.  RESTful架构
    -   [理解RESTful架构](http://www.ruanyifeng.com/blog/2011/09/restful.html)
    -   [RESTful API设计指南](http://www.ruanyifeng.com/blog/2014/05/restful_api.html)
    -   [RESTful API最佳实践](http://www.ruanyifeng.com/blog/2018/10/restful-api-best-practices.html)
2.  API接口文档的撰写
    -   [RAP2](http://rap2.taobao.org/)
    -   [YAPI](http://yapi.demo.qunar.com/)
3.  [django-REST-framework](https://www.django-rest-framework.org/)的应用

##### 项目中的重点难点剖析

[](#项目中的重点难点剖析)

1.  使用缓存缓解数据库压力 - Redis
2.  使用消息队列做解耦合和削峰 - Celery + RabbitMQ

#### 第96天：[软件测试和自动化测试](/jackfrued/Python-100-Days/blob/master/Day91-100/96.%E8%BD%AF%E4%BB%B6%E6%B5%8B%E8%AF%95%E5%92%8C%E8%87%AA%E5%8A%A8%E5%8C%96%E6%B5%8B%E8%AF%95.md)

[](#第96天软件测试和自动化测试)

##### 单元测试

[](#单元测试)

1.  测试的种类
2.  编写单元测试（`unittest`、`pytest`、`nose2`、`tox`、`ddt`、……）
3.  测试覆盖率（`coverage`）

##### Django项目部署

[](#django项目部署)

1.  部署前的准备工作
    -   关键设置（SECRET\_KEY / DEBUG / ALLOWED\_HOSTS / 缓存 / 数据库）
    -   HTTPS / CSRF\_COOKIE\_SECUR / SESSION\_COOKIE\_SECURE
    -   日志相关配置
2.  Linux常用命令回顾
3.  Linux常用服务的安装和配置
4.  uWSGI/Gunicorn和Nginx的使用
    -   Gunicorn和uWSGI的比较
        -   对于不需要大量定制化的简单应用程序，Gunicorn是一个不错的选择，uWSGI的学习曲线比Gunicorn要陡峭得多，Gunicorn的默认参数就已经能够适应大多数应用程序。
        -   uWSGI支持异构部署。
        -   由于Nginx本身支持uWSGI，在线上一般都将Nginx和uWSGI捆绑在一起部署，而且uWSGI属于功能齐全且高度定制的WSGI中间件。
        -   在性能上，Gunicorn和uWSGI其实表现相当。
5.  使用虚拟化技术（Docker）部署测试环境和生产环境

##### 性能测试

[](#性能测试)

1.  AB的使用
2.  SQLslap的使用
3.  sysbench的使用

##### 自动化测试

[](#自动化测试)

1.  使用Shell和Python进行自动化测试
2.  使用Selenium实现自动化测试
    -   Selenium IDE
    -   Selenium WebDriver
    -   Selenium Remote Control
3.  测试工具Robot Framework介绍

#### 第97天：[电商网站技术要点剖析](/jackfrued/Python-100-Days/blob/master/Day91-100/97.%E7%94%B5%E5%95%86%E7%BD%91%E7%AB%99%E6%8A%80%E6%9C%AF%E8%A6%81%E7%82%B9%E5%89%96%E6%9E%90.md)

[](#第97天电商网站技术要点剖析)

1.  商业模式和需求要点
2.  物理模型设计
3.  第三方登录
4.  缓存预热和查询缓存
5.  购物车的实现
6.  支付功能集成
7.  秒杀和超卖问题
8.  静态资源管理
9.  全文检索方案

#### 第98天：[项目部署上线和性能调优](/jackfrued/Python-100-Days/blob/master/Day91-100/98.%E9%A1%B9%E7%9B%AE%E9%83%A8%E7%BD%B2%E4%B8%8A%E7%BA%BF%E5%92%8C%E6%80%A7%E8%83%BD%E8%B0%83%E4%BC%98.md)

[](#第98天项目部署上线和性能调优)

1.  MySQL数据库调优
2.  Web服务器性能优化
    -   Nginx负载均衡配置
    -   Keepalived实现高可用
3.  代码性能调优
    -   多线程
    -   异步化
4.  静态资源访问优化
    -   云存储
    -   CDN

#### 第99天：[面试中的公共问题](/jackfrued/Python-100-Days/blob/master/Day91-100/99.%E9%9D%A2%E8%AF%95%E4%B8%AD%E7%9A%84%E5%85%AC%E5%85%B1%E9%97%AE%E9%A2%98.md)

[](#第99天面试中的公共问题)

1.  计算机基础
2.  Python基础
3.  Web框架相关
4.  爬虫相关问题
5.  数据分析
6.  项目相关

### 第100天 - [补充内容](/jackfrued/Python-100-Days/blob/master/Day91-100/100.%E8%A1%A5%E5%85%85%E5%86%85%E5%AE%B9.md)

[](#第100天---补充内容)

-   面试宝典
    
    -   Python 面试宝典
    -   SQL 面试宝典（数据分析师）
    -   商业分析面试宝典
    -   机器学习面试宝典
-   机器学习数学基础
    
-   深度学习
    
    -   计算机视觉
    -   大语言模型

---

内容效果不满意？[点此反馈](https://feedback.notebooksyncer.com/feedback/61c38547_1781595012034?u=https%3A%2F%2Fgithub.com%2Fjackfrued%2FPython-100-Days.git&s=obsidian)