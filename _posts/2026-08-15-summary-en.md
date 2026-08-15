---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 24 items, 3 important content pieces were selected

---

1. [BDH-CQ: 150M Model Achieves 29.5% on ARC-AGI-1 via Recurrent Latent Reasoning](#item-1) ⭐️ 9.0/10
2. [AI's Larger Working Memory May Outperform Human Mathematicians](#item-2) ⭐️ 8.0/10
3. [Alibaba's Qwen open-weight models hit 3B downloads, outpacing Meta and Google](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [BDH-CQ: 150M Model Achieves 29.5% on ARC-AGI-1 via Recurrent Latent Reasoning](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 9.0/10

The BDH-CQ model combines in-context learning with recurrent latent reasoning, updating its recurrent memory from task demonstrations and solving queries through iterative computation in a high-dimensional latent space without decoding intermediate steps. A 150M-parameter configuration reaches 29.5% pass@2 on ARC-AGI-1 at a computed cost of $0.00070 per task. This result claims to break the previously reported cost-accuracy Pareto frontier on ARC-AGI-1, showing that a compact 150M-parameter model can compete with far larger systems at a fraction of the cost. It challenges the dominant chain-of-thought paradigm by demonstrating that reasoning can happen entirely in latent space, which could reshape how in-context learning and test-time compute are approached. BDH-CQ builds on Dragon Hatchling (BDH), a post-Transformer recurrent architecture in which neuron-like units communicate through low-rank interactions and maintain context in an evolving associative state. Neither task identifiers nor evaluation-task demonstration pairs are used in training, and no parameters are updated at inference time.

reddit · r/MachineLearning · /u/moschles · Aug 15, 06:18

**Background**: ARC-AGI-1 is a benchmark designed to measure progress toward general intelligence by testing a system's ability to solve novel tasks it has not seen before. Traditional chain-of-thought reasoning models scale test-time compute by generating more tokens, whereas latent reasoning models like BDH-CQ iterate a recurrent block in continuous space, avoiding token-by-token decoding. In-context learning allows the model to adapt to new tasks from demonstrations given at inference time, without fine-tuning or parameter updates.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.09888v1">BDH-CQ: In-Context Learning with Recurrent Latent Reasoning</a></li>
<li><a href="https://arxiv.org/abs/2608.09888">[2608.09888] BDH-CQ: In-Context Learning with Recurrent ...</a></li>
<li><a href="https://www.explainx.ai/blog/pathway-bdh-cq-150m-post-transformer-arc-agi-august-2026">Pathway BDH-CQ: 150M Model, 11x Cheaper Than GPT-5.6 ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#in-context learning`, `#recurrent memory`, `#ARC-AGI`, `#latent reasoning`

---

<a id="item-2"></a>
## [AI's Larger Working Memory May Outperform Human Mathematicians](https://davidepiffer.com/p/ai-isnt-outthinking-mathematicians) ⭐️ 8.0/10

A recent essay argues that AI's vastly larger working memory, measured by context windows, could enable it to out-think humans in mathematics even without human-like reasoning. The author reframes intelligence as 'out-remembering' rather than raw logical horsepower. This challenges common assumptions about AI's limitations in mathematical reasoning and suggests future AI may solve problems through exhaustive exploration rather than insight. It could reshape debates about AI's role in intellectual and scientific work. Working memory in LLMs corresponds to the context window, measured in tokens, with larger windows allowing the model to process more information at once. The essay cites examples from mathematics and mentions projects like theoremdb.org that aim to collect and reuse negative results.

hackernews · rzk · Aug 15, 18:13 · [Discussion](https://news.ycombinator.com/item?id=49312845)

**Background**: LLMs are built on transformer architectures that use attention mechanisms, and the context window is the maximum amount of text the model can consider when generating output. Human working memory is limited to a few items, while modern AI context windows can span millions of tokens, creating a qualitative difference in 'memory' capacity. This difference underpins the essay's argument that AI might outperform humans in mathematical exploration.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Context_window">Context window - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/context-window">What is a context window? - IBM</a></li>
<li><a href="https://atlan.com/know/working-memory-llms/">Working Memory in LLMs: Context Window Deep Dive</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree, noting that human intelligence often boils down to out-remembering others, and that AI agents can publish and reuse negative results without fatigue. One commenter referenced Michael Nielsen's essay 'Augmenting Long-Term Memory,' while another said the point is fairly obvious, with others adding that AI also benefits from never getting tired.

**Tags**: `#AI`, `#cognition`, `#memory`, `#mathematics`, `#LLM`

---

<a id="item-3"></a>
## [Alibaba's Qwen open-weight models hit 3B downloads, outpacing Meta and Google](https://www.bloomberg.com/news/articles/2026-08-15/alibaba-ai-models-hit-3-billion-downloads-passing-meta-google) ⭐️ 8.0/10

Alibaba's open-weight Qwen AI models have surpassed 3 billion global downloads over the past six months, overtaking Meta's and Google's models, according to a Hugging Face report. Qwen has released more than 460 open-source models and spawned over 300,000 derivative versions. This milestone shows that Alibaba has become the most widely adopted open-weight AI model provider, beating Western tech giants in the open-model ecosystem. It signals a shift in AI leadership toward Chinese open-weight models and could influence how developers choose foundational models globally. The Hugging Face report shows Google models recorded 418 million downloads and Meta models 227 million in 2026, far behind Alibaba's 3 billion. Alibaba's Qwen family includes multiple model sizes, and its 'open weights' allow users to download and self-host the trained parameters, though this differs from full open-source licensing.

telegram · zaihuapd · Aug 15, 15:18

**Background**: Open-weight AI models make their trained parameters (weights) publicly available for download, enabling developers to run or fine-tune them without paying per-token API costs, unlike closed models. Alibaba launched Qwen (Tongyi Qianwen) in 2023, initially based on Meta's Llama architecture, and has since released dozens of models in various sizes. Qwen has become the most downloaded open model family, with a presence on platforms like Hugging Face.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://www.secondtalent.com/resources/every-qwen-ai-model-explained-compared/">Every Qwen AI Model Explained and Compared (Aug, 2026)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Open-source`, `#Alibaba`, `#Qwen`, `#Industry news`

---