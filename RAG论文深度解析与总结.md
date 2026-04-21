# RAG论文深度解析与总结

> 📅 推送日期：2026-04-21 | arXiv: 2005.11401 | 引用量：12,952

## 论文信息

- **标题**：Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
- **作者**：Patrick Lewis, Ethan Perez, Aleksandra Piktus, Fabio Petroni, Vladimir Karpukhin, Naman Goyal, Heinrich Küttler, Mike Lewis, Wen-tau Yih, Tim Rocktäschel, Sebastian Riedel, Douwe Kiela
- **发布时间**：2020年5月（Accepted at NeurIPS 2020）
- **链接**：https://arxiv.org/abs/2005.11401

---

## 深度解读

### 背景与动机

大型预训练语言模型（LLM）虽然在各类NLP任务上取得了最先进的结果，但它们存储知识的能力本质上是"参数化"的——知识被压缩在权重中，难以精确检索和操控。这一局限性导致在知识密集型任务（如开放域问答）上，LLM的表现往往不如专门设计的检索-抽取架构。此外，LLM无法提供决策溯源，也难以及时更新过时知识。如何让语言模型既拥有强大的生成能力，又能动态、精确地访问外部知识，成为当时的核心挑战。

### 核心方法

本文提出了检索增强生成（RAG）框架，将预训练的参数化语言模型与非参数化知识库相结合。具体架构包含两个核心组件：

1. **参数化记忆**：一个预训练的seq2seq模型（基于BART），负责根据检索到的内容生成答案
2. **非参数化记忆**：一个预训练的神经检索器（DPR，Dense Passage Retriever），从Wikipedia的稠密向量索引中检索相关段落

作者提出了两种RAG变体：
- **RAG-Sequence**：整篇生成序列共用同一检索段落
- **RAG-Token**：每个生成token可使用不同检索段落

两种方法均通过端到端微调优化，使检索器和生成器协同训练、互相增强。

### 关键创新

1. **统一框架**：首次将神经检索与语言生成深度整合，无需为每个下游任务单独设计模块
2. **端到端可微调**：检索器与生成器联合优化，检索质量直接服务于生成效果
3. **开源可复现**：发布完整代码和模型权重，推动了RAG技术的快速普及

### 实验与结果

在多个知识密集型任务上，RAG模型刷新了三项开放域问答SOTA：

- **NaturalQuestions**：RAG在TriviaQA上达到54.4 EM
- **MS MARCO**：RAG在三个子任务上均超越专用模型
- **Jeopardy问答**：在生成事实性和多样性上显著优于纯参数化模型

### 局限与启示

- 检索库限于Wikipedia，无法覆盖长尾或实时知识
- 推理开销较大（需实时检索），部署成本高
- 为后续Agentic RAG、多模态RAG等演进奠定了基础，被引用超过12,000次，是RAG领域的奠基性工作
