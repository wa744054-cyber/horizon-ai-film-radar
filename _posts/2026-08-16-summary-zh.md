---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 29 条内容中筛选出 4 条重要资讯。

---

1. [Anthropic 第二季营收超 115 亿美元，同比增长 14 倍](#item-1) ⭐️ 9.0/10
2. [发展中国家工程师力挺 RISC-V：嵌入式低成本硬件的最优解](#item-2) ⭐️ 8.0/10
3. [Anthropic 公开 Claude 系统提示词，引发透明度分析](#item-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B：令人印象深刻的开源视觉 LLM，但默认过度思考](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 第二季营收超 115 亿美元，同比增长 14 倍](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 9.0/10

Anthropic 公布第二季初步营收超过 115 亿美元，同比增长逾 14 倍，当季调整后营业利润转正。公司正在筹备可能在秋季启动的大型 IPO。 这标志着领先 AI 实验室取得重大商业里程碑，表明前沿 AI 公司能够实现快速商业化和盈利。此事可能重塑与 OpenAI 等竞争对手的格局，并显示投资者对 AI 公司 IPO 有强烈兴趣。 相关数字为初步数据，仍可能调整；第二季营收相比去年同期的 7.87 亿美元及 2026 年第一季的 47.3 亿美元均有大幅增长。据报道 IPO 目标定于秋季，但尚未公布官方申请细节。

telegram · zaihuapd · 8月16日 07:26

**背景**: Anthropic 是一家以 Claude 大型语言模型著称的人工智能公司，也是 OpenAI 的主要竞争对手。在生成式 AI 的企业需求强劲推动下，公司实现爆炸式增长，若成功上市将成为 AI 领域规模最大的 IPO 之一。

**标签**: `#Anthropic`, `#营收`, `#IPO`, `#AI行业`, `#财务新闻`

---

<a id="item-2"></a>
## [发展中国家工程师力挺 RISC-V：嵌入式低成本硬件的最优解](https://rvembedded.com/blog_post/12/) ⭐️ 8.0/10

一位来自发展中国家的嵌入式工程师发表文章，回应《RISC-V 他们本该更明智》的批评，指出 RISC-V 的价值在于低成本、易获取的硬件而非高性能。文章为 RISC-V 辩护，反驳了关于性能和碎片化的批评，同时也承认在某些地区运费可能远高于芯片本身的价格。 这篇回应为 RISC-V 的争论增添了来自欧美之外、难得一见的发展中国家视角。它指出，对于发展中国家的嵌入式开发者来说，成本和可及性往往比极致性能更具决定性，从而拓展了通常以硅谷为中心的讨论视野。 作者描述由于其所处地理位置，为一美元的芯片需要支付 60 到 200 美元的运费，但后文却声称 RISC-V 提供了‘一种以每颗十美分到达我所在国家的架构’。评论者质疑这一明显矛盾，并指出尼日利亚、孟加拉国等处于主要贸易航线上的国家运费要便宜得多。

hackernews · Narishma · 8月16日 17:01 · [社区讨论](https://news.ycombinator.com/item?id=49321717)

**背景**: RISC-V 是一种开放标准的指令集架构（ISA），与专有 ISA 不同，它可以被自由实现和扩展，因此对低成本、定制化的嵌入式设计很有吸引力。开源硬件运动强调设计文件和文档的可获取性，让更多人能够参与硬件开发。关于 RISC-V 的争论，常将其灵活性与开放性，同它在性能和碎片化方面与 ARM64 等成熟 ISA 的差距进行比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>
<li><a href="https://riscv.org/specifications/ratified/">Ratified Specifications - RISC-V International</a></li>
<li><a href="https://opensource.com/resources/what-open-hardware">What is open hardware ? | Opensource.com</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍欣赏这篇来自不同视角的文章，但也认为它在一定程度上没有真正回应原批评——原批评关注的是 RISC-V 在嵌入式之外的性能不佳以及 ISA 碎片化问题。另有几位评论者质疑运费论点：kelnos 和 vlovich123 指出，如果运费高达 60–200 美元，那么 10 美分与 1 美元的芯片差价几乎可以忽略；HawtAds 则表示，向尼日利亚或孟加拉国运送几美元以下的芯片并不需要 60 美元。

**标签**: `#RISC-V`, `#embedded systems`, `#open hardware`, `#cost`, `#accessibility`

---

<a id="item-3"></a>
## [Anthropic 公开 Claude 系统提示词，引发透明度分析](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在官方文档平台公开了 Claude 的系统提示词，披露了塑造模型行为的完整指令集。这一发布引发了社区的深入分析，包括 Simon Willison 用 git 提交历史对比不同模型版本间提示词的变化。 这一透明度举措让研究人员和开发者前所未有地看到 Anthropic 如何引导 Claude 的行为，有助于可解释性和安全性研究。它同时也引发了关于 AI 对齐以及将 AI 人格化所带来伦理影响的公开讨论。 公开的提示词包含值得注意的安全机制，例如在用户处于危机状态时优先考虑其福祉，并指示 Claude 在被虐待时保持礼貌语气或使用 end_conversation 工具结束对话。社区成员指出，系统提示词只是塑造 Claude 行为的整个分层体系中的一层。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**背景**: 系统提示词是在任何用户输入之前提供给大语言模型的一组隐藏指令，用于定义模型在整个交互过程中应如何表现。Claude 是 Anthropic 开发的 AI 助手，其训练采用“宪法 AI”方法，即用一套人类原则作为“宪法”来引导模型的伦理与安全行为。公开这些提示词让外部人士难得一见这套指导框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://promptengineering.org/system-prompts-in-large-language-models/">System Prompts in Large Language Models - Prompt Engineering</a></li>
<li><a href="https://en.wikipedia.org/wiki/Constitutional_AI">Constitutional AI</a></li>

</ul>
</details>

**社区讨论**: 评论者大多欢迎这次发布：Simon Willison 构建了提示词的 git 提交历史以追踪变化，并重点指出了关于 Claude Fable 5 和 Claude Mythos 5 首次发布的新指令。一些人表达了对鼓励将机器拟人化及其对人类互动下游影响的担忧，另一些人则提醒说，这些提示词只是塑造行为的分层系统中一个切片。还有一条离题评论指责本论坛删除了对 AI 持负面态度的帖文。

**标签**: `#Claude`, `#system prompts`, `#AI transparency`, `#LLM`, `#AI safety`

---

<a id="item-4"></a>
## [Qwen 3.8 27B：令人印象深刻的开源视觉 LLM，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

阿里巴巴 Qwen 实验室发布了 Qwen 3.8 27B，这是一款采用 Apache 2.0 许可、具备视觉能力的 27B 参数语言模型，其自报基准相比 Qwen 3.6 27B 和闭源模型 Qwen 3.7-Plus 有大幅提升。该模型默认使用 xhigh 推理深度，实际使用中会导致高 token 消耗和过度思考。 此次发布延续了可在消费级硬件上运行的开源权重模型的趋势，为开发者和爱好者提供了多模态任务的闭源 API 可行替代方案。其强劲的基准性能表明开源模型正在缩小与专有领先者的差距，但默认推理深度可能需要进行调整才能实际使用。 该模型提供了适用于 LM Studio 的 17GB Q4_K_M 量化 GGUF 版本，作者在 M5 Max MacBook Pro 和 NVIDIA DGX Spark 上进行了测试。在默认的 xhigh 推理设置下，生成一个简单的 SVG 花费了 21 分钟，消耗了 22,276 个推理 token 来产生 3,223 个输出 token，而关闭推理后速度明显更快。

rss · Simon Willison · 8月16日 22:00

**背景**: 视觉语言模型（VLM）是一种人工智能系统，能够同时从图像和文本中解析并生成信息，将大语言模型的能力从纯文本扩展到多模态。与传统计算机视觉模型不同，VLM 可以接受自然语言指令，并处理分类、检测、摘要和视觉问答等多类任务。开放权重模型会公开训练后的参数，允许本地部署和微调；而闭源模型（如 GPT-4）则保持权重私有，只提供 API。开放权重与闭源模型的选择涉及成本、控制力、数据驻留、安全性和生态等方面的权衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/vision-language-models/">What are Vision-Language Models? | NVIDIA Glossary</a></li>
<li><a href="https://theplanettools.ai/blog/closed-vs-open-weight-ai-models-how-to-choose-2026">Closed vs Open-Weight AI: How to Actually Choose (2026)</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Qwen`, `#open-source`, `#benchmarks`, `#AI`

---