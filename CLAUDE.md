# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

本项目是一份《基础算法从入门到精通》中文教程，基于 Duke University CS 330: Design & Analysis of Algorithms (Spring 2026) 课程内容编写。目标读者是具有基本编程和数据结构知识的本科生/研究生，用于一对一辅导场景。

github仓库：git@github.com:ZhengtongDu/Master-Basic-Algorithm-by-Claude-Code.git

## 项目结构

- `index.html` - docsify 入口文件（含 KaTeX、Mermaid、搜索等插件配置）
- `index.md` - 教程目录和章节索引
- `README.md` - GitHub 项目说明
- `chapter00.md` - How to use this tutorial（含主定理速查）
- `chapter01.md` ~ `chapter08.md` - 各章节内容（每章对应一个主题）
- `appendix-a.md` ~ `appendix-c.md` - 附录内容
- `_sidebar.md` - docsify 侧边栏配置
- `.nojekyll` - GitHub Pages 配置
- `.github/workflows/deploy.yml` - GitHub Actions 自动部署

## 写作规范

- **语言**: 所有文档使用中文撰写，交流可以用英文
- **格式**: 使用 Markdown 格式
- **内容定位**: 要经常写一些 toy case 的代码（Python/伪代码），专注于讲解算法的原理、设计技巧与复杂度分析
- **目标**: 帮助读者从入门到精通基础算法的设计与分析
- **参考教材**:
  - [DPV] Dasgupta, Papadimitriou, Vazirani, *Algorithms* (2006)
  - [Er] Erickson, *Algorithms* (2019) - https://jeffe.cs.illinois.edu/teaching/algorithms/

## 图表绘制规范

本项目使用 **Mermaid** 绘制所有结构化图表（已在 index.html 中集成 docsify-mermaid 插件）。

### 使用方式

在 Markdown 中使用 ` ```mermaid ` 代码块即可渲染图表：

- **树结构**：使用 `graph TD`（自顶向下）
- **图结构**：使用 `graph LR`（左到右）或 `graph TD`
- **流程图**：使用 `flowchart`
- **状态图**：使用 `stateDiagram-v2`

### 适用场景

| 场景 | Mermaid 语法 | 示例 |
|------|-------------|------|
| 递归树 / 分治树 | `graph TD` | 归并排序递归树、递推关系展开 |
| 有向图 / 无向图 | `graph LR` / `graph TD` | DFS/BFS 遍历、最短路径 |
| 流网络 | `graph LR` + 边标注 | 最大流、残余图 |
| 状态转移 | `stateDiagram-v2` | DP 状态转移 |
| 算法流程 | `flowchart TD` | 算法步骤、判断分支 |

### 注意事项

- 所有树、图、流程图**必须使用 Mermaid**，不要使用 ASCII art 或外部图片
- 节点标签使用中文
- 边上可标注权重、容量等信息，如 `A -->|w=5| B`
- 复杂图表可拆分为多个小图分步展示

## 章节对应关系

| 章节 | 课程讲义 | 主题 |
|------|---------|------|
| Ch01 | L01-L03 | 基础与分治 |
| Ch02 | L04-L05 | 并行算法 |
| Ch03 | L06-L08 | 动态规划 |
| Ch04 | L09-L13 | 图算法 |
| Ch05 | L14-L15 | 贪心算法 |
| Ch06 | L16-L17 | 网络流 |
| Ch07 | L18-L20 | 计算复杂性 |
| Ch08 | L21-L24 | 大数据算法 |

## Done Tasks

- [x] 2026-02-09: 创建项目结构和 docsify 配置
- [x] 2026-02-09: 生成 index.md 教程目录大纲
- [x] 2026-02-09: 创建 8 个章节和 3 个附录的占位文件
- [x] 2026-02-09: 集成 Mermaid 图表绘制支持
- [x] 2026-02-09: 编写 Chapter 00（含主定理完整证明与速查表）
- [x] 2026-02-09: 编写 Chapter 02：并行算法（Work/Span 分析、并行求和、矩阵乘法、归并排序）
- [x] 2026-02-09: 编写 Chapter 03：动态规划（Fibonacci、LCS、MCM、背包、树形 DP）
- [x] 2026-02-09: 添加 GitHub Actions 自动部署 workflow
- [x] 2026-02-09: 添加 README.md
- [x] 2026-02-09: 修复 KaTeX 数学公式渲染（参考 LEAN 项目方案）
- [x] 2026-02-09: 调整正文字号（17px）和行高（1.8）
- [x] 2026-02-09: 创建 MyQuestions.md 问题记录文件（参考 LeanCC 格式）
- [x] 2026-02-09: 编写 Chapter 00 第 0.6 节：渐近符号（定义、性质、运算规则、8 道测试题）
- [x] 2026-02-09: 为 Chapter 02 添加 2.0 预备知识节（DAG、计算 DAG、fork-join 模型、记号汇总）
- [x] 2026-02-09: 扩充 Chapter 03：添加 DP 通用解题框架（3.2 节）+ 扩展背包问题（暴力复杂度、伪代码、对比图、空间优化）
- [x] 2026-02-11: 润色 Chapter 01：修正标题层级、添加 4 张 Mermaid 图表、补充对比表和伪代码、添加章节总结
- [x] 2026-02-13: 润色 Chapter 03：整合补充伪代码为 Python 实现，新增编辑距离（3.3.3）和零钱兑换（3.7.3）小节，补充 LCS/Tree DP/Fab/回文子串的 Python 代码和详细复杂度分析

## Current Task

编写第四章：图算法

## Todolist
- [x] 编写第一章：基础与分治
- [ ] 编写第四章：图算法
- [ ] 编写第五章：贪心算法
- [ ] 编写第六章：网络流
- [ ] 编写第七章：计算复杂性
- [ ] 编写第八章：大数据算法
