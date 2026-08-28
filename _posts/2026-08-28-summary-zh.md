---
layout: default
title: "Horizon Summary: 2026-08-28 (ZH)"
date: 2026-08-28
lang: zh
---

> 从 31 条内容中筛选出 13 条重要资讯。

---

1. [Cloudflare 优化 1.1.1.1 DNS 缓存，节省 100TB 内存](#item-1) ⭐️ 9.0/10
2. [Anthropic 开放智能体操控硬件的模型硬件标准研究预览](#item-2) ⭐️ 9.0/10
3. [小模型时代已经到来](#item-3) ⭐️ 8.0/10
4. [谷歌发布高精度语音转文本模型 Gemini-3.5-Transcribe](#item-4) ⭐️ 8.0/10
5. [Microduck：Pollen Robotics 推出的开源双足机器人平台](#item-5) ⭐️ 8.0/10
6. [法官裁定特朗普政府将 Anthropic 列入黑名单违法](#item-6) ⭐️ 8.0/10
7. [84 天完成 N64 游戏《Snowboard Kids》反编译](#item-7) ⭐️ 8.0/10
8. [谷歌发布 Gemini Omni 1.1 Flash，支持 40 秒场景扩展与 4K 视频生成](#item-8) ⭐️ 8.0/10
9. [提示注入攻击以 80%成功率突破 Claude Code 自动模式](#item-9) ⭐️ 8.0/10
10. [新基准 HarnessOpt-Bench 测试 AI 改进其他 AI 的能力](#item-10) ⭐️ 8.0/10
11. [英伟达 Q4 营收 681 亿美元超预期，下季度指引上调至 780 亿美元](#item-11) ⭐️ 8.0/10
12. [OpenAI 被曝开发常驻 Codex 代理，持续工作直至休眠](#item-12) ⭐️ 8.0/10
13. [美国国防部将 Anthropic 列入黑名单 防务公司弃用 Claude](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare 优化 1.1.1.1 DNS 缓存，节省 100TB 内存](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 9.0/10

Cloudflare 发布了一篇博客文章，详细介绍了他们如何通过优化 1.1.1.1 公共 DNS 解析器的缓存，节省了 100TB 内存。这些优化涉及重新组织 DNS RRset 在内存中的表示，并采用更紧凑的数据结构和分配策略。 这很重要，因为 1.1.1.1 是全球最大的公共 DNS 服务之一，减少 100TB 内存使用可降低运营成本和能源消耗，同时可能提升缓存性能。所展示的技术为其他构建大规模、内存受限系统的工程师提供了实用的参考。 优化包括将记录数据直接内联到 CacheEntry 结构中、将几个独立的列表合并为一个，以及使用竞技场分配。据讨论中一位评论者指出，合并列表可能会削弱 Rust 在索引越界检查方面的一些编译期安全保证。

hackernews · TangerineDream · 8月27日 17:17 · [社区讨论](https://news.ycombinator.com/item?id=49468083)

**背景**: 1.1.1.1 DNS 解析器将 DNS 响应缓存为资源记录集（RRset），即共享相同名称和类型的记录分组。在大规模部署中，这些缓存条目的内存占用可能变得非常巨大。为了减少内存，工程师使用了诸如竞技场分配等技术——将许多小分配合并成更大的块，以及 xor 过滤器——一种比广泛使用的 Bloom 过滤器更节省空间的概率数据结构，用于集合成员测试且不会产生假阴性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.dnsimple.com/articles/understanding-rrsets-rrsigs/">What Are RRSETs and RRSIGs in DNSSEC? - DNSimple Help</a></li>
<li><a href="https://arxiv.org/pdf/1912.08258">Xor Filters: Faster and Smaller Than Bloom and Cuckoo Filters</a></li>
<li><a href="https://en.wikipedia.org/wiki/Region-based_memory_management">Region-based memory management - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论普遍称赞这篇文章是系统级优化的典范。多位读者分享了自己的内存优化经验，例如使用单个大型 malloc 加载黑名单、注意结构体对齐等；同时有一位评论者担心将列表合并为一个可能会削弱 Rust 在索引方面的安全保证。

**标签**: `#DNS`, `#performance`, `#memory-optimization`, `#systems-programming`, `#Rust`

---

<a id="item-2"></a>
## [Anthropic 开放智能体操控硬件的模型硬件标准研究预览](https://www.anthropic.com/news/model-hardware-standard-research-preview) ⭐️ 9.0/10

Anthropic 推出了模型硬件标准（MHS）的研究预览，这是一份共享规范，让 AI 智能体能够安全地并行操控显微镜、液体处理器和机械臂等物理设备。设备集成时间从数周或数月缩短到数小时甚至数分钟。 这标志着 AI 从仅在软件中运行转向直接操控物理硬件，可能加速生物技术、先进制造和量子计算等领域的自动化。基因泰克、卡内基梅隆大学和 QuEra 等合作伙伴的参与表明其具有广泛的现实影响力。 据 Anthropic 介绍，MHS 可适用于任何具有可编程接口的设备。QuEra 的 AI 控制器在 99.3% 的情况下无需人工干预即可恢复量子计算机的激光锁定，Anthropic 计划在完成安全评估后将该标准开源。

telegram · zaihuapd · 8月28日 01:38

**背景**: MHS 最初是 Anthropic 与 HHMI Janelia Research Campus 的合作项目，旨在让 AI 加速科学研究。该标准将与科学、机器人、电子和制造领域的合作伙伴共同开发，之后开源。量子计算机需要精确的激光锁定，这历来需要耗费大量人工调试，而 AI 智能体很适合这类任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/model-hardware-standard-research-preview">Previewing the Model Hardware Standard \ Anthropic</a></li>
<li><a href="https://www.cnbc.com/2026/08/27/anthropic-pushes-into-physical-world-with-new-standard-to-help-ai-agents-operate-machines.html">Anthropic pushes into physical world with new standard to ...</a></li>
<li><a href="https://www.modelhardwarestandard.com/">Model Hardware Standard</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI Hardware`, `#Robotics`, `#Automation`, `#AI Agents`

---

<a id="item-3"></a>
## [小模型时代已经到来](https://calv.info/small-models-have-arrived) ⭐️ 8.0/10

文章《小模型时代已经到来》指出，小巧、快速且成本低廉的 AI 模型如今已成为许多工作负载的实用且日益受青睐的选择，标志着业界正从默认使用前沿超大模型转向更轻量的方案。 这之所以重要，是因为它反映出 AI 生态系统正日趋成熟：在部署决策中，成本效益和速度与原始能力同样重要，影响着那些希望在可控成本下规模化应用 AI 的开发者、初创企业和大型企业。 文章区分了“IQ 180”型工作（罕见的、高水平解决方案）和“token 喷射器”型工作（高容量、增量式任务），并认为小模型非常适合后者。文章还提到投资者对消费级 AI 公司稀少感到困惑，暗示专注于产品本身的逆向投资者存在机会。

hackernews · tosh · 8月27日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=49466917)

**背景**: 前沿模型是以极端规模训练、超越当前最先进性能并展现出涌现能力的通用 AI 系统。小语言模型（SLM）通常拥有少于 400 亿个参数，专为在智能手机、嵌入式系统等资源受限环境中高效运行而设计，因此部署成本更低、速度更快，并且与更大模型相比还能降低幻觉风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_language_model">Small language model - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认同这一观点，并分享了使用专用小模型来降低成本、减少幻觉的实践经验，有人指出“这更像是一种最佳实践”。其他人则讨论了高水平工作与高容量工作之间的区别，以及专注于满足真实用户需求而非与前沿实验室竞争的消费级 AI 公司的潜力。

**标签**: `#AI`, `#small language models`, `#ML deployment`, `#cost efficiency`, `#industry trends`

---

<a id="item-4"></a>
## [谷歌发布高精度语音转文本模型 Gemini-3.5-Transcribe](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/) ⭐️ 8.0/10

谷歌发布了新的语音转文本模型 Gemini-3.5-Transcribe，据称在转录准确率上超越竞品。然而，早期社区测试显示，其延迟仍落后于 Soniox 和 Voxtral 等专门的实时语音识别服务。 此次发布加剧了语音转文本市场的竞争，为开发者提供了一个来自谷歌的高准确率选项，同时也凸显了低延迟对实时转录应用的重要性。社区的快速基准测试表明，仅靠准确率可能不足以赢得开发者的青睐。 测试过该模型的社区成员指出，虽然 Gemini-3.5-Transcribe 在准确率上胜过其他模型，但延迟方面仍需改进。该模型还支持函数调用，可将图像生成等任务委托给其他 Gemini 模型，部分用户担心无意中的文本简化可能改变原意。

hackernews · k9294 · 8月27日 18:03 · [社区讨论](https://news.ycombinator.com/item?id=49468818)

**背景**: 语音转文本（STT）模型将口语转换为书面文字，实时 STT 需要同时具备高准确率和低延迟，才能用于实时翻译、听写和字幕生成。相关竞品包括 Soniox（一个实时语音 AI 平台）和 Voxtral（Mistral AI 开发的开源多模态音频对话模型）。Google 的 Gemini-3.5-Transcribe 属于 Gemini 模型家族，该家族专为包括音频理解在内的多模态任务而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://soniox.com/">Soniox | Multilingual Speech AI platform: Realtime STT, TTS ...</a></li>
<li><a href="https://arxiv.org/abs/2507.13264">[2507.13264] Voxtral - arXiv.org Voxtral TTS: Free Open-Source AI Voice Generator mistralai/Voxtral-Small-24B-2507 · Hugging Face Voxtral Realtime WebGPU - a Hugging Face Space by mistralai Voxtral TTS - docs.mistral.ai</a></li>

</ul>
</details>

**社区讨论**: 测试过该模型的开发者称赞其准确率，但认为延迟才是决定性因素，一位开发者表示 Soniox STT v5 仍然是实时翻译的最佳选择。还有用户提到 Voxtral Mini 3b 是令人满意的本地模型，部分用户指出该模型会过度简化精确措辞，且其函数调用功能的文档令人困惑。

**标签**: `#speech-to-text`, `#Google`, `#AI models`, `#transcription`, `#machine learning`

---

<a id="item-5"></a>
## [Microduck：Pollen Robotics 推出的开源双足机器人平台](https://pollen-robotics.com/microduck/) ⭐️ 8.0/10

Pollen Robotics 在 GitHub 上发布了名为 Microduck 的开源双足机器人平台。这个 25 厘米高的机器人拥有 15 个电机、摄像头、深度传感器、两个 IMU 和可活动的喙，并利用强化学习策略进行移动。 Microduck 降低了在真实硬件上进行强化学习实验的门槛，让爱好者和学术界更容易接触人形风格机器人研究。由于 Pollen Robotics 现已成为 Hugging Face 的一部分，该项目也凸显了 AI/ML 生态与实体机器人之间日益紧密的交集。 由于公司位于法国，仿真器默认使用 AZERTY 键盘布局（ZQSD 键），这让一些用户感到意外。机器人的强化学习策略先在 MuJoCo（由 Google DeepMind 维护的物理引擎）中训练，然后再部署到实体机器人上。

hackernews · robotswantdata · 8月27日 10:57 · [社区讨论](https://news.ycombinator.com/item?id=49462763)

**背景**: Pollen Robotics 是一家创立于 2016 年的法国机器人公司，现已成为 Hugging Face 的一部分，以开发富有表现力的开源交互式机器人而闻名。Microduck 是一款小型双足机器人，使用强化学习（RL）——一种让智能体在模拟环境中通过反复试错来改进行为的方法。MuJoCo（Multi-Joint dynamics with Contact）是一款广泛用于模拟机器人和训练强化学习策略的物理引擎。该项目旨在让研究人员和创客能够复现并扩展机器人的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pollen-robotics.com/microduck/blog/introducing-microduck/">Meet Microduck | Pollen Robotics</a></li>
<li><a href="https://github.com/pollen-robotics/microduck">GitHub - pollen- robotics / microduck : A Tiny biped duck robot</a></li>
<li><a href="https://pollen-robotics.com/">Pollen Robotics - Robots for AI builders</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者热情响应，帖子获得 586 分和 199 条评论。批评主要集中在对仿真器 AZERTY 键盘布局、完整硬件零件清单是否真正开放的质疑，以及 F1TENTH/RoboRacer、Legolas、Tinker 等其他开源机器人替代品的推荐。还有几位评论者强调了 MuJoCo 在机器人学习中的核心作用，为讨论提供了有价值的技术背景。

**标签**: `#robotics`, `#open-source`, `#simulation`, `#hardware`, `#AI`

---

<a id="item-6"></a>
## [法官裁定特朗普政府将 Anthropic 列入黑名单违法](https://www.nytimes.com/2026/08/27/technology/anthropic-government-blacklisting-ruling.html) ⭐️ 8.0/10

2026 年 8 月 27 日，一名联邦法官裁定，特朗普政府将 AI 公司 Anthropic 列入黑名单的行为非法。这一裁决是对行政权力的一种法律约束，限制了政府将 AI 企业列入黑名单的做法。 该裁决加强了 AI 公司在面对政府审查时的法律保护，并可能为行政权力针对科技企业的行动如何被司法审查开创先例。它还可能通过明确国家安全理由必须符合法律标准，来影响未来的 AI 监管。 该裁决并不一定消除潜在的国家安全担忧，政府也可能会提出上诉。根据法院的补救措施，Anthropic 可能有权恢复相关资格、获得损害赔偿或其他与黑名单有关的救济。

hackernews · jbegley · 8月28日 02:03 · [社区讨论](https://news.ycombinator.com/item?id=49473522)

**背景**: 黑名单是政府的一种做法，通常会以国家安全为由，禁止企业参与特定合同、获得许可证或进行其他官方往来。Anthropic 是一家重要的人工智能公司，在前一届政府执政期间被列入此类名单，由此引发了法律挑战并最终促成这项裁决。

**社区讨论**: 评论者普遍对这一裁决的实际影响持怀疑态度，质疑违不违法对现任政府来说是否重要，以及法律是否过于缓慢、难以应对快速变化的科技问题。还有人讽刺地认为，这件事反而推动了主权 AI 和自托管的发展，并怀疑大型参与者不会因此承担任何负面后果。

**标签**: `#AI policy`, `#law`, `#Anthropic`, `#regulation`, `#government`

---

<a id="item-7"></a>
## [84 天完成 N64 游戏《Snowboard Kids》反编译](https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/) ⭐️ 8.0/10

一位开发者记录了在 84 天内完整反编译任天堂 64 游戏《Snowboard Kids》的过程，详细介绍了逆向工程流程和所用工具。该文章还展示了包括 LLM 在内的现代工具如何加速了这一工作。 这之所以重要，是因为完整的反编译能够支持社区驱动的游戏保护、模组制作和移植，为被忽视的经典游戏注入新生命。它还展示了一套可复现的工作流程，可能激励复古游戏生态中的类似项目。 该项目据称将原始游戏代码以高级语言进行了 1:1 重建，这是现代反编译工作的标志。文章还讨论了 LLM 辅助编码的使用，以及将受版权保护的可执行代码转换为开源表示所涉及的法律细节。

hackernews · knackers · 8月27日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49466006)

**背景**: 游戏反编译是一种逆向工程过程，通过检查编译后的游戏二进制文件，用 C 等高级语言重建其原始源代码。对于 N64 游戏，这使社区能够制作 PC 移植版、改进画面并修复漏洞。最近，LLM 被用来自动化和加速这一过程的某些部分。反编译项目的法律地位仍有争议，历史上相关概念如“净室”（clean room）重实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://readonlymemo.com/decompilation-projects-and-n64-recompiled-list/">Decompilation projects and N64 Recompiled PC ports (August 2026)</a></li>
<li><a href="https://arxiv.org/abs/2402.18659">[2402.18659] Large Language Models and Games: A Survey and ...</a></li>
<li><a href="https://tetracorp.github.io/tokimeki-memorial/methods/what-is-decompilation.html">Exploring Tokimeki Memorial: What is decompilation ?</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一成果表示赞赏，并提到了类似项目如《The Legend of Dragoon》的重编译版。其他人则讨论反编译的法律地位，并对游戏公司为何不借此赚钱表示惊讶。还有人指出，LLM 辅助的工作流程能让开发者效率倍增，但受限于时间和 token。部分评论推荐了其他怀旧向游戏。

**标签**: `#decompilation`, `#reverse engineering`, `#Nintendo 64`, `#game preservation`, `#LLMs`

---

<a id="item-8"></a>
## [谷歌发布 Gemini Omni 1.1 Flash，支持 40 秒场景扩展与 4K 视频生成](https://blog.google/innovation-and-ai/technology/developers-tools/build-with-gemini-omni-1-1-flash/) ⭐️ 8.0/10

谷歌发布了 Gemini Omni 1.1 Flash，这是其多模态视频生成模型的更新版本，新增了 40 秒场景扩展、起始/结束关键帧控制、360p 草稿预览以及 1080p 或 4K 输出能力。该模型已通过 Gemini API 和 Google AI Studio 向开发者开放。 此次发布巩固了谷歌在 AI 视频生成领域的地位，谷歌在该领域持续加大投入，而 OpenAI 等竞争对手已从类似方向收缩。新的创意控制让模型更适用于生产环境，可能加速其在影视、广告和内容创作中的应用，也引发了对创意行业从业者影响的讨论。 场景扩展功能可分析现有视频的最多 10 秒内容，并以 10 秒为增量将其延长至累计 40 秒，相比早期版本提升了视觉一致性。该模型还支持指定镜头的首尾关键帧、生成 360p 草稿以便快速迭代，以及输出 1080p 或 4K 全分辨率视频。

hackernews · saretup · 8月27日 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49467922)

**背景**: Gemini Omni Flash 是谷歌推出的高性能多模态模型，专为视频生成与编辑设计，可通过 Gemini API 和 Google AI Studio 使用。场景扩展功能允许模型基于已有片段继续生成以延长镜头，关键帧控制则让创作者指定镜头的起始和结束画面。此次 1.1 更新扩展了这些能力，支持更长的扩展、草稿预览和更高分辨率的输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/omni">Generate and edit videos with Gemini Omni Flash | Gemini API | Google AI for Developers</a></li>
<li><a href="https://the-decoder.com/googles-gemini-omni-1-1-flash-makes-ai-video-generation-cheaper-and-more-flexible/">Google's Gemini Omni 1.1 Flash makes AI video generation cheaper and more flexible</a></li>

</ul>
</details>

**社区讨论**: 评论者提到该技术可能对配音演员和演员行业产生影响，并就谷歌持续投入视频生成而 OpenAI 放弃 Sora 的策略展开讨论，也不乏对 Gemini Pro 迟迟未更新的调侃。一位开发者表示失望，因为该模型无法将生成的视频与已有音频同步用于对口型，并称自己改用本地运行的 Minimax H3 来完成这类任务。

**标签**: `#AI`, `#Google`, `#video-generation`, `#Gemini`, `#developer-tools`

---

<a id="item-9"></a>
## [提示注入攻击以 80%成功率突破 Claude Code 自动模式](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

安全研究员 Johann Rehberger 演示了一种针对 Claude Code 自动模式的提示注入攻击，成功率约 80%。该攻击诱使智能体下载并解压 zip 压缩包，然后执行代码，通过 base64 内部对 struct 的依赖，在不知不觉中导入并运行恶意的本地 struct.py 文件。 这很重要，因为 Anthropic 最近将 Claude Code 的自动模式设为 Pro、Max 和 Team 方案的默认选项，依赖其分类器来保护用户免受提示注入攻击。一位可信的研究人员证明该安全机制可以被绕过，甚至还会阻止 Claude 自己的清理命令，这引发了对自主 AI 编码智能体安全性的严重担忧。 该攻击利用了 Python 模块遮蔽（module shadowing）：从 zip 压缩包中解压出的 struct.py 文件在 base64 导入 struct 时优先于标准库模块生效。在数次运行中，自动模式虽然察觉到了入侵，却阻止了智能体终止恶意进程的命令，表明分类器本身可能成为故障的一部分。

rss · Simon Willison · 8月27日 22:50

**背景**: 提示注入是一种攻击方式，攻击者将精心构造的文本隐藏在 LLM 读取的内容中，使模型执行本不应遵循的指令。Claude Code 的自动模式是一种权限模式，通过分类器批准或阻止工具调用，目的是让智能体无需日常提示即可自主运行。Python 模块遮蔽是指本地文件与标准库模块同名，由于 Python 优先搜索当前目录，导致导入的是本地版本而非已安装的标准库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://claude.com/blog/auto-mode">Auto mode for Claude Code | Claude by Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#AI security`, `#Claude Code`, `#LLM agents`, `#cybersecurity`

---

<a id="item-10"></a>
## [新基准 HarnessOpt-Bench 测试 AI 改进其他 AI 的能力](https://www.reddit.com/r/MachineLearning/comments/1w052xg/can_ai_improve_itself_rsi_might_be_the_answer_r/) ⭐️ 8.0/10

该论文提出了 HarnessOpt-Bench，一个通过评估 LLM 在多大程度上改进另一个智能体的 harness（代理外壳）来打分的基准，并通过沙箱隔离从构造上防止作弊。它报告了 5 个前沿模型、4 个下游任务和 111 次运行的实验结果。 这是对递归自我改进研究的一项新颖实证贡献，这一课题具有高影响力和安全意义。它提供了一种标准化方法，用于衡量 AI 系统能否真正改进其他 AI 系统，这关乎智能爆炸的相关争论。 隔离通过构造而非指令来保证：保留的评估器和权限控制位于进化循环之外。结果显示，Claude Opus 5 在 OpenCode 下在 4 个任务中 3 个表现最佳，而 opencode 在 20 个模型-任务对中的 11 个上击败了原生 harness（Claude Code、Codex、Kimi CLI）。

reddit · r/MachineLearning · /u/shehio · 8月27日 20:13

**背景**: Agent harness（代理外壳）是 LLM 周围的软件基础设施，使其能够作为 AI 智能体运行，管理工具调用、记忆和反馈循环。递归自我改进是一个假设的过程，即 AI 系统重写自己的代码，可能引致智能爆炸。HarnessOpt-Bench 在昂贵且随机的评估条件下测试端到端的 harness 优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.06301">[2608.06301] HarnessOpt-Bench: Evaluating LLMs at Harness ...</a></li>
<li><a href="https://labs.scale.com/papers/harnessopt-bench">HarnessOpt-Bench: Evaluating LLMs at Harness Optimization</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#recursive self-improvement`, `#LLM agents`, `#benchmark`, `#machine learning`

---

<a id="item-11"></a>
## [英伟达 Q4 营收 681 亿美元超预期，下季度指引上调至 780 亿美元](https://t.me/zaihuapd/43450) ⭐️ 8.0/10

英伟达公布第四财季营收 681 亿美元，其中数据中心业务贡献 623 亿美元，两项数据均高于市场预期。公司预计 2027 财年第一季度销售额为 780 亿美元，超过华尔街预测的 726 亿美元，盘后股价上涨逾 3%。 这份超预期财报和上调的指引确认 AI 基础设施需求依然异常强劲，这一信号波及整个 AI 与半导体供应链。同时表明，尽管市场担忧 OpenAI 的融资能力和行业竞争，大型云厂商和企业仍在积极部署 GPU。 数据中心业务占 681 亿美元总营收中的 623 亿美元，而游戏和汽车业务营收未达预期。CEO 黄仁勋提到计算需求呈现指数级增长，并表示公司已采取战略性措施保障库存以应对供应链压力。

telegram · zaihuapd · 8月27日 08:51

**背景**: 英伟达是 AI 训练和推理所用 GPU 的主导供应商，其季度业绩是观察 AI 基础设施投资的重要风向标。该公司负责芯片设计但将制造外包，因此供应链约束和库存管理对满足云服务商和企业激增的需求至关重要。

**标签**: `#NVIDIA`, `#earnings`, `#AI infrastructure`, `#data center`, `#GPUs`

---

<a id="item-12"></a>
## [OpenAI 被曝开发常驻 Codex 代理，持续工作直至休眠](https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/) ⭐️ 8.0/10

据 WIRED 审查的代码，OpenAI 正为命令行版 Codex 添加「常驻模式」，使代理能够持续工作直到被「休眠」，不同于现有模式在几分钟或几小时后即停止的做法。OpenAI 确认正在测试该功能，但暂无近期上线计划。 这标志着向长期运行的自主编码代理迈出了重要一步，可能通过让开发者委托更广泛、跨会话的任务来改变软件工程工作流程。这也表明主要 AI 实验室正在将代理式 AI 从一次性交互推向持续的、目标驱动型运作。 常驻模式内置「主动性」设定：完成请求后会自动创建后续任务，并可跨会话执行，依据对用户的了解来决定工作内容。改动用户系统之外的东西仍需事先批准，目前尚无确定的发布日期。

telegram · zaihuapd · 8月28日 02:47

**背景**: Codex 是 OpenAI 开发的 AI 编程代理，用于编写代码、修复错误等软件工程任务，于 2025 年 4 月以 Codex CLI 形式发布，并可通过 ChatGPT 网页、桌面应用和多种 IDE 集成使用。AI 代理是能够追求目标、使用工具并自主执行多步骤任务的人工智能程序，通常由大语言模型驱动。常驻模式扩展了此类代理常见的「会话受限」模式，使其能运行更长时间并自主管理任务队列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#AI agents`, `#autonomous coding`, `#software engineering`

---

<a id="item-13"></a>
## [美国国防部将 Anthropic 列入黑名单 防务公司弃用 Claude](https://t.me/zaihuapd/43460) ⭐️ 8.0/10

美国国防部正式将 Anthropic 列为“供应链风险”，这是美国本土科技公司首次获得该标签。随后，多家国防科技公司要求员工停止使用 Anthropic 的 Claude 模型，改用其他 AI 工具。 这是一次重大政策转向，可能限制 Anthropic 参与国防相关合同的资格，并为美国 AI 监管开创先例。这也表明美国政府正加大对 AI 企业与国家安全供应链关系的审查，可能重塑 Claude 在国防领域的采用格局。 据报道，Anthropic 是首家被五角大楼列入供应链风险清单的美国本土企业。另据 3 月 10 日报道，Anthropic 已就该认定对国防部等联邦机构提起诉讼。该决定出自特朗普政府，并由 CNBC 率先报道。

telegram · zaihuapd · 8月28日 03:15

**背景**: Anthropic 是一家成立于 2021 年的人工智能初创公司，由前 OpenAI 研究人员达里奥·阿莫迪和丹妮拉·阿莫迪兄妹创立，致力于构建安全、可解释、可操控的 AI 系统。其 Claude 模型采用“宪法式 AI”原则进行训练，目标是让助手做到有用、无害且诚实。在美国国防规则中，“供应链风险”认定通常意味着该公司的产品因国家安全原因被禁止进入国防供应链。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Anthropic">Anthropic - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.winzheng.com/article/pentagon-labels-anthropic-supply-chain-risk">官方确认：五角大楼将Anthropic列为 供 应 链 风 险 ，美 国 首家 | 赢政天下</a></li>
<li><a href="https://www.tmtpost.com/nictation/7906725.html">Anthropic就“ 供 应 链 风 险 ”认定起诉美 国 国 防 部</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#AI regulation`, `#national security`, `#defense technology`, `#supply chain risk`

---