---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 24 条内容中筛选出 3 条重要资讯。

---

1. [BDH-CQ：150M 参数模型通过循环潜在推理在 ARC-AGI-1 上达到 29.5%](#item-1) ⭐️ 9.0/10
2. [AI 更大的工作记忆或能超越人类数学家](#item-2) ⭐️ 8.0/10
3. [阿里 Qwen 开放权重模型下载量超 30 亿，超越 Meta 和谷歌](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [BDH-CQ：150M 参数模型通过循环潜在推理在 ARC-AGI-1 上达到 29.5%](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 9.0/10

BDH-CQ 模型将上下文学习与循环潜在推理相结合，通过任务演示更新其循环记忆，并在高维潜在空间中进行迭代计算来求解查询，而无需解码中间步骤。一个 150M 参数的配置在 ARC-AGI-1 上达到 29.5%的 pass@2，每任务计算成本为 0.00070 美元。 这一结果声称突破了此前 ARC-AGI-1 上报告的成本-精度帕累托前沿，表明一个紧凑的 150M 参数模型能以极低的成本与更大的系统竞争。它挑战了以思维链为主导的范式，证明推理可以完全在潜在空间中进行，这可能重塑上下文学习和测试时计算的方式。 BDH-CQ 基于 Dragon Hatchling（BDH）这一后 Transformer 循环架构，其中的类神经元单元通过低秩交互进行通信，并在演化的联想状态中维持上下文。训练中不使用任务标识符或评测任务的演示对，推理时也不更新任何参数。

reddit · r/MachineLearning · /u/moschles · 8月15日 06:18

**背景**: ARC-AGI-1 是一个旨在衡量通用智能进展的基准测试，用于检验系统解决从未见过的新任务的能力。传统的思维链推理模型通过生成更多词元来扩展测试时计算，而像 BDH-CQ 这样的潜在推理模型则在连续空间中迭代循环模块，避免了逐词元解码。上下文学习使模型能够在推理时根据演示适应新任务，而无需微调或更新参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.09888v1">BDH-CQ: In-Context Learning with Recurrent Latent Reasoning</a></li>
<li><a href="https://arxiv.org/abs/2608.09888">[2608.09888] BDH-CQ: In-Context Learning with Recurrent ...</a></li>
<li><a href="https://www.explainx.ai/blog/pathway-bdh-cq-150m-post-transformer-arc-agi-august-2026">Pathway BDH-CQ: 150M Model, 11x Cheaper Than GPT-5.6 ...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#in-context learning`, `#recurrent memory`, `#ARC-AGI`, `#latent reasoning`

---

<a id="item-2"></a>
## [AI 更大的工作记忆或能超越人类数学家](https://davidepiffer.com/p/ai-isnt-outthinking-mathematicians) ⭐️ 8.0/10

近期一篇评论文章提出，AI 远超人类的工作记忆（以上下文窗口衡量）可能使其在数学领域超越人类，即使不具备类似人类的推理能力。作者将智力重新定义为“记忆取胜”而非纯粹的逻辑马力。 这挑战了关于 AI 在数学推理方面局限性的常见假设，并表明未来的 AI 可能通过穷举探索而非洞见来解决问题。它可能重塑关于 AI 在智力与科学工作中角色的讨论。 LLM 中的工作记忆对应于以 token 计量的上下文窗口，窗口越大，模型能同时处理的信息就越多。该文引用了数学中的实例，并提到如 theoremdb.org 等项目，旨在收集和复用阴性结果（失败尝试）。

hackernews · rzk · 8月15日 18:13 · [社区讨论](https://news.ycombinator.com/item?id=49312845)

**背景**: LLM 基于使用注意力机制的 Transformer 架构，上下文窗口是模型生成输出时能考虑的最大文本量。人类工作记忆只能容纳少量信息，而现代 AI 的上下文窗口可达数百万 token，在“记忆”容量上形成了质的差异。这一差异是该文论证 AI 可能在数学探索中超越人类的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/context-window">What is a context window? - IBM</a></li>
<li><a href="https://atlan.com/know/working-memory-llms/">Working Memory in LLMs: Context Window Deep Dive</a></li>

</ul>
</details>

**社区讨论**: 评论者大体表示认同，指出人类的智力往往归结为比他人记得更多，而 AI 智能体可以不知疲倦地发表和复用阴性结果。有评论者引用 Michael Nielsen 的文章《Augmenting Long-Term Memory》，还有人称这一观点显而易见，另有人补充说 AI 还从不知疲倦中受益。

**标签**: `#AI`, `#cognition`, `#memory`, `#mathematics`, `#LLM`

---

<a id="item-3"></a>
## [阿里 Qwen 开放权重模型下载量超 30 亿，超越 Meta 和谷歌](https://www.bloomberg.com/news/articles/2026-08-15/alibaba-ai-models-hit-3-billion-downloads-passing-meta-google) ⭐️ 8.0/10

阿里巴巴的开放权重 AI 模型 Qwen 在过去六个月全球下载量超过 30 亿次，超越了 Meta 和谷歌的模型。据 Hugging Face 报告，阿里已开源超过 460 个模型，并衍生出超过 30 万个版本。 这一里程碑表明阿里巴巴已成为采用最广泛的开放权重 AI 模型提供方，在开放模型生态中超过了西方科技巨头。这标志着 AI 领导力向中国开放权重模型转移，可能影响全球开发者对基础模型的选择。 Hugging Face 报告显示，2026 年谷歌模型下载量为 4.18 亿次，Meta 为 2.27 亿次，远低于阿里的 30 亿次。Qwen 模型家族包含多种尺寸，其‘开放权重’允许用户下载并自行托管训练好的参数，但这与完全的开源许可有所不同。

telegram · zaihuapd · 8月15日 15:18

**背景**: 开放权重 AI 模型公开提供训练好的参数（权重），开发人员可以下载并微调或自行部署，而无需按 token 支付 API 费用，这与封闭模型不同。阿里于 2023 年推出 Qwen（通义千问），最初基于 Meta 的 Llama 架构，此后发布了数十种不同尺寸的模型。Qwen 已成为下载量最大的开放模型家族，在 Hugging Face 等平台上广泛使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://www.secondtalent.com/resources/every-qwen-ai-model-explained-compared/">Every Qwen AI Model Explained and Compared (Aug, 2026)</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open-source`, `#Alibaba`, `#Qwen`, `#Industry news`

---