# Chapter 0: 如何使用本教程

> 本章介绍本教程的设计理念、内容结构，以及如何借助 Claude Code 获得高效的交互式学习体验。

## 0.1 教程简介

本教程基于 Duke University CS 330: Design & Analysis of Algorithms (Spring 2026) 课程内容编写，旨在为**一对一辅导场景**提供系统化的算法学习材料。

与传统教材不同，本教程有以下特点：

- **交互式学习**：每个概念都配有可运行的 Python 代码示例，鼓励读者动手实验
- **渐进式讲解**：从直觉出发，先给出 toy case，再推广到一般情形
- **可视化优先**：使用 Mermaid 图表展示树、图、状态转移等结构，让抽象概念具象化
- **证明与直觉并重**：既给出严格的数学证明，也提供"为什么这样做"的直觉解释

**目标读者**：具有基本编程能力（熟悉至少一门编程语言）和数据结构基础知识（数组、链表、栈、队列、树）的本科生或研究生。

## 0.2 如何借助 Claude Code 学习

本教程设计为与 [Claude Code](https://claude.ai/code)（Anthropic 的 CLI 工具）配合使用。以下是推荐的学习工作流：

### 基本用法

1. **克隆本仓库**：
```bash
git clone git@github.com:ZhengtongDu/Master-Basic-Algorithm-by-Claude-Code.git
cd Master-Basic-Algorithm-by-Claude-Code
```

2. **启动 Claude Code**，在仓库目录下运行 `claude`，Claude 会自动读取 `CLAUDE.md` 了解项目上下文。

3. **按章节学习**：告诉 Claude 你想学习哪一章，例如：

```
请带我学习第三章动态规划，从斐波那契数列开始
```

### 推荐的交互方式

| 你想做什么 | 怎么问 Claude |
|-----------|--------------|
| 理解一个概念 | "用一个简单的例子解释 Dijkstra 算法" |
| 看代码实现 | "给我写一个归并排序的 Python 实现，加上详细注释" |
| 理解证明 | "主定理的证明中，为什么要分三种情况？" |
| 做练习 | "给我出一道关于动态规划的练习题，难度中等" |
| 对比概念 | "DFS 和 BFS 在什么场景下各有优势？" |
| 可视化 | "画一个 Mermaid 图展示 Prim 算法的执行过程" |

### 使用 /probe 命令

`/probe` 是一个自定义命令，用于深入探究某个知识点。当你对某个概念感到困惑时，可以使用：

```
/probe 为什么贪心算法不能解决所有优化问题？
```

Claude 会从多个角度分析这个问题，给出反例、直觉解释和严格论证。

## 0.3 教程结构说明

本教程共分为 **8 章**，每章对应一个核心主题，覆盖课程 L01-L24 的全部内容：

| 章节 | 主题 | 核心内容 |
|------|------|---------|
| [Chapter 1](chapter01.md) | **基础与分治** | 渐近分析、归并排序、快速排序、主定理 |
| [Chapter 2](chapter02.md) | **并行算法** | 工作量-深度模型、并行前缀和、Brent 定理 |
| [Chapter 3](chapter03.md) | **动态规划** | 记忆化、编辑距离、背包、矩阵链乘法、区间 DP |
| [Chapter 4](chapter04.md) | **图算法** | DFS、BFS、拓扑排序、Dijkstra、Bellman-Ford |
| [Chapter 5](chapter05.md) | **贪心算法** | MST、Kruskal、Prim、哈夫曼编码、调度 |
| [Chapter 6](chapter06.md) | **网络流** | 最大流最小割、Ford-Fulkerson、二部图匹配 |
| [Chapter 7](chapter07.md) | **计算复杂性** | P vs NP、归约、NP 完全、近似算法 |
| [Chapter 8](chapter08.md) | **大数据算法** | 聚类、K-means、哈希、Sketch、流算法 |

此外还有三个附录：[数学基础](appendix-a.md)、[数据结构回顾](appendix-b.md)、[参考资料](appendix-c.md)。

**建议学习顺序**：按章节顺序学习。Chapter 1 是后续所有章节的基础；Chapter 3（动态规划）和 Chapter 4（图算法）是重中之重，建议花最多时间。

## 0.4 排版约定

本教程使用以下排版约定：

- **定义**以加粗文字引出
- 数学公式使用 $\LaTeX$ 排版，如 $T(n) = 2T(n/2) + O(n)$
- 代码示例使用 Python，偶尔使用伪代码
- 树和图结构使用 Mermaid 图表展示
- 每节末尾的"练习题"分为三个难度：基础、进阶、挑战

## 0.5 参考资料

- **[DPV]** Dasgupta, Papadimitriou, Vazirani, *Algorithms* (2006)
- **[Er]** Erickson, *Algorithms* (2019) — [在线免费阅读](https://jeffe.cs.illinois.edu/teaching/algorithms/)
- **[CLRS]** Cormen, Leiserson, Rivest, Stein, *Introduction to Algorithms* (4th ed.)
