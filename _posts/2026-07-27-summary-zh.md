---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 33 条内容中筛选出 12 条重要资讯。

---

1. [Moonshot AI 发布开源 3T 参数大模型 Kimi-K3](#item-1) ⭐️ 9.0/10
2. [小型 4B 开源权重模型在瑞典医疗问答中接近 o3 水平](#item-2) ⭐️ 9.0/10
3. [谷歌透露 Gemini 4 为迄今最雄心勃勃的预训练项目，预计 2026 年底发布](#item-3) ⭐️ 9.0/10
4. [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞](#item-4) ⭐️ 9.0/10
5. [vLLM v0.26.0 支持 Inkling 和 DeepSeek-V4 优化](#item-5) ⭐️ 8.0/10
6. [美国公民因 GrapheneOS 手机在机场被搜时自动清除数据而遭指控](#item-6) ⭐️ 8.0/10
7. [形式化验证的证明自动化取得进展](#item-7) ⭐️ 8.0/10
8. [面向数据设计 PDF 导论（2004）](#item-8) ⭐️ 8.0/10
9. [欧盟提议浏览器级隐私设置取代 Cookie 横幅](#item-9) ⭐️ 8.0/10
10. [LLM 令牌转售欺诈市场内部调查](#item-10) ⭐️ 8.0/10
11. [Claude 共享对话遭搜索引擎索引，用户隐私泄露](#item-11) ⭐️ 8.0/10
12. [SpaceX 拒接 Falcon 9 订单，全力押注 Starship](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Moonshot AI 发布开源 3T 参数大模型 Kimi-K3](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

7 月 27 日，Moonshot AI 在 HuggingFace 上发布了 Kimi-K3，这是一个拥有 2.8 万亿参数的开源大语言模型。该模型基于公司自研的 Kimi Delta Attention (KDA) 混合线性注意力机制，支持 100 万 token 的上下文窗口。 Kimi-K3 是全球首个开源的三万亿参数级别模型，标志着超大规模 AI 的可及性迈出了重要一步。它的发布可能推动 AI 市场竞争，可能降低推理成本，并激发在智能编程和知识工作领域的创新。 该模型使用原生 MXFP4 量化需要约 1.5TB 显存进行部署，逼近当前硬件（如 8 块 B200 GPU）的极限。它集成了原生视觉理解能力，专为长周期编程和推理等前沿智能场景设计。

hackernews · nateb2022 · 7月27日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=49065752)

**背景**: 万亿参数级别的大语言模型需要巨大的计算资源进行训练和推理。像 Kimi-K3 这样的开源发布允许开发者和研究人员研究和微调模型，但高昂的硬件要求将其实际部署限制在资金充足的组织或云服务商手中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://www.kimi.com/en">Kimi AI with K3 | Built for Agentic Coding & Knowledge Work</a></li>

</ul>
</details>

**社区讨论**: 社区对模型表示兴奋，但主要关注实际障碍，尤其是巨大的显存需求（约 1.5TB）和托管成本。一些评论者讨论了类似模型（如 GLM-5.2）的竞争如何推动了价格下降，认为 Kimi-K3 可能进一步加速价格下滑。其他人则推测未来的硬件创新，例如用于大规模模型存储的类 ROM 芯片。

**标签**: `#AI`, `#LLM`, `#HuggingFace`, `#Moonshot AI`, `#model release`

---

<a id="item-2"></a>
## [小型 4B 开源权重模型在瑞典医疗问答中接近 o3 水平](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 9.0/10

一位开发者对 Gemma-1.5-4B 进行后训练，并在瑞典医疗执照考试数据集 MedQA-SWE 上测试了更新的 4B 模型（Gemma4-E4B、Qwen3.5-4B），最高达到 87%准确率，与 OpenAI o3 模型在相关基准上的 88%相当。 这表明小型开源权重模型在专业领域可以媲美 o3 等顶级推理模型，降低部署成本，并为瑞典语等低资源语言实现私有、高效的医疗 AI。 启用推理的 Qwen3.5-4B 达到 87%准确率；使用了 S-GRPO 论文中的早退干预来防止推理轨迹循环。尽管提示是瑞典语，模型仍用英语进行所有推理，突显了语言无关能力。

reddit · r/MachineLearning · /u/AccomplishedCat4770 · 7月26日 11:58

**背景**: Gemma 和 Qwen 等开源权重模型公开其训练参数，允许针对特定任务进行微调。OpenAI 的 o3 是一种推理模型，通过扩展思维链在基准测试中达到高准确率。MedQA-SWE 是一个瑞典医疗执照考试选择题数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_o3">OpenAI o3 - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">[2505.07686] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models Images S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models (PDF) S-GRPO: Early Exit via Reinforcement Learning in ... [PDF] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning ...</a></li>
<li><a href="https://medium.com/@kimanited73/open-weight-models-f504be677b1c">Open Weight Models . What are they, and why should you... | Medium</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#medical AI`, `#open-weight models`, `#LLM`, `#Swedish`

---

<a id="item-3"></a>
## [谷歌透露 Gemini 4 为迄今最雄心勃勃的预训练项目，预计 2026 年底发布](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 9.0/10

谷歌 CEO 桑达尔·皮查伊在 Alphabet 2026 年第二季度财报电话会议上宣布，Gemini 4 已投入训练，并称其为公司迄今为止最具雄心的预训练项目。该模型预计在 2026 年底发布，很可能在 11 月或 12 月。 这表明谷歌继续致力于用更大的基础模型引领 AI 前沿发展。Gemini 4 的发布可能会显著影响大语言模型的竞争格局，并推动向通用人工智能（AGI）的能力迈进。 皮查伊强调，谷歌将优先将算力分配给前沿 AGI 研发，以确保 Gemini 4 发布时仍处于最前沿。同时，Gemini 3.x Flash 系列将保持几乎每月一次的更新频率，重点提升智能编码等能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 预训练是大语言模型训练的第一阶段，在大量文本数据集上学习语法、事实和推理能力。预训练之后，模型会经过微调以专门处理特定任务。Gemini 是 Google DeepMind 开发的多模态大语言模型系列，是 LaMDA 和 PaLM 2 的后继者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.entrypointai.com/blog/pre-training-vs-fine-tuning-vs-in-context-learning-of-large-language-models/">Pre-training vs Fine-Tuning vs In-Context Learning of Large Language Models | Entry Point AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#large language model`, `#pre-training`

---

<a id="item-4"></a>
## [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

安全研究人员 Kirill Firsov 披露，Fastjson 1.2.68 至 1.2.83 版本存在无需 autoType 或 gadget 链即可利用的严重远程代码执行漏洞，影响 JDK 8、17 和 21。 该漏洞十分严重，因为 Fastjson 1.x 广泛用于 Java 应用，且已停止维护、无官方补丁，迫使受影响项目升级到 Fastjson 2 或采取有风险的缓解措施。 该漏洞无需开启 autoType 或依赖 classpath 中的特定 gadget 链，从而在 JDK 8/17/21 上更容易利用。Fastjson 1.x 已于 2024 年 10 月停止维护，因此预计不会有官方修复。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson 是阿里巴巴开发的流行 Java JSON 序列化/反序列化库。反序列化漏洞通常依赖“gadget 链”——一组能导致任意代码执行的类序列。“autoType”是 Fastjson 的一项功能，允许通过 JSON 指定目标类型，这曾是之前 CVE 的常见攻击向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson">GitHub - alibaba/fastjson: FASTJSON 2.0.x has been released ...</a></li>
<li><a href="https://www.klogixsecurity.com/scorpion-labs-blog/gadget-chains">Java Deserialization Gadget Chains</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/enable_autotype">enable_autotype · alibaba/fastjson Wiki · GitHub</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Fastjson`, `#RCE`, `#Java`

---

<a id="item-5"></a>
## [vLLM v0.26.0 支持 Inkling 和 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 新增对 Inkling 模型族的支持，通过专用内核提升 DeepSeek-V4 性能，并允许按 KV-cache 组选择注意力后端。 此版本大幅扩展了 vLLM 的模型覆盖范围，支持前沿的 Inkling 模型，并为 DeepSeek-V4 提供了关键延迟优化，惠及部署大规模推理的 AI 从业者。灵活的注意力机制也为结合滑动窗口和全注意力的混合模型铺平了道路。 此版本包含来自 212 位贡献者的 411 次提交，特性包括通过 head_dtype 实现 fp32 lm_head、KV 卸载成熟以及支持多模态视频/音频的 Rust 前端。特别地，它为 Inkling 家族引入了分段式 CUDA 图支持和 ModelOpt NVFP4 量化。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，使用 PagedAttention 管理 GPU 内存。Inkling 模型是 Thinking Machines Lab 于 2026 年 7 月发布的开源权重多模态基础模型，支持文本、图像和音频输入。NVFP4 量化通过使用 4 位浮点权重减少内存占用，常用于在 NVIDIA GPU 上部署大型模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.sglang.io/docs/sglang-diffusion/quantization">Quantization - SGLang Documentation</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#open-source`

---

<a id="item-6"></a>
## [美国公民因 GrapheneOS 手机在机场被搜时自动清除数据而遭指控](https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html) ⭐️ 8.0/10

一名美国公民的 GrapheneOS 手机在美国机场边境搜查时自动清除数据，随后其面临指控。此事凸显了在边境使用胁迫密码或自动清除功能的法律风险。 此案凸显了旨在保护隐私的安全功能与边境官员法律权力之间的紧张关系。它可能影响安全意识和开发者如何为过境场景进行威胁建模。 指控据称源于手机因输入胁迫密码或类似机制而触发的自动清除功能。该设备运行的是 GrapheneOS，这是一款以安全为重点、基于 Android 的操作系统，以这类隐私功能著称。

hackernews · eecc · 7月26日 22:21 · [社区讨论](https://news.ycombinator.com/item?id=49063022)

**背景**: GrapheneOS 是一款基于 Android 开源项目、注重安全与隐私的开源移动操作系统。它包含如胁迫密码等功能，可在紧急情况下清除设备数据以保护隐私。美国边境官员拥有搜查电子设备的广泛权力，干扰此类搜查可能导致指控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：一些人强调用户必须承担使用胁迫密码的法律后果，而另一些人则指出需要更好的威胁建模和替代隐私工具，如 VeraCrypt 的隐藏卷。还讨论了在边境安全实践与法律合规之间的平衡。

**标签**: `#GrapheneOS`, `#privacy`, `#border search`, `#security`, `#legal`

---

<a id="item-7"></a>
## [形式化验证的证明自动化取得进展](https://www.imperialviolet.org/2026/07/26/zstd-lean.html) ⭐️ 8.0/10

这很重要，因为形式化验证提供了强大的正确性保证，但成本过高；使其更便宜和更自动化可以显著提高整个行业的软件安全性和可靠性。 文章指出，由于不可判定性，证明自动化具有根本性挑战，但近期进展（如 Verus、LLM 引导的证明）显示出前景。成本比较表明，对于某些项目，自动化可以将验证工作量从 20 倍降低到接近开发水平。

hackernews · zdw · 7月26日 20:53 · [社区讨论](https://news.ycombinator.com/item?id=49062291)

**背景**: 形式化验证使用数学证明来确认软件是否符合其规范。传统上，它需要大量的人工工作——通常是开发量的 10-20 倍。证明自动化旨在通过 Coq、Lean 以及现在的 LLM 辅助推理等工具来减轻这一负担，使验证更加普及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2512.09758">Towards Language Model Guided TLA+ Proof Automation</a></li>
<li><a href="https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html">Prediction: AI will make formal verification go mainstream — Martin...</a></li>
<li><a href="https://veriprajna.com/services/formal-verification-proof-automation">Formal Verification & Proof Automation for AI | Veriprajna</a></li>

</ul>
</details>

**社区讨论**: 评论者看法不一：有人认为依赖类型和全函数在维护方面无法扩展（el_pollo_diablo），而另一些人认为 LLM 将使程序员能够自动编写形式规范与证明（gz09）。另一位评论者强调了 LLM 反向实现功能的风险，表明验证是必要的。

**标签**: `#formal verification`, `#security`, `#programming languages`, `#software engineering`

---

<a id="item-8"></a>
## [面向数据设计 PDF 导论（2004）](https://www.gamedevs.org/uploads/introduction-to-data-oriented-design.pdf) ⭐️ 8.0/10

一篇由 Mike Acton 于 2004 年发布的基础 PDF 演示文稿介绍了面向数据设计（DOD），这是一种面向性能的编程方法，优先考虑数据的布局而非面向对象的抽象。 面向数据设计在游戏开发和系统编程中因优化 CPU 缓存使用而产生深远影响，这份文档仍是塑造现代性能工程的经典参考资料。 该 PDF 强调通过首先定义数据结构和转换来设计算法，从而产生缓存友好的代码；但一些社区成员指出，实际需求经常变化，使 DOD 在演进项目中难以持续。

hackernews · tosh · 7月26日 18:11 · [社区讨论](https://news.ycombinator.com/item?id=49060724)

**背景**: 面向数据设计是一种编程方法，专注于内存中的数据布局和高效处理，特别是避免 CPU 缓存未命中。它与面向对象设计形成对比，后者通常将相关数据分散在对象中。DOD 在性能至关重要的游戏开发中变得流行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data - oriented design - Wikipedia</a></li>
<li><a href="https://medium.com/mirum-budapest/introduction-to-data-oriented-programming-85b51b99572d">Introduction to Data - Oriented Design | by Tamás Losonczi | Medium</a></li>
<li><a href="https://stackoverflow.com/questions/1641580/what-is-data-oriented-design">What is data oriented design ? - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: 评论表现出热情与谨慎并存：dustbunny 解释了数据优先算法设计的核心原则；ghosty141 警告频繁的需求变更会破坏 DOD 的假设；ChicagoDave 认为复杂系统中领域应拥有自己的数据；PessimalDecimal 指出 DOD 似乎是缓存感知算法的重新包装。

**标签**: `#data-oriented design`, `#software engineering`, `#game development`, `#performance optimization`

---

<a id="item-9"></a>
## [欧盟提议浏览器级隐私设置取代 Cookie 横幅](https://killthecookiebanner.eu/) ⭐️ 8.0/10

欧盟委员会提出一项新规，允许用户在浏览器中一次性设置隐私偏好，从而消除每个网站上的 Cookie 横幅。 如果实施，这将通过将同意权从单个网站转移到浏览器标准，大幅改善用户体验和隐私合规性，减少烦恼并提高透明度。 该提案基于现有的退出信号如 Global Privacy Control（GPC），但将使浏览器级偏好对欧盟所有网站具有法律约束力。

hackernews · rapnie · 7月26日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49057175)

**背景**: Cookie 横幅是欧盟电子隐私指令要求的，用于获取跟踪 Cookie 的同意，但被批评为侵入性强且效果不佳。浏览器级偏好如 GPC 已经作为技术机制存在，新法规将将其编纂为法律，可能完全取代横幅。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://globalprivacycontrol.org/">Global Privacy Control — Take Control Of Your Privacy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Privacy_Control">Global Privacy Control - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者支持这一举措，指出 Cookie 横幅很少构成知情同意。其他人讨论技术细节，如默认站点隔离 Cookie 和明确的跨站点共享提示。

**标签**: `#privacy`, `#cookie banners`, `#EU regulation`, `#web standards`, `#user experience`

---

<a id="item-10"></a>
## [LLM 令牌转售欺诈市场内部调查](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard 的调查揭示了中国的一个市场，通过 one-api 和 new-api 等代理工具汇集 API 密钥，滥用免费试用和窃取的凭证，以折扣价转售 LLM 令牌。 这个市场暴露了一个复杂的欺诈生态系统，增加了 LLM 提供商和合法用户的安全风险，凸显了改善 API 密钥管理和严格支出上限的紧迫需求。 这些代理主要使用 one-api 及其分支 new-api 等开源工具，这些本是合法的 API 网关却被滥用于欺诈。买家寻求更便宜的令牌、绕过地域限制或进行模型蒸馏。

rss · Simon Willison · 7月26日 19:30

**背景**: LLM API 密钥用于验证对 GPT-4 等模型的访问，通常每个密钥有速率限制。API 密钥池化技术汇集多个密钥以绕过这些限制。转售市场利用免费试用、未受保护的端点和被盗信用卡收集密钥，并以折扣价转售访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/songquanpeng/one-api/blob/main/README.en.md">one-api/README.en.md at main · songquanpeng/one-api</a></li>
<li><a href="https://github.com/QuantumNous/new-api">GitHub - QuantumNous/new-api: A unified AI model hub for aggregation & distribution. It supports cross-converting various LLMs into OpenAI-compatible, Claude-compatible, or Gemini-compatible formats. A centralized gateway for personal and enterprise model management. 🍥</a></li>
<li><a href="https://keyd.cloudwaddie.com/">Credit-based API key pooling platform</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#fraud`, `#LLM`, `#API`

---

<a id="item-11"></a>
## [Claude 共享对话遭搜索引擎索引，用户隐私泄露](https://search.brave.com/search?q=site%3Aclaude.ai%2Fshare&amp;source=android) ⭐️ 8.0/10

数百个 Claude AI 共享对话链接已被 Google 和 Bing 等搜索引擎索引，导致 API 密钥、社会安全号码和公司内部文件等敏感数据未经用户同意被公开。 这一隐私漏洞使无数用户面临身份盗窃和企业间谍风险，任何人通过搜索即可访问私人对话。同时也凸显了 AI 聊天平台中的重复性问题——一年前 ChatGPT 出现类似问题并已修复，但 Anthropic 尚未解决。 Google 目前已屏蔽这些被索引的页面，但 Brave 和 Bing 仍在搜索结果中显示。据研究，约 600 条 Claude 对话被 Google 索引，而超过 143,000 条 AI 聊天记录存储在 Archive.org 上。

telegram · zaihuapd · 7月26日 11:16

**背景**: Claude 是 Anthropic 开发的 AI 助手，提供通过公开链接分享对话的功能。用户分享链接时，内容本应对收到链接的人保密，但如果页面缺少'noindex' HTML 元标记，搜索引擎就可以抓取并索引它，使其可被公开搜索。'noindex'标签指示搜索引擎不要将页面包含在索引中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://startupfortune.com/claude-shared-chats-have-been-indexed-by-google-and-anyone-with-a-search-bar-can-find-them/">Claude shared chats have been indexed by Google and anyone ...</a></li>
<li><a href="https://thecybersecguru.com/news/claude-shared-chats-google-search-privacy/">Claude Shared Chats Indexed by Search Engines Raise Privacy ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#Claude`, `#Anthropic`, `#search engine`

---

<a id="item-12"></a>
## [SpaceX 拒接 Falcon 9 订单，全力押注 Starship](https://www.bloomberg.com/news/articles/2026-07-23/spacex-is-turning-away-falcon-customers-in-major-bet-on-starship) ⭐️ 8.0/10

SpaceX 已开始拒绝卫星运营商 2028 年后的专用 Falcon 9 发射请求，并不再接受拼单任务的新预订，同时缩减部分非重复使用 Falcon 部件的生产，以加速向 Starship 过渡。 这一战略转变可能导致如果 Starship 无法在 2028 年底前投入商业运营，许多太空公司将面临发射能力缺口，影响卫星运营商、政府任务以及整个商业航天市场。 SpaceX 仍可能为美国国防部和 NASA 保留 Falcon 9 任务，但 Starship 的延误已导致 SpaceX 自 2026 年 6 月 IPO 以来股价下跌约 25%。

telegram · zaihuapd · 7月26日 12:42

**背景**: Falcon 9 是 SpaceX 的主力可重复使用火箭，多年来主导了商业发射市场。Starship 是下一代完全可重复使用的超重型运载火箭，旨在将大型载荷和宇航员送往月球、火星及更远目的地，但尚未投入商业运营，且测试屡遭延误。

**标签**: `#SpaceX`, `#Starship`, `#Falcon 9`, `#space launch`, `#strategic shift`

---