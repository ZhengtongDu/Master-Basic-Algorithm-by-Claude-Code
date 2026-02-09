# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

本项目是一份《基础算法从入门到精通》中文教程，基于 Duke University CS 330: Design & Analysis of Algorithms (Spring 2026) 课程内容编写。目标读者是具有基本编程和数据结构知识的本科生/研究生，用于一对一辅导场景。

github仓库：git@github.com:ZhengtongDu/Master-Basic-Algorithm-by-Claude-Code.git

## 项目结构

- `index.html` - docsify 入口文件
- `index.md` - 教程目录和章节索引
- `chapter00.md` - How to use this tutorial
- `chapter01.md` ~ `chapter24.md` - 各章节内容（对应 L01-L24 讲义）
- `appendix-a.md` ~ `appendix-c.md` - 附录内容
- `_sidebar.md` - docsify 侧边栏配置
- `.nojekyll` - GitHub Pages 配置

## 写作规范

- **语言**: 所有文档使用中文撰写，交流可以用英文
- **格式**: 使用 Markdown 格式
- **内容定位**: 要经常写一些 toy case 的代码（Python/伪代码），专注于讲解算法的原理、设计技巧与复杂度分析
- **目标**: 帮助读者从入门到精通基础算法的设计与分析
- **参考教材**:
  - [DPV] Dasgupta, Papadimitriou, Vazirani, *Algorithms* (2006)
  - [Er] Erickson, *Algorithms* (2019) - https://jeffe.cs.illinois.edu/teaching/algorithms/

## 章节对应关系

| 章节 | 课程讲义 | 主题 |
|------|---------|------|
| Ch01 | L01 | 算法基础与渐近分析 |
| Ch02 | L02 | 分治算法 I：归并排序与递推关系 |
| Ch03 | L03 | 分治算法 II：快速排序与随机化 |
| Ch04 | L04 | 并行算法 I：概念与分析 |
| Ch05 | L05 | 并行算法 II：算法设计 |
| Ch06 | L06 | 动态规划 I：入门与记忆化 |
| Ch07 | L07 | 动态规划 II：序列比对与依赖图 |
| Ch08 | L08 | 动态规划 III：矩阵乘法与树 |
| Ch09 | L09 | 图遍历 I：深度优先搜索 |
| Ch10 | L10 | 图遍历 II：拓扑排序与强连通分量 |
| Ch11 | L11 | 图遍历 III：广度优先搜索 |
| Ch12 | L12 | 最短路径 I：Dijkstra 算法 |
| Ch13 | L13 | 最短路径 II：动态规划方法 |
| Ch14 | L14 | 贪心算法 I：最小生成树 |
| Ch15 | L15 | 贪心算法 II：压缩与调度 |
| Ch16 | L16 | 网络流 I：最大流与最小割 |
| Ch17 | L17 | 网络流 II：算法与应用 |
| Ch18 | L18 | 计算复杂性 I：复杂性类与 NP 完全 |
| Ch19 | L19 | 计算复杂性 II：NP 完全问题与归约 |
| Ch20 | L20 | 计算复杂性 III：近似算法 |
| Ch21 | L21 | 大数据算法 I：聚类（贪心方法） |
| Ch22 | L22 | 大数据算法 II：聚类（K-means 与随机化） |
| Ch23 | L23 | 大数据算法 III：哈希 |
| Ch24 | L24 | 大数据算法 IV：草图与流算法 |

## Done Tasks

- [x] 2026-02-09: 创建项目结构和 docsify 配置
- [x] 2026-02-09: 生成 index.md 教程目录大纲
- [x] 2026-02-09: 创建 24 个章节和 3 个附录的占位文件

## Current Task

无

## Todolist
- [ ] 编写第一章：算法基础与渐近分析
- [ ] 编写第二章：分治算法 I
- [ ] ...（后续章节）
