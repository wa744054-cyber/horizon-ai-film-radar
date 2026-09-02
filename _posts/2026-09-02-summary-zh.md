---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---

> 从 40 条内容中筛选出 11 条重要资讯。

---

1. [谷歌发布 Gemini 3.8 Flash 与 Flash Cyber 模型](#item-1) ⭐️ 9.0/10
2. [Anthropic 发布 Claude Fable 5.1；鹈鹕测试暴露推理设置怪象](#item-2) ⭐️ 9.0/10
3. [Meta 发布 Muse Spark 1.3：低价编程模型登顶 DeepSWE](#item-3) ⭐️ 8.0/10
4. [报告：三个网站生成 215,128 个“最佳软件”页面，被 Perplexity 大规模引用](#item-4) ⭐️ 8.0/10
5. [Jasper Research 发布从零训练文生图模型的详细指南](#item-5) ⭐️ 8.0/10
6. [开源 AI 检测器在实际基准测试中难以达到 0.5%假阳性率](#item-6) ⭐️ 8.0/10
7. [英伟达发布 DLSS 5 神经渲染，9 月 3 日随 NBA 2K27 上线](#item-7) ⭐️ 8.0/10
8. [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜夺冠](#item-8) ⭐️ 8.0/10
9. [月之暗面与美云巨头谈判，拟按最高 30%分成授权 Kimi K3](#item-9) ⭐️ 8.0/10
10. [xAI 发布 Grok 4.6，强化长时智能体任务与视觉能力](#item-10) ⭐️ 8.0/10
11. [FBI 调查暗网服务 Nexus 兜售 1.53 亿张驾照扫描件](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌发布 Gemini 3.8 Flash 与 Flash Cyber 模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 9.0/10

谷歌发布了 Gemini 3.8 Flash 与 Gemini 3.8 Flash Cyber，距离上一代 3.7 Flash 仅约三周。它们在多项基准测试中接近 Opus 5 等更贵的前沿模型，同时速度更快、成本更低。 此次发布大幅降低了接近前沿水平的智能成本与延迟，可能改写开发者在长时程编码和自主智能体上的选型逻辑与成本结构。Cyber 版本还为网络安全防御者提供了针对漏洞检测和自动修补等任务的专用工具。 Gemini 3.8 Flash 基于 3.7 Flash 改进，在软件工程和智能体知识工作流上有显著提升；Flash Cyber 增加了漏洞检测与自动修补能力，但仅通过 Google 的 Fairwind Program 提供给受信任的防御者。社区基准测试显示该模型智能评分达到 59，与 Opus 5 medium 持平；还有开发者仅花约 1.8 美分、13 秒就生成了可用的 HTML 页面。

hackernews · bratao · 9月2日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**背景**: Gemini Flash 是 Google 主打轻量、低成本的模型系列，适合大规模和低延迟任务。新版 Flash 被定位为近乎前沿水平、价格更低的替代品，可对标 Anthropic Opus 5 等高价旗舰模型，同时保留 Gemini 特有的多模态输入能力，支持音频和视频输入，而竞争对手旗舰目前大多只能处理图像。官方博客附有 DeepMind 模型卡片和基准测试资源链接，可进一步了解技术细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3 . 8 Flash and 3 . 8 Flash Cyber</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-8-flash/">Gemini 3 . 8 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://www.androidauthority.com/gemini-3-8-flash-google-ai-model-3706483/">Google’s Gemini 3 . 8 Flash is built to “work harder”</a></li>

</ul>
</details>

**社区讨论**: HN 评论区反响热烈：Simon Willison 展示了快速廉价的 HTML/JavaScript 生成能力，并称赞 Gemini 支持音频和视频输入；也有人指出它在 DeepSwe 等排行榜上领先，智能评分与 Opus 5 medium 持平。也有谨慎观点，认为低思考强度下相比 3.7 可能略有退步，实际体验仍有待进一步检验。

**标签**: `#AI`, `#Gemini`, `#Google`, `#LLM`, `#announcement`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude Fable 5.1；鹈鹕测试暴露推理设置怪象](https://simonwillison.net/2026/Sep/1/claude-fable-5-1/) ⭐️ 9.0/10

Anthropic 发布了 Claude Fable 5.1（以及 Mythos 5.1），在新基准 Terminal-Bench-Science 0.1 上取得 52.6% 的成绩，高于 Fable 5 的 24.7%。随后 Simon Willison 让该模型在不同推理级别下生成“骑自行车的鹈鹕”SVG 图像，以进行测试。 此次发布意义重大，因为它是 Anthropic 的一次重大模型更新，在智能体科学研究基准上取得了显著提升。Willison 的实际测试独立展示了新的推理级别设置在创意代码生成任务上的表现，这对于评估模型真实行为的开发者很重要。 Claude Fable 5.1 提供 low、medium、high、xhigh、max 五个推理级别，且无法完全关闭推理。在 Willison 的测试中，对于简单的 SVG 提示，low 和 medium 设置都输出了约 1,990 个 token 且没有可见的推理痕迹，说明模型可能跳过了推理；而 high 设置则启用了推理并输出更多 token。

rss · Simon Willison · 9月1日 23:57

**背景**: “骑自行车的鹈鹕”基准是 Simon Willison 在 2024 年底创建的非正式 LLM 测试：它要求模型根据这一简单提示生成 SVG 图像，从而考察模型的指令遵循、代码生成和视觉构图能力。Terminal-Bench-Science 0.1 是一个全新的智能体基准，于 8 月 27 日首次发布，用于评估 AI 智能体在跨科学领域的长期研究流程中的表现，而不仅仅是简单的单轮问答。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rdworldonline.com/anthropic-doubles-a-science-benchmark-score-with-fable-5-1-while-openai-says-its-astra-models-crosses-critical-cyber-threshold/">Anthropic doubles a science benchmark score with Fable 5.1 while...</a></li>
<li><a href="https://www.terminal-bench-science.ai/">TERMINAL - BENCH - SCIENCE</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#benchmarks`, `#model release`

---

<a id="item-3"></a>
## [Meta 发布 Muse Spark 1.3：低价编程模型登顶 DeepSWE](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta 于 2026 年 9 月 2 日发布 Muse Spark 1.3，这是其编码模型系列五个月内的第三个版本。它在 DeepSWE 基准上取得 75.4 分，评论者称这是目前公开的最佳成绩；输入每百万 token 1.25 美元、输出每百万 token 4.25 美元。 这一发布表明，低价模型也能达到接近前沿的智能体编码水平，加剧了与 Gemini 3.8 Flash、Claude 等产品的竞争。它为开发者提供了面向智能体编码工作流的廉价选择，并可能压低整个行业的模型价格。 该模型是多模态推理模型，上下文窗口为 1,048,576 token，面向长时间运行的智能体、多智能体与编码工作流。它同时驱动 Meta 的 Muse Code 终端智能体，并可通过 Meta 模型 API 和 OpenRouter 使用。

hackernews · bvaldivielso · 9月2日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**背景**: Muse Spark 是 Meta 专为编码和智能体任务打造的 AI 模型系列，1.3 是该系列五个月内推出的第三个版本。DeepSWE 是 Datacurve 开发的长期软件工程基准，用于衡量编程智能体能否端到端自主解决活跃开源仓库中的真实问题，每个任务都在没有互联网的隔离容器中执行。这类基准之所以重要，是因为现有公共榜单在前沿模型层面开始饱和。极低的 token 价格和百万级上下文窗口已成为编码模型市场的关键竞争点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/meta/muse-spark-1.3">Muse Spark 1 . 3 - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE</a></li>
<li><a href="https://pasqualepillitteri.it/en/news/14145/meta-muse-spark-1-3-coding-model">Meta ships Muse Spark 1 . 3 , its biggest coding jump yet</a></li>

</ul>
</details>

**社区讨论**: 讨论整体积极且偏重实操：simonw 发现 Muse Spark 1.3 在生成 SVG 时明显优于 1.2，单次运行成本仅约 4.2 美分；bertili 则指出 DeepSWE 75.4 分是目前公开最佳成绩，超过了 Google 的 Gemini 3.8 Flash。也有用户在询问实际接入方式，例如将 Claude Code 指向 Muse Spark 还是使用 Meta 自家的 Muse Code；superfrank 则分享说，若允许 Meta 用用户数据训练，Spark 1.2 在日常开发中非常便宜且好用。

**标签**: `#AI`, `#machine learning`, `#Meta`, `#coding assistant`, `#model release`

---

<a id="item-4"></a>
## [报告：三个网站生成 215,128 个“最佳软件”页面，被 Perplexity 大规模引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

Trellner 的一份新报告显示，仅三个网站就通过程序化方式生成了 215,128 个“最佳软件”对比页面，而 Perplexity 的 AI 回答经常将这些页面作为来源引用。 这一发现表明，AI 搜索引擎容易受到低质量批量生成内容的影响，这可能降低答案可靠性，并在内容农场与大语言模型之间形成反馈循环。这也提醒企业和内容方必须认真关注自己在 AI 生成答案中的呈现方式。 该报告聚焦于程序化 SEO 页面——这类页面利用模板和结构化数据批量生成，以规模化覆盖搜索查询，并且往往追求生成式引擎优化（GEO）。这一调查规模表明，基于模板批量生成的页面即使缺乏真正的人工编辑内容，也可能主导 AI 的引用来源。

hackernews · jakobgreenfeld · 9月2日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**背景**: 程序化 SEO（Programmatic SEO）是一种利用模板和结构化数据自动创建大量网页，以规模化覆盖各种搜索查询的技术。生成式引擎优化（GEO）则是优化内容，使其更容易被 Perplexity、ChatGPT、Google AI Overviews 等 AI 搜索系统理解、信任并引用的相关做法。这两种手段叠加，会使批量生产、投入极低的页面更容易出现在 AI 回答中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.semrush.com/blog/programmatic-seo/">What Is Programmatic SEO? Examples + How to Do It</a></li>
<li><a href="https://www.brafton.com/what-is-generative-engine-optimization/">What Is Generative Engine Optimization ( GEO )? | Brafton</a></li>

</ul>
</details>

**社区讨论**: 评论区整体表达担忧，用户指出大语言模型似乎更偏爱 AI 生成的内容，有时会凭空编造不存在的地点，并且 Perplexity 为了追求速度导致结果质量下降。还有人补充说，AI 智能体对已发布信息来源背后的动机缺乏质疑，但他们认为这个缺陷会随着时间推移得到改进。

**标签**: `#AI`, `#search`, `#content-farms`, `#LLM`, `#hallucination`

---

<a id="item-5"></a>
## [Jasper Research 发布从零训练文生图模型的详细指南](https://www.reddit.com/r/MachineLearning/comments/1w5c9rd/detailed_explanation_of_how_to_create_a/) ⭐️ 8.0/10

Jasper Research 发布了一份技术手册和开源代码库，详细讲解如何从零构建文生图（text-to-image）模型。该发布包含名为 MONET 的 1 亿张精选图文数据集，以及一套极简的 nano-t2i 代码库，用于端到端训练一个小型 flow-matching 模型。 该资源降低了实践者理解和复现现代文生图流程的门槛，这类流程通常被视为专有的黑盒。它分享了完整思路、中间结果、大型数据集以及可在单块 H200 GPU 上以不到 300 美元成本运行的代码，使前沿风格的训练对个人和小型实验室变得可行。 nano-t2i 仓库被描述为一套极简、可修改、开放（Apache-2.0）的代码库，用于在 MONET 数据集上训练文生图 flow-matching 模型。MONET 的全称是 Massive, Open, Non-redundant and Enriched Text-to-image dataset，该手册则以交互式技术报告的形式托管在 Hugging Face Spaces 上。

reddit · r/MachineLearning · /u/dh7net · 9月2日 14:40

**背景**: 文生图模型通过在海量图文对（image-text pairs）上训练，学习根据自然语言描述生成图片。所谓“从零构建”这类模型，是指自己设计和训练架构与数据流程，而不是在已有模型上进行微调。Flow matching 是一种较新的生成模型训练范式，它通过简单的回归目标学习把噪声转换为数据，而 MONET 为这种训练提供了大规模精选数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/gojasper/nano-t2i">GitHub - gojasper/ nano - t 2 i : Minimal training code of a nano...</a></li>
<li><a href="https://huggingface.co/datasets/jasperai/monet">jasperai/monet · Datasets at Hugging Face</a></li>

</ul>
</details>

**标签**: `#text-to-image`, `#deep learning`, `#generative models`, `#open source`, `#tutorial`

---

<a id="item-6"></a>
## [开源 AI 检测器在实际基准测试中难以达到 0.5%假阳性率](https://www.reddit.com/r/MachineLearning/comments/1w58erw/most_opensource_ai_detectors_cant_hold_a_05/) ⭐️ 8.0/10

一项针对六款开源 AI 文本检测器的公开基准测试发现，大多数检测器无法维持 0.5%的假阳性率，其中旧版 OpenAI RoBERTa 检测器的 AUC 仅为 0.31，比抛硬币还差。表现最好的模型 tropa-mini 能识别 93.2%的未改写 AI 文本，但对经过 humanizer 改写的文本识别率仅为 41.6%，对前沿模型输出仅为 33.6%。 这一结果对开源 AI 检测器在教育、内容审核等实际场景中的可靠性提出了质疑，而 0.5%的假阳性率是常见的业务要求。测试还暴露了系统性偏见：所有被测模型对非英语母语者作文的误判率都高于英语母语者，这引发了人们对这类工具部署公平性的担忧。 该评估仅使用公开数据：Jabarian & Imas 2025（NBER）、Liang 2023 托福作文、含 1060 篇文本的前沿模型数据组，以及 5000 篇 LLM 出现前（2018 年）的 FineWeb 网页。每个模型都在相同的 6930 篇人类文档上把阈值校准到 0.5%假阳性率，再分组测量召回率；MAGE 在任何阈值下都无法达到 0.5% FPR，因为它给 26%的普通人类网页文本打出了高于 0.9999 的分数。

reddit · r/MachineLearning · /u/grumpyp2 · 9月2日 12:04

**背景**: AI 文本检测器是一类分类器，用于区分人类撰写的文本和机器生成的文本。假阳性指人类写作被错误标记为 AI 生成；0.5%的假阳性率意味着每 200 篇人类文本中可能有 1 篇被误判。旧款检测器（如 OpenAI 的 RoBERTa 模型）是在 GPT-2 输出上训练的，难以应对现代语言模型；而“humanizer”等改写工具可以让 AI 输出规避检测。FineWeb 是一个包含 15 万亿 token 的网页级数据集，在本基准中用作 LLM 出现前的人类文本来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2305.13242v3">MAGE: Machine-generated Text Detection in the Wild - arXiv.org</a></li>
<li><a href="https://github.com/openai/gpt-2-output-dataset/blob/master/detector/README.md">gpt-2-output-dataset/detector/README.md at master · openai ...</a></li>
<li><a href="https://huggingface.co/spaces/HuggingFaceFW/blogpost-fineweb-v1">FineWeb: decanting the web for the finest text data at scale - a Hugging Face Space by HuggingFaceFW</a></li>

</ul>
</details>

**标签**: `#AI detection`, `#evaluation`, `#machine learning`, `#benchmark`, `#bias`

---

<a id="item-7"></a>
## [英伟达发布 DLSS 5 神经渲染，9 月 3 日随 NBA 2K27 上线](https://www.nvidia.com/en-us/geforce/news/dlss-5-3d-guided-neural-rendering/) ⭐️ 8.0/10

英伟达正式发布 DLSS 5，引入 3D 引导神经渲染，利用 AI 实时生成光影与材质细节。该功能将于太平洋时间 9 月 3 日晚 9 点随《NBA 2K27》一同上线，适用于 GeForce RTX 50 系列 PC、笔记本及 GeForce NOW Ultimate 会员。 DLSS 5 标志着从重建已有画面转向生成新的视觉细节，有望在不牺牲性能的情况下提升画质。该技术首发即登陆《NBA 2K27》和 GeForce NOW，意味着大量玩家可能比竞争技术普及更早体验到 AI 驱动的渲染。 英伟达称，RTX 5090 在 4K 超高画质并开启光线追踪下帧率最高可达 370 FPS，1440p 下最高可达 590 FPS。玩家需安装同日发布的新版 GeForce Game Ready 驱动，且该功能仅限 RTX 50 系列硬件或 GeForce NOW Ultimate 使用。

telegram · zaihuapd · 9月2日 03:00

**背景**: DLSS 是英伟达基于深度学习的图像技术套件，此前多个版本分别负责超分辨率、帧生成和光线追踪画质优化。神经渲染则是在渲染管线末端加入生成式 AI 模型，对已经渲染好的画面重新处理其对光线的响应，并从真实世界数据中学习视觉先验，以补充更丰富的光影和材质细节。在 DLSS 5 中，该模型利用每帧现有的颜色信息和运动矢量，实时增强光照和材质表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/geforce/news/dlss-5-3d-guided-neural-rendering/">DLSS 5: 3D-Guided Neural Rendering Debuts in NBA 2K27 | NVIDIA</a></li>
<li><a href="https://research.nvidia.com/labs/adlr/DLSS5/">DLSS 5: Generative Neural Rendering - NVIDIA ADLR</a></li>
<li><a href="https://wccftech.com/nvidia-dlss-5-neural-rendering-in-10-modern-games-the-best-unofficial-dlss-5-on-vs-off-comparisons-so-far/">NVIDIA DLSS 5 Neural Rendering In 10 Modern Games – The Best Unofficial DLSS 5 ON vs OFF Comparisons So Far</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#DLSS`, `#Neural Rendering`, `#Graphics`, `#Gaming`

---

<a id="item-8"></a>
## [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜夺冠](https://mp.weixin.qq.com/s/BfKRXMAR5ykD58LDkBftLg) ⭐️ 8.0/10

阿里通义千问发布了 Qwen3.8-Max-0902，该模型在 CodeArena 前端编程总榜上获得 1691 分，较旧版提升 22 分。该版本已上线千问 AI 平台，并接入千问办公、Qoder 与千问 APP。 这一发布凸显了 LLM 在编程能力和价格上的激烈竞争，阿里以远低于榜单第二名和第三名模型的 API 价格夺得榜首。使用编程助手的开发者和企业可能受益于以更低成本获得顶尖模型能力。 该模型拥有 2.4T 参数和 1M tokens 的上下文窗口，API 价格为每百万输入 tokens 2 美元、每百万输出 tokens 6 美元，综合均价约 5 美元。这明显低于榜单第二名和第三名模型所报道的 20 美元和 12 美元价格。

telegram · zaihuapd · 9月2日 06:05

**背景**: CodeArena 是一个在线评估平台，通过多个子任务和多种编程语言衡量 LLM 的代码生成能力，提供及时且无偏见的排行榜。后训练是指在预训练之后将基础模型转变为对齐的、能遵循指令的助手，并可针对编程等任务进行专门优化。1M tokens 的上下文窗口让模型可以在一次请求中阅读和推理非常长的输入，从而减少切分文本或单独保存摘要的需要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2503.01295">CodeArena : A Collective Evaluation Platform for LLM Code Generation</a></li>
<li><a href="https://aiwiki.ai/wiki/post-training">Post-training - AI Wiki</a></li>
<li><a href="https://bota.chat/kimi-k3/1m-token-context-window/">1 Million Token Context Window Explained: What Fits</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#Model Release`, `#Coding Benchmark`, `#Qwen`, `#Alibaba`

---

<a id="item-9"></a>
## [月之暗面与美云巨头谈判，拟按最高 30%分成授权 Kimi K3](https://www.jiemian.com/article/15040119.html) ⭐️ 8.0/10

月之暗面正与微软、亚马逊和谷歌进行早期谈判，拟以最高 30% 的收入分成授权其 Kimi K3 模型。若达成，这将成为中国 AI 公司与美国云巨头之间的首个重大模型收入分成协议。 若达成协议，将为中国开源权重 AI 模型进入西方云市场打开重要分销渠道，并为 AI 模型授权的收入分成树立新范式。这也凸显了 Kimi K3 等大型开源模型的商业价值。 谈判仍处早期阶段，核心条款未定，各方均拒绝置评。Kimi K3 于 2026 年 7 月发布，总参数达 2.8 万亿，是迄今最大的开源权重模型；截至 6 月中旬，其年度经常性收入已突破 3 亿美元。

telegram · zaihuapd · 9月2日 07:36

**背景**: 月之暗面（Moonshot AI）是一家总部位于北京的人工智能公司，也是中国六家“AI 老虎”（AI Tigers）之一。其 2026 年 7 月发布的 Kimi K3 基于 Kimi Delta Attention 与 Attention Residuals 构建，具备原生视觉能力和 100 万 token 上下文窗口，是迄今发布的最大的开源权重模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**标签**: `#AI`, `#Moonshot AI`, `#Kimi K3`, `#cloud`, `#revenue sharing`

---

<a id="item-10"></a>
## [xAI 发布 Grok 4.6，强化长时智能体任务与视觉能力](https://t.me/zaihuapd/43559) ⭐️ 8.0/10

xAI 于 2026 年 8 月 12 日发布 Grok 4.6，在 Grok 4.5 基础上重点强化长时间运行的智能体任务、交互与视觉能力。该模型在综合九项基准的 Artificial Analysis 智能指数上与 GPT-5.6 Sol 持平。 此次发布标志着 xAI 持续推进以保持与 GPT-5.6 Sol 等前沿模型的竞争力，同时推动智能体 AI 这一关键行业趋势。由于 Grok 4.6 即刻上线 Cursor、Grok Build 和 API，开发者和企业可以立即将其用于编程与智能体工作负载。 该模型定价为每百万输入 token 2 美元、输出 token 6 美元，另有双倍价格的快速版本。Artificial Analysis 智能指数包含九项基准，涵盖推理、编程、知识、指令遵循、科学推理和多步任务完成等能力。

telegram · zaihuapd · 9月2日 08:10

**背景**: 长时间运行的智能体任务是指自主多步骤工作流，通常可持续数分钟到数小时甚至数天，往往需要队列、检查点以及超出单次函数调用的基础设施。Artificial Analysis 智能指数是一个综合基准分数，用于衡量语言模型在推理、编程、知识及多步任务上的能力。Grok Build 是 xAI 基于终端的 AI 编程智能体，可将大型任务委派给并行的专门子智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index v4.1.1 | Artificial Analysis</a></li>
<li><a href="https://www.openlegion.ai/en/learn/ai-agent-long-running-tasks">AI Agent Long Running Tasks : Queues, Checkpoints... | OpenLegion</a></li>
<li><a href="https://x.ai/build">Grok Build | SpaceXAI</a></li>

</ul>
</details>

**标签**: `#Grok`, `#xAI`, `#AI model`, `#agents`, `#API`

---

<a id="item-11"></a>
## [FBI 调查暗网服务 Nexus 兜售 1.53 亿张驾照扫描件](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) ⭐️ 8.0/10

FBI 正在调查名为 Nexus 的暗网身份信息售卖服务，该平台声称掌握超过 1.53 亿张美国和加拿大居民的驾照数字扫描件并开始对外出售。KrebsOnSecurity 报道了这一进展，并指出该平台已开始兜售这些数据。 由于驾照包含姓名、住址、出生日期等敏感个人信息，这批数据可能被用于大规模身份冒用与欺诈。该事件也凸显了旧文档扫描件被汇总泄露后，在暗网市场上重新流通的持续风险。 Krebs 推测这些驾照扫描件可能来自汽车经销商、保险公司等机构此前发生的旧数据泄露。目前官方尚未确认数据的具体来源，也未公布受影响的确切人数。

telegram · zaihuapd · 9月2日 09:31

**背景**: 暗网是互联网中存在于暗网网络（darknet）之上的一部分内容，这些叠加网络需要特定软件、配置或授权才能访问。它允许私有计算机网络匿名通信和交易，也因此成为出售被盗个人数据的非法市场的温床。“暗网”常与深网（deep web）相混淆，但它特指只能通过 Tor 等工具访问的那一小部分隐藏网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_Web">Dark web - Wikipedia</a></li>
<li><a href="https://geekflare.com/guide/what-is-dark-web/">What Is Dark Web? How It Works, and Why It Exists - Geekflare</a></li>
<li><a href="https://www.security.org/identity-theft/dark-web/">What Is the Dark Web? - Security.org</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data-breach`, `#dark-web`, `#identity-theft`, `#privacy`

---