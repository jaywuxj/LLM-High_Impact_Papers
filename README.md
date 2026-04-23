# LLM High Impact Papers — 大语言模型高影响力论文深度解析

> 每日自动推送 LLM / Agent 领域高引用经典论文与近期热度论文，提供 2000-4000 字中文深度解读。

---

## 📖 项目简介

本仓库收录大语言模型（LLM）与 AI Agent 领域的**高影响力论文深度解析**，涵盖：

- **高引用经典论文**：引用量 > 3000 的奠基性工作，如 Transformer、GPT 系列、BERT、Chain-of-Thought 等
- **近期热度论文**：最近一周发布、在学术界与工业界引发广泛关注的前沿研究
- **Agent 专题**：ReAct、AgentSPEX 等智能体推理与执行框架

每篇解析均以**中文**撰写，字数 2000-4000 字，力求让读者不读原文即可掌握核心思想。

---

## 📂 论文目录

### 🏛️ 经典基础论文

| 论文 | 关键词 | 引用量 |
|------|--------|--------|
| [Attention Is All You Need（Transformer）](./Attention-Is-All-You-Need深度论文分析.md) | Transformer, Self-Attention, Encoder-Decoder | 100,000+ |
| [BERT: Pre-training of Deep Bidirectional Transformers](./BERT论文深度解析与总结.md) | BERT, Pre-training, Fine-tuning, NLU | 80,000+ |
| [Language Models are Few-Shot Learners（GPT-3）](./GPT-3论文深度解析与总结.md) | GPT-3, Few-Shot, In-Context Learning | 30,000+ |
| [Improving Language Understanding by Generative Pre-Training（GPT-1）](./GPT-1论文深度解析与总结.md) | GPT-1, Generative Pre-Training, Transfer Learning | 10,000+ |
| [Scaling Laws for Neural Language Models](./Scaling%20Laws%20for%20Neural%20Language%20Models%20深度解析与总结.md) | Scaling Laws, Compute, Data, Parameters | 8,000+ |
| [LLaMA: Open and Efficient Foundation Language Models](./LLaMA论文深度解析与总结.md) | LLaMA, Open-Source, Efficient Training | 20,000+ |
| [Llama 2: Open Foundation and Fine-Tuned Chat Models](./2026-04-22-Llama2开源对话模型深度解析.md) | Llama 2, RLHF, Chat, Safety | 15,000+ |

### 🧠 推理与对齐

| 论文 | 关键词 | 引用量 |
|------|--------|--------|
| [Chain-of-Thought Prompting Elicits Reasoning in LLMs](./Chain-of-Thought论文深度解析与总结.md) | Chain-of-Thought, Reasoning, Prompting | 15,000+ |
| [Training Language Models to Follow Instructions（InstructGPT）](./InstructGPT论文深度解析与总结.md) | InstructGPT, RLHF, Alignment | 10,000+ |
| [Constitutional AI: Harmlessness from AI Feedback](./Constitutional-AI论文深度解析与总结.md) | Constitutional AI, RLAIF, Safety | 5,000+ |
| [Self-Consistency Improves Chain of Thought Reasoning](./2026-04-23-Self-Consistency深度解析.md) | Self-Consistency, Majority Voting, CoT | 8,000+ |
| [CoT-PoT Ensembling for Efficient LLM Reasoning](./2026-04-23-CoT-PoT-Ensembling深度解析.md) | CoT, PoT, Ensembling, Efficiency | — |
| [Language Models are Few-Shot Learners（GPT-3 深度版）](./2026-04-23-GPT3-Few-Shot深度解析.md) | GPT-3, Few-Shot, Prompting | 30,000+ |
| [DeepSeek-R1: Incentivizing Reasoning via RL](./DeepSeek-R1深度论文分析.md) | DeepSeek-R1, Reinforcement Learning, Reasoning | 5,000+ |

### 🤖 AI Agent

| 论文 | 关键词 | 引用量 |
|------|--------|--------|
| [ReAct: Synergizing Reasoning and Acting in LLMs](./2026-04-22-ReAct推理与行动协同深度解析.md) | ReAct, Tool Use, Reasoning, Acting | 5,000+ |
| [AgentSPEX: Agent Specification and Execution Language](./2026-04-22-AgentSPEX%20Agent规范与执行语言深度解析.md) | AgentSPEX, Agent DSL, Execution | — |
| [ReactBench: Benchmarking LLM Agents](./ReactBench论文深度解析与总结.md) | ReactBench, Agent Evaluation, Tool Use | — |
| [Experience Compression Spectrum](./Experience-Compression论文深度解析与总结.md) | Agent Memory, Experience Compression, Multi-Agent | — |

### 🔍 检索增强与多模态

| 论文 | 关键词 | 引用量 |
|------|--------|--------|
| [Retrieval-Augmented Generation（RAG）](./RAG论文深度解析与总结.md) | RAG, Retrieval, Knowledge-Intensive NLP | 12,000+ |
| [LLaVA: Visual Instruction Tuning](./LLaVA论文深度解析与总结.md) | LLaVA, Multimodal, Visual Instruction Tuning | 15,000+ |

### ⚡ 效率与优化

| 论文 | 关键词 | 引用量 |
|------|--------|--------|
| [Sequential KV Cache Compression](./Sequential-KV-Cache-Compression论文深度解析与总结.md) | KV Cache, Compression, Inference Efficiency | — |

---

## 📋 每篇解析的内容结构

每篇深度解析均包含以下章节：

```
1. 论文基本信息（标题、作者、年份、引用量、arXiv 链接）
2. 研究背景与动机
3. 核心方法详解
4. 实验设计与结果
5. 关键创新与贡献
6. 后续影响与演进
7. 局限性与改进方向
8. 总结与启示
9. 参考文献
```

---

## 🚀 更新机制

本仓库由自动化 AI 研究助手**每日推送**，策略如下：

| 类型 | 数量 | 筛选标准 |
|------|------|---------|
| 高引用经典论文 | 2 篇/天 | LLM/Agent 方向，引用量 > 3,000 |
| 近期热度论文 | 1 篇/天 | 最近一周发布，学术/工业界热度高 |

数据来源：[Semantic Scholar API](https://api.semanticscholar.org/) + [Hugging Face Daily Papers](https://huggingface.co/papers)

---

## 🗺️ 学习路线建议

如果你是 LLM 领域的初学者，建议按以下顺序阅读：

```
基础架构
└── Attention Is All You Need（Transformer）
    └── BERT（双向预训练）
        └── GPT-1 → GPT-3（生成式预训练 + Few-Shot）
            └── Scaling Laws（规模定律）
                └── InstructGPT（RLHF 对齐）
                    └── Constitutional AI（AI 反馈对齐）

推理能力
└── Chain-of-Thought（思维链）
    └── Self-Consistency（自洽性）
        └── CoT-PoT Ensembling（高效推理）

Agent 方向
└── ReAct（推理 + 行动）
    └── AgentSPEX（Agent 规范语言）
        └── ReactBench（Agent 评测）

检索增强
└── RAG（检索增强生成）

多模态
└── LLaVA（视觉指令微调）

前沿推理
└── DeepSeek-R1（强化学习推理）
```

---

## 📊 统计

- 📄 **论文总数**：21 篇（持续更新）
- 🗓️ **最近更新**：2026-04-23
- 🌐 **覆盖领域**：LLM 基础、推理、对齐、Agent、多模态、效率优化

---

## 🤝 贡献

欢迎提交 Issue 推荐你认为值得深度解析的论文，或对现有解析提出改进建议。

---

## 📜 License

本仓库内容为学术研究目的的论文解读与总结，原始论文版权归各自作者所有。
