---
title: llmappl 记录
date: 2026-01-25
description: 
tags: 
    - llmappl
categories:
    - "技术"
---

#### 01/25 学习路线

❌ 阶段1：深度学习基础（可跳）
原因： 
* Agent 开发 不要求你会反向传播 / CNN / Transformer 推导
* 会“怎么用模型”比“模型怎么训练出来”重要

👉 建议替代方案：
* 了解即可：Transformer 是什么 + Attention 在干嘛
* 不要陷入 PyTorch 细节

🟡 阶段2：大模型技术总览（必须快速看）
需要知道：
* LLM ≠ ChatGPT
* Inference / Token / Context Window / KV Cache 是什么
* 为什么 Agent 会慢 / 会幻觉
👉 不求细节，只求架构感

🟡 阶段3：大模型部署实战（偏工程，推荐）
强烈建议学，原因：
* AI Agent = 后端服务 + LLM 推理
* 不懂部署 → Agent 只能跑在 notebook 里
重点掌握：
* vLLM / llama.cpp / Ollama
* GPU / CPU 推理差异
* API 封装

✅ 阶段4：Prompt 提示工程（必学）
这是 Agent 的“编程语言”。
你必须会：
* System / User / Tool Prompt 设计
* Chain of Thought / ReAct

JSON / Schema 输出

多轮状态控制

Prompt 能力 ≈ Agent 开发能力的一半

✅ 阶段5：RAG + Agent（核心）

这是你**从“会用 LLM” → “能做系统”**的分水岭。

你要重点掌握：

向量数据库（FAISS / Milvus）

Chunk / Embedding 策略

Tool Calling

Agent 调度逻辑

👉 这是企业最常用的 LLM 形态

🟡 阶段6：垂域微调（选学）

什么时候有用？

RAG 不够

Prompt 控制不住输出风格

企业私有知识强

只学：

LoRA / QLoRA

不碰全量训练

❌ 阶段7 & 8：预训练 + 分布式训练（可跳）

这是：

算法工程师

大厂模型团队

Infra / CUDA 方向

👉 与你的目标几乎不重合

🟡 阶段9：产品级推理优化（建议）

非常加分的一阶段：

你会懂：

延迟 / 吞吐 / 成本权衡

KV Cache / Batch

多 Agent 并发

✅ 阶段10：推理引擎部署（必学）

这是工程落地能力的体现。

你要会：

单机 / 多卡

API 限流

与后端系统集成

❌ 阶段11：多模态（按需）

如果你做：

OCR Agent

语音 Agent

图像分析 Agent
👉 才学

否则可跳

✅ 阶段12：综合项目实战（必学）

这是你简历最重要的一部分。

项目目标应是：

“一个能完成真实任务的 Agent 系统”

✅ 阶段13：Agent + MCP 工业系统（强烈推荐）

这是：

多 Agent 协作

状态机

工具链

长任务分解

👉 这一步你已经是 Agent 工程师了

🟡 阶段14：面试专项（最后学）

