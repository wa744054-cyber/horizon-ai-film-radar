---
layout: default
title: "Horizon Summary: 2026-08-29 (ZH)"
date: 2026-08-29
lang: zh
---

> 从 30 条内容中筛选出 12 条重要资讯。

---

1. [GLM-5.3 开源权重模型发布获好评](#item-1) ⭐️ 9.0/10
2. [Triton 3.8.0 发布，带来聚合类型与 tl.topk 增强](#item-2) ⭐️ 8.0/10
3. [GUI 应完全支持键盘驱动：无障碍与效率的呼声](#item-3) ⭐️ 8.0/10
4. [Htmx 4.0 发布，为超媒体驱动的 Web 树立里程碑](#item-4) ⭐️ 8.0/10
5. [美国将意大利托管集体 A/I 列为全球恐怖分子](#item-5) ⭐️ 8.0/10
6. [现在，一条漏洞传闻就足以让人找到利用方法](#item-6) ⭐️ 8.0/10
7. [Luanti 因无根据的 AI 版权通知被 Google Play 下架](#item-7) ⭐️ 8.0/10
8. [微型潜流 Transformer 在 RP2350 上生成 128x128 人脸图像](#item-8) ⭐️ 8.0/10
9. [腾讯发布混元 Hy4 Preview，盲测成绩略胜竞品](#item-9) ⭐️ 8.0/10
10. [长鑫科技 2026 年上半年净利 776 亿元，同比扭亏为盈](#item-10) ⭐️ 8.0/10
11. [Z.ai 发布 GLM-5.3-Flash：激活参数 18B，价格降为十分之一](#item-11) ⭐️ 8.0/10
12. [OpenAI 因 SpaceX 收购 Cursor，将于 2026 年 11 月停止提供模型](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GLM-5.3 开源权重模型发布获好评](https://huggingface.co/zai-org/GLM-5.3) ⭐️ 9.0/10

Z.ai 在 Hugging Face 上以开放权重形式发布了 GLM-5.3，该模型基于与 GLM-5.2 相同的基础模型，所有改进均来自后训练阶段。此次发布重点提升了复杂软件工程和智能体能力。 GLM-5.3 提供了具有竞争力的开源权重模型替代方案，社区反馈强调其性能与效率。此次发布可能加速开源权重模型在实际应用中的采用，并加剧 AI 生态系统的竞争。 GLM-5.3 与 GLM-5.2 使用相同的基础模型，所有性能提升均来自后训练技术而非新的预训练。该模型提供多种量化版本，可用于 llama.cpp、Ollama 和 LM Studio 等工具，并已于 2026 年 8 月 14 日发布。

hackernews · jeudesprits · 8月28日 15:20 · [社区讨论](https://news.ycombinator.com/item?id=49479878)

**背景**: 开源权重模型是指核心参数公开发布的 AI 模型，任何人都可以下载、微调和部署。Z.ai 的 GLM 系列以提供高性能的开源权重大语言模型而闻名。后训练是指在初始预训练之后应用的技术，如监督微调和强化学习，以优化模型行为和能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://kie.ai/blog/what-is-glm-5-3">What Is GLM - 5 . 3 ? Z.ai's Next Open-Weight Model</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">zai-org/ GLM - 5 . 3 · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者称赞了 GLM-5.3 的性能和效率，有人指出它在处理复杂问题方面优于 DeepSeek Flash 等类似模型。其他人则强调其实用优势，如资源需求更低、定价更有竞争力，还有人将其输出质量与 Opus 4.8 等专有模型相媲美。

**标签**: `#AI/ML`, `#open-weights`, `#large-language-model`, `#release`, `#GLM`

---

<a id="item-2"></a>
## [Triton 3.8.0 发布，带来聚合类型与 tl.topk 增强](https://github.com/triton-lang/triton/releases/tag/v3.8.0) ⭐️ 8.0/10

Triton v3.8.0 已发布，将 @triton.aggregate 和 @gluon.aggregate 变为公共 API，并为 tl.topk 增加了 descending 参数。该版本还包含多项后端、编译器和基础设施改进。 Triton 是一种广泛使用的类 Python GPU 编程语言，此版本同时提升了开发者的生产效率和编译器功能。聚合类型简化了内核参数传递并提高了可读性，而 topk 的 descending 选项则扩展了其在机器学习和数据处理工作负载中的适用性。 聚合类型支持继承字段、默认值、自动生成的构造函数、不可变实例以及 aggregate_replace() 操作。将 tl.topk 的 descending 设置为 False 可返回最小值而非最大值；其他更改包括修复 GFX950 BF16 错误编译的 LLVM 更新，以及扩展的多 CTA 支持。

github · warrendeng · 8月28日 18:25

**背景**: Triton 是一种使用类 Python 语法编写 GPU 内核的领域专用语言和编译器，常用于深度学习框架。tl.topk 函数传统上返回张量在某个维度上的 k 个最大元素，而新的 descending 参数增加了灵活性。@triton.aggregate 装饰器将此前内部的聚合数据类型正式化，使得向内核传递结构化数据更加方便。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://triton-lang.org/main/python-api/generated/triton.language.topk.html">triton.language. topk — Triton documentation</a></li>
<li><a href="https://github.com/triton-lang/triton/issues/8781">[Frontend] OOP + aggregate in triton/gluon · Issue #8781 · triton-lang/triton</a></li>

</ul>
</details>

**标签**: `#Triton`, `#GPU`, `#Compiler`, `#AI/ML`, `#Release`

---

<a id="item-3"></a>
## [GUI 应完全支持键盘驱动：无障碍与效率的呼声](https://ckardaris.com/blog/2026/08/28/keyboard-driven-guis.html) ⭐️ 8.0/10

这篇博文主张图形用户界面不应只依赖鼠标，而应设计为可以完全通过键盘操作，以提升无障碍性和可用性。该观点在 Hacker News 上引发热议，获得 653 分和 322 条评论，讨论其实现难点与好处。 键盘驱动的 GUI 之所以重要，是因为许多用户（包括行动或视觉障碍者以及高效用户）不使用鼠标导航，不友好的界面会把他们排斥在外。这场讨论促使设计师和框架开发者将键盘导航视为核心需求，而不是事后的补救项。 实现细节包括焦点管理技术（如 roving tabindex）、保持合理的 Tab 顺序，以及避免“键盘陷阱”（用户无法将焦点移出某个控件）。作者和评论者也指出，只有当应用遵循标准的焦点行为时，Tab、方向键和 Enter 才能作为通用的系统级导航方式。

hackernews · ckardaris · 8月28日 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49479837)

**背景**: 键盘无障碍是 Web 和桌面无障碍标准（如 WCAG 的“无键盘陷阱”准则）的核心要求。在菜单、列表框、工具栏等复合控件中，开发者常用 roving tabindex 模式：Tab 顺序中只有一个元素为 tabindex=0，其余元素通过方向键移动焦点。如果焦点管理不细致，自定义控件对仅使用键盘的用户（尤其是依赖屏幕阅读器等辅助技术的用户）将变得无法使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stefanjudis.com/today-i-learned/roving-tabindex/">What's 'roving tabindex'? | Stefan Judis Web Development</a></li>
<li><a href="https://www.boia.org/blog/why-keyboard-traps-are-one-of-the-most-frustrating-accessibility-issues">Why Keyboard Traps Are One of the Most Frustrating Accessibility ...</a></li>
<li><a href="https://accessibility-test.org/blog/development/interactive-aria-widgets-implementation-guide-for-developers/">Interactive ARIA Widgets | Implementation Guide for Developers</a></li>

</ul>
</details>

**社区讨论**: 评论者大多支持键盘无障碍，但在程度上存在分歧。一位评论者敦促开发者用屏幕阅读器和键盘测试应用，指出一次错位的 Tab 顺序就可能让残障用户“撞墙”；另一位将忽视键盘支持归咎于流行的 UI 框架。也有反对声音认为，高效用户的需求不等于普通用户体验，强迫所有人都使用键盘驱动 GUI 忽略了普通用户的学习曲线。

**标签**: `#accessibility`, `#keyboard navigation`, `#GUI design`, `#software usability`

---

<a id="item-4"></a>
## [Htmx 4.0 发布，为超媒体驱动的 Web 树立里程碑](https://four.htmx.org/announcements/2026-08-28-htmx-4.0.0-is-released) ⭐️ 8.0/10

Htmx 4.0.0 于 2026 年 8 月 28 日发布，这是面向超媒体的 JavaScript 库的一次重大版本更新。这次发布标志着这个流行的开源项目的重要里程碑。 Htmx 已在希望采用更简单、对服务端渲染友好的前端架构的开发者中获得了广泛采用。这次重大版本发布再次印证了超媒体方法作为复杂单页应用框架可行替代方案的地位。 htmx 是一个体积小（压缩后约 14k）、无依赖的库，可通过 HTML 属性直接使用 AJAX、CSS 过渡、WebSocket 和 Server-Sent Events。4.0 版本包含了 hx-alpine-compat，用于解决与 Alpine.js 的兼容性问题。

hackernews · rmsaksida · 8月28日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=49478178)

**背景**: htmx 是一个开源 JavaScript 库，通过自定义属性扩展 HTML，让开发者无需编写 JavaScript 即可使用 AJAX、CSS 过渡、WebSocket 和 Server-Sent Events。它体现了超媒体理念，常与 HATEOAS（超媒体作为应用状态引擎）相关联，并作为 intercooler.js 的改进版本而诞生。超媒体是指包含指向其他媒体链接的内容，构成了现代 Web 的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>
<li><a href="https://en.wikipedia.org/wiki/Htmx">htmx - Wikipedia</a></li>
<li><a href="https://hypermedia.systems/hypermedia-a-reintroduction/">Hypermedia: A Reintroduction</a></li>

</ul>
</details>

**社区讨论**: 社区反响总体积极，开发者称赞 htmx 的简单性和使用乐趣，公司 CEO 在评论中披露了自己的身份。一位评论者提出相反观点，认为将表现层与后端逻辑混在一起让 .NET/Angular 开发变得更困难。还有人提到尝试了 Alpine AJAX 等替代方案，并指出 htmx 对 Datastar 等项目的影响。

**标签**: `#htmx`, `#frontend-development`, `#web-development`, `#hypermedia`, `#open-source`

---

<a id="item-5"></a>
## [美国将意大利托管集体 A/I 列为全球恐怖分子](https://www.inventati.org/) ⭐️ 8.0/10

美国国务院将 Autistici/Inventati（A/I 集体）列为“特别指定全球恐怖分子”，该意大利集体运营 autistici.org 和 noblogs.org。此举相当于制裁一家互联网基础设施与托管服务商，据称是此类指定中的首例。 以恐怖主义认定来针对托管和隐私基础设施服务商，为美国施压活动人士所用服务开创了危险先例。这可能对数字权利、言论自由以及更广泛的互联网治理生态产生寒蝉效应，影响从博主到隐私工具开发者等各类人群。 美国国务院声称 A/I 为暴力“反法”（Antifa）小组和极左激进分子构建并运营数字基础设施。A/I 于 2001 年由自治反资本主义运动创立，为活动人士提供邮箱、托管以及基于 WordPress 的匿名博客平台 Noblogs；截至报道时，autistici.org 已无法访问，noblogs.org 部分功能失常。

hackernews · exiguus · 8月28日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49477854)

**背景**: “特别指定全球恐怖分子”（SDGT）是美国的一种制裁工具，用以冻结指定实体的财产并禁止美国人与之交易。Autistici/Inventati 是 2001 年诞生的意大利集体，为草根和社会运动活动人士提供电子邮件、邮件列表和匿名博客等互联网服务。其 Noblogs 平台允许匿名发布且不记录 IP，因此被许多独立博主广泛使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesperson/2026/08/designation-of-autistici-inventati-as-a-specially-designated-global-terrorist">Designation of Autistici/Inventati as a Specially Designated Global Terrorist - United States Department of State</a></li>
<li><a href="https://www.autistici.org/about">autistici.org - Who we are</a></li>
<li><a href="https://noblogs.org/">NoBlogs.org</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧明显：一些人称这一认定前所未有且令人担忧，质疑 I2P、Monero、Veilid、Tox 或 Signal 的用户和开发者是否会是下一个目标。另一些人提供了历史背景，谈及 A/I 起源于 2001 年热那亚八国集团峰会抗议和 Indymedia；还有人表示对 A/I 到底做什么感到困惑；一位评论者质疑所谓与库尔德工人党（PKK）的联系，称找不到任何 A/I 托管或支持 PKK 内容的证据。

**标签**: `#sanctions`, `#privacy`, `#civil-liberties`, `#hosting`, `#internet-governance`

---

<a id="item-6"></a>
## [现在，一条漏洞传闻就足以让人找到利用方法](https://anil.recoil.org/notes/rumour-is-the-exploit) ⭐️ 8.0/10

一篇新文章认为，在 LLM 时代，仅凭一条漏洞传闻就足以快速发现并利用漏洞，从而大大扩展了漏洞利用开发的范围。作者指出，关于漏洞的传闻实际上已成为 AI 辅助漏洞利用的种子。 这一现象意义重大，因为它降低了编写可用漏洞利用代码的技能门槛，并把危险的攻击窗口扩展到了价值较低的目标上。安全团队和开源维护者现在正面临大量 AI 生成的漏洞披露和利用尝试。 这篇文章反映了一个更广泛的趋势，即 LLM 加速了 N-day 漏洞利用的开发，CISA 指出漏洞利用时间已从数月压缩到数小时。维护者也报告了现实影响：rclone 在过去一个月收到 40 多份安全披露，而该项目头十年总共只有约 20 份。

hackernews · avsm · 8月28日 15:58 · [社区讨论](https://news.ycombinator.com/item?id=49480466)

**背景**: 传统漏洞研究需要深入代码分析和人工逆向工程，才能把发现的缺陷变成可用的利用程序。如今 LLM 可以辅助代码理解、补丁分析和利用框架搭建，使这些技术更容易上手。过去需要专家知识才能处理的随口漏洞评论，现在也能快速变成具体探测手段。这改变了网络攻击的成本结构，使得低价值目标的大规模利用成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2512.22753">From Rookie to Pro: Social Engineering LLMs for Automated...</a></li>
<li><a href="https://runtimerebel.com/blog/llm-assisted-exploit-creation-claude-mythos-accelerates-n-day-attacks">LLM - Assisted Exploit Creation: Claude Mythos... | RuntimeRebel</a></li>
<li><a href="https://me.aiyu.co.in/blogs/how-frontier-llms-are-accelerating-nday-exploit-development">Aiyu | How Frontier LLMs Are Accelerating N‑Day Exploit Development</a></li>

</ul>
</details>

**社区讨论**: 维护者和安全研究人员大体认同文章观点，但也增加了更多细节：rclone 维护者表示披露数量令人应接不暇，但约 75%的披露有值得调查的内容。还有人指出，问题不仅在于发现漏洞，还在于部署和修补的速度；也有人认为这种做法在 LLM 出现之前就存在，只是现在被规模化并普及了。

**标签**: `#security`, `#LLM`, `#vulnerability research`, `#open source`, `#exploit development`

---

<a id="item-7"></a>
## [Luanti 因无根据的 AI 版权通知被 Google Play 下架](https://blog.luanti.org/2026/08/27/luanti-dmca-tracer-ai/) ⭐️ 8.0/10

2026 年 8 月 27 日，Luanti 项目宣布，其开源体素游戏引擎因 Tracer AI 提交的一份貌似无根据的 AI 生成 DMCA 通知而被 Google Play 下架。该项目正在对下架提出申诉。 这一事件表明，AI 生成的 DMCA 通知几乎无需核实就能让热门开源项目从主要分发平台下架，威胁依赖应用商店的开发者。它也为要求改革 DMCA 的呼声增添了动力，例如对恶意下架行为进行处罚。 社区成员指出，Tracer AI 曾在 2023 年向 Luanti 发出过类似通知并被成功申诉，今年还针对独立游戏 Allumeria 发出类似通知。评论者还注意到，最新通知声称适用瓦努阿图司法管辖区，而之前的通知声称适用美国，这让人质疑通知是否具有欺诈性。

hackernews · miniBill · 8月28日 06:33 · [社区讨论](https://news.ycombinator.com/item?id=49475079)

**背景**: Luanti（原名 Minetest）是一个由社区驱动的自由开源体素游戏引擎，自 2010 年开始开发，允许用户通过 Lua 脚本和内置的 ContentDB 浏览器创建和定制沙盒游戏。DMCA 下架通知是移除涉嫌侵权内容的法律请求，但 AI 工具如今可以大规模生成看似可信的通知，滥用者会利用它们进行审查、骚扰或打击竞争对手，即使实际上并不存在侵权行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Luanti">Luanti</a></li>
<li><a href="https://www.xbiz.com/features/291975/fighting-back-against-ai-fueled-fake-takedown-notices">Fighting Back Against AI -Fueled Fake Takedown Notices - XBIZ.com</a></li>
<li><a href="https://isthisscam.app/ai-generated-dmca">AI - generated DMCA notices : how to spot the fakes</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍同情 Luanti 并谴责该通知。有人提出具体改进方案，例如提交下架请求前需缴纳保证金；也有人指出 Tracer AI 屡次发送此类通知，且在瓦努阿图与美国司法管辖声明之间不一致，并建议对轻率的 DMCA 提交进行处罚。

**标签**: `#DMCA`, `#open-source`, `#AI-copyright`, `#Google Play`, `#software-licensing`

---

<a id="item-8"></a>
## [微型潜流 Transformer 在 RP2350 上生成 128x128 人脸图像](https://www.reddit.com/r/MachineLearning/comments/1w10tax/i_implemented_a_very_tiny_image_generation_model/) ⭐️ 8.0/10

开发者（u/cpldcpu）在 RP2350 微控制器上实现了一个 240 万至 400 万参数的潜流 Transformer 图像生成模型，经 int8 量化后可在约 20 秒内生成 128x128 的人脸图像。该模型完全在芯片上运行，生成的图像可以显示在显示器上或通过 USB 传输。 这表明传统上需要大型 GPU 的生成式图像模型可以被压缩到低成本、低功耗的微控制器中。它为设备端图像生成、隐私保护式生成或嵌入式创意设备等实用边缘 AI 应用打开了可能性，并可能激励更多微控制器级别的扩散/流模型。 该模型有 12 层，采用 AdaLN-Zero 条件化机制，并支持无分类器引导（CFG），显著提升了生成质量。为了适配内存，推理引擎在计算上一层的同时通过 DMA 从闪存流式读取权重；此外，ReLU²激活函数产生的稀疏性被引擎利用来跳过部分计算。

reddit · r/MachineLearning · /u/cpldcpu · 8月28日 19:48

**背景**: RP2350 是一款小型低功耗微控制器，内存非常有限且没有 GPU，因此在其上运行神经网络需要激进的压缩与流式处理技术。潜流 Transformer 将流匹配（一种学习把随机噪声转化为数据的方法）与在压缩潜空间而非原始像素上运行的 Transformer 层相结合。int8 量化把每个权重打包成 8 位整数，与 32 位浮点数相比可将内存占用减少约四倍。AdaLN-Zero 是扩散/流 Transformer 中常用的一种条件化设计，用于注入类别标签或引导强度等控制信号，同时保持训练稳定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/latent-flow-transformers-lft">Latent Flow Transformers (LFT)</a></li>
<li><a href="https://www.emergentmind.com/topics/adaln-zero-conditioning">AdaLN - Zero Conditioning in Deep Models</a></li>
<li><a href="https://www.vietanh.dev/glossary/squared-relu">What is: Squared ReLU ? | Viet-Anh on Software</a></li>

</ul>
</details>

**标签**: `#microcontrollers`, `#image generation`, `#edge AI`, `#transformers`, `#quantization`

---

<a id="item-9"></a>
## [腾讯发布混元 Hy4 Preview，盲测成绩略胜竞品](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 8.0/10

2026 年 8 月 28 日，腾讯发布了迄今最强的开源模型 Hy4 preview，拥有 770B 总参数、49B 活跃参数和 1M token 的上下文窗口。在 203 个工程任务的盲评中，Hy4 preview 以 2.99 分略胜 GLM 5.3（2.92）与 Kimi K3（2.94）。 这是中国科技巨头腾讯发布的重要开源模型，展现了与领先模型相当的性能，并提供超大上下文窗口。这可能给竞争对手带来压力，同时为开发者提供一个高性能、开放权重的新选择，适用于软件工程、科学研究等长上下文任务。 该模型采用混合专家（MoE）架构，总参数量达 770B，但每个 token 仅激活 49B 参数，在能力与效率之间取得平衡。目前已上线腾讯云、GitHub、HuggingFace、ModelScope、AtomGit 和 OpenRouter 等平台，API 定价为输入每 1M tokens 0.834 美元、输出每 1M tokens 2.501 美元。

telegram · zaihuapd · 8月28日 06:11

**背景**: 混合专家（MoE）架构将模型拆分为多个专门的“专家”子网络，并通过路由器为每个 token 仅激活其中一小部分。这使模型既能拥有很高的总参数量以实现更强的能力，又能让推理成本更接近活跃参数量。盲评是指在不告知评分者输出来自哪个模型的情况下进行打分，从而减少比较中的偏差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE)</a></li>
<li><a href="https://www.mindstudio.ai/blog/mixture-of-experts-architecture-glm-5-2-active-parameters">Mixture of Experts Architecture Explained: How GLM... | MindStudio</a></li>
<li><a href="https://medium.com/john-snow-labs/blind-testing-for-llm-evaluation-71cc5a936db9">Generative AI Lab 7.6: Blind Testing for LLM Evaluation | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#large language models`, `#open-source`, `#Tencent`, `#model release`

---

<a id="item-10"></a>
## [长鑫科技 2026 年上半年净利 776 亿元，同比扭亏为盈](https://t.me/zaihuapd/43468) ⭐️ 8.0/10

8 月 28 日，长鑫科技披露半年报：上半年实现营业收入 1503.1 亿元，同比增长 873.64%；归属于上市公司股东的净利润 776.05 亿元，而上年同期为亏损 23.32 亿元。上半年主营业务毛利率达 84.84%。 这一巨大反转使长鑫科技成为全球盈利最强的半导体公司之一，反映出 AI 需求与供给紧张共同驱动的存储芯片历史性上行周期。同时也凸显了中国在 DRAM 自给方面的快速进展，对全球存储价格以及与三星、SK 海力士、美光的竞争格局具有重大影响。 分季度看，第一季度归母净利润为 247.62 亿元，第二季度归母净利润为 528.43 亿元，环比增长 113%；经营活动现金流量净额达 1311.56 亿元，同比增长 2985.64%；基本每股收益为 1.2893 元。

telegram · zaihuapd · 8月28日 11:34

**背景**: 长鑫科技（CXMT）是中国领先的 DRAM 存储芯片制造商，前身为长鑫存储技术有限公司。公司持续扩大产能并推进工艺节点，以减少中国对进口存储芯片的依赖。本次财务暴增与 2025—2026 年存储市场超级周期相符，当时受 AI 服务器需求及主要厂商供给纪律影响，DRAM 和 NAND 价格大幅上涨。

**标签**: `#semiconductor`, `#financial-results`, `#memory-chips`, `#CXMT`, `#China-tech`

---

<a id="item-11"></a>
## [Z.ai 发布 GLM-5.3-Flash：激活参数 18B，价格降为十分之一](https://t.me/zaihuapd/43471) ⭐️ 8.0/10

Z.ai 发布了 GLM-5 系列首个原生多模态模型 GLM-5.3-Flash，这是一个总参数量 320B、激活参数仅 18B 的 MoE 模型。它在多项编程和智能体基准上超过 GLM-5.2，接近 Claude Opus 4.8，且限时 API 输入价格每百万 tokens 仅 0.075 美元，约为上代价格的十分之一。 这一发布表明，高效的 MoE 设计能够以极低的成本提供接近前沿模型的性能，可能会改变开发者选择 LLM API 的方式。激进的价格策略有望加速 GLM 模型在高并发编程和智能体场景中的采用。 GLM-5.3-Flash 总参数为 320B，但每个 token 仅激活 18B 参数，从而降低推理计算量。限时优惠价为每百万 tokens 输入 0.075 美元、缓存输入 0.015 美元、输出 0.25 美元，缓存存储暂时免费；原价则更高。

telegram · zaihuapd · 8月28日 15:32

**背景**: 混合专家（MoE）架构使用多个专门的子网络（“专家”）和一个门控机制，只为每个输入激活部分参数。稀疏 MoE 模型在推理时需要将整个网络加载到内存中，但只计算其中一小部分参数，因此“激活参数”比“总参数”更能反映计算成本。这种设计使实验室能够构建非常大的模型，同时保持每次推理的成本可控。此次价格降至上一代十分之一，与这种稀疏化带来的效率提升相吻合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gpt-news.net/why-active-parameters-matter-more-than-total-vram">Why Active Parameters Matter More Than Total VRAM – GPT News</a></li>
<li><a href="https://www.linkedin.com/pulse/mixture-experts-moearchitecture-padmashri-suresh-o5nqc">Mixture of Experts ( MoE ) architecture</a></li>
<li><a href="https://virtualizationreview.com/articles/2025/11/03/large-language-model-selection-why-the-parameter-count-isnt-everything.aspx">Large Language Model Selection -- Why the Parameter Count...</a></li>

</ul>
</details>

**标签**: `#AI`, `#GLM`, `#LLM`, `#MoE`, `#Model Release`

---

<a id="item-12"></a>
## [OpenAI 因 SpaceX 收购 Cursor，将于 2026 年 11 月停止提供模型](https://openai.com/index/our-decision-on-cursor-following-its-acquisition-by-spacex/) ⭐️ 8.0/10

OpenAI 宣布将终止向 Cursor 提供模型的合同，建议停服日期为 2026 年 11 月 12 日，理由是 SpaceX 收购 Cursor 后存在合规担忧。这一决定结束了双方近四年的合作。 这是一项重大行业动态，因为 Cursor 是最广泛使用的 AI 编程工具之一，失去 OpenAI 模型可能会重塑 AI 编程工具格局。这也凸显了企业收购和个人竞争如何能够扰乱 AI 生态系统的合作关系。 OpenAI 引用了 SpaceX 的违约记录，包括收购 Twitter 后违反合同，以及 xAI 今年早些时候在宣誓下承认违反 OpenAI 服务条款。与 Cursor 的定制协议允许在控制权变更后的限时窗口内终止合作，OpenAI 提供了合同允许的最大通知期。

telegram · zaihuapd · 8月29日 02:24

**背景**: Cursor 是由 Anysphere 开发的一款基于 Visual Studio Code 的 AI 编程编辑器，于 2026 年 8 月被 SpaceXAI 收购，而 SpaceXAI 前身是 xAI，后者在 2026 年 2 月被 SpaceX 收购。OpenAI 的这一决定反映了 OpenAI 与马斯克旗下公司之间日益紧张的关系，双方此前已有多起法律和合同纠纷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Cursor`, `#SpaceX`, `#AI tools`, `#industry news`

---