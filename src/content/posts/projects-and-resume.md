---
title: Projects and Resume / 项目与履历
published: 2026-06-17
description: A public snapshot of my projects, awards, and technical background.
tags: [Projects, Resume, AI]
category: Projects
draft: false
lang: zh_CN
---

这篇文章整理我的公开履历信息，方便快速了解我做过什么、关注什么。

## Education

- 西南大学，计算机与信息科学学院软件学院。
- 软件工程（中外合作办学），2022.09 - 2026.06。
- GPA: 4.1 / 5.0，Rank: 8 / 127。
- IELTS: 6.5。

## 智居云枢

**基于 RAG + MCP 的多模态智能家居系统**

这是一个面向多租户短租场景的智能家居系统，集成 RAG 和 AI 助手，实现设备智能控制、安防预警和租户行为分析。

我负责项目整体推进和智能体工作流设计。系统使用 BGE-M3 向量模型构建防火、节能、App 使用指南知识库，并通过 MaxKB 设计问答工作流和部署 DeepSeek / Qwen 等语言模型。后端通过 FastMCP 暴露 20+ 个可远程调用的设备控制接口，让大模型可以自主完成设备控制任务。

## 影随飞

**姿态驱动的无人机控制及目标追随系统**

这是 2024 年中国大学生计算机设计大赛项目，获得国家级二等奖。

项目基于 MediaPipe 姿态估计识别人身关键点，通过上半身姿态动作触发无人机控制逻辑，例如向前飞、手掌降落和进入目标追随模式。系统使用 Tello SDK 完成无人机控制，并用 PySide2 开发可视化界面。

## Awards

- 第十七届中国大学生计算机设计大赛，国家级二等奖。
- 全国大学生数学建模竞赛，省级一等奖。
- 蓝桥杯 Python A 组，省级一等奖。
- 全国大学生数学竞赛（非数学类 A 组），省级三等奖。
- 西南大学本科生奖学金、三好学生。

## Skills

- Python, C/C++, Markdown, LaTeX, Matlab。
- PyTorch, CUDA, SQL, Docker, Git, FastAPI。
- Linux 环境配置、调试与基础工程实践。
