# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

本项目是一份《基础算法从入门到精通》中文教程，基于 Duke University CS 330: Design & Analysis of Algorithms (Spring 2026) 课程内容编写。目标读者是具有基本编程和数据结构知识的本科生/研究生，用于一对一辅导场景。

github仓库：git@github.com:ZhengtongDu/Master-Basic-Algorithm-by-Claude-Code.git

## 项目结构

- `index.html` - docsify 入口文件
- `index.md` - 教程目录和章节索引
- `chapter00.md` - How to use this tutorial
- `chapter01.md` ~ `chapter08.md` - 各章节内容（每章对应一个主题）
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

## Current Task

无

## Todolist
- [ ] 编写第一章：基础与分治
- [ ] 编写第二章：并行算法
- [ ] ...（后续章节）
