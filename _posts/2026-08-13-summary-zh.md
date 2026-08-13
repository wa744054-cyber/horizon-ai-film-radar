---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 32 条内容中筛选出 10 条重要资讯。

---

1. [DRAM 意面化：新攻击打乱内存映射，解锁 CPU 隐藏区域](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 发布，开放 1.7T 参数权重](#item-2) ⭐️ 9.0/10
3. [DeepMind 手语转文字模型 SL2T 首次登陆 Pixel 11](#item-3) ⭐️ 9.0/10
4. [DeepSeek 开源 Harness，并发布 V4-Pro-0813 权重](#item-4) ⭐️ 9.0/10
5. [谷歌发布 Gemini 3.7 Flash，视觉转 HTML 能力突出](#item-5) ⭐️ 8.0/10
6. [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度提升 7 倍](#item-6) ⭐️ 8.0/10
7. [选择无聊技术：明智花费创新代币](#item-7) ⭐️ 8.0/10
8. [DeepSeek 发布开源智能体 Harness 开发者预览版](#item-8) ⭐️ 8.0/10
9. [像素指标无法对机器人视频上的世界模型排序；开源工具诊断原因](#item-9) ⭐️ 8.0/10
10. [OpenAI 推出 GPT-5.6 系列，新增 Think 按钮并扩大免费权限](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DRAM 意面化：新攻击打乱内存映射，解锁 CPU 隐藏区域](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas 发布了硬件安全工具“skitter-creek-bath-salts”，通过改写 DRAM 控制器的物理地址映射来打乱内存。该技术已在 AMD Family 16h CPU 上演示，能够绕过高层防护，暴露平台安全处理器(PSP)、系统管理模式(SMM)和 CPU 微码等隐藏区域。 此事意义重大，因为 DRAM 地址解码长期以来被视为可信的抽象层；暴露它使内存控制器成为攻击面。如果该漏洞在当前 CPU 上可利用，就可能破坏内存隔离，并泄露通常由负环(negative ring)硬件保护的机密，从而重新定义我们对硬件安全的认知。 该攻击通过翻转内存控制器中的单个比特位，并利用线性代数重建专有的 DRAM 地址置乱(scrambling)机制。目前已在 2013 年的 AMD Jaguar(Family 16h)上演示；相关说明提到 Zen 3 的内存控制器基地址不同，因此新 CPU 上是否仍存在攻击面尚不明确。

hackernews · matt_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM 地址解码是将 CPU 物理地址映射为内存芯片内部行、列、Bank 等坐标的过程。现代内存控制器出于信号完整性和安全原因，会对此映射施加专有的置乱(scrambling)算法，且通常对操作系统和管理程序隐藏。攻击者通过操控控制器，可使地址落到预期的物理位置之外，从而触及通常位于“负环”区域的 SMM、PSP 或 CPU 微码等隐藏资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">Spaghettifying DRAM</a></li>
<li><a href="https://zeli.app/en/story/49286341">Spaghettifying DRAM: Unlock Everything on the CPU | Zeli</a></li>
<li><a href="https://upstract.com/x/201aa8130cc32a64">Spaghettifying DRAM - upstract.com</a></li>

</ul>
</details>

**社区讨论**: 评论者们热情高涨，盛赞 Christopher Domas 并期待他在 Black Hat 上的演讲。也有人对实用范围提出疑问：该攻击目前只在 2013 年的 AMD Jaguar 上演示，尚不清楚对 Zen 3 等现代 CPU 影响如何。还有评论指出，虽然 Xbox 或 PlayStation 等游戏机很难获得 ring-0 权限，但一旦获得，这种技术将使一切防护都形同虚设。

**标签**: `#security`, `#DRAM`, `#hardware`, `#exploitation`, `#reverse-engineering`

---

<a id="item-2"></a>
## [DeepSeek V4 Pro 0813 发布，开放 1.7T 参数权重](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 9.0/10

DeepSeek V4 Pro 0813 现已通过 OpenRouter API 提供，其开放权重（1.7T 参数，893 GB）也已发布在 Hugging Face 上。Simon Willison 指出目前还没有官方的发布公告页面。 这是一次重要的开放权重大型语言模型发布，延续了 DeepSeek 定期发布的风格。它通过 API 和可下载权重为开发者和研究者提供了 1.7T 参数的模型，对中国乃至全球 AI 社区都意义重大。 Hugging Face 上的发布文件大小为 893 GB，表明这是一个庞大的模型。Simon Willison 注意到不同推理级别（低、中、高）生成的图像输出差异很大，这与其他模型相比很不寻常。基准测试结果先发在 DeepSeek 官方微信群，随后在 Reddit 帖子被删除后，又被转载到 Hacker News。

rss · Simon Willison · 8月12日 23:59

**背景**: DeepSeek 是一家以发布强大的开放权重语言模型而闻名的中国 AI 公司，例如 DeepSeek V3 和 V4 系列。开放权重模型允许开发者下载并修改模型参数，从而实现本地部署和微调，这与仅提供 API 的闭源模型形成对比。OpenRouter 是一个统一的 API 网关，可以访问来自不同提供商的数百种模型，方便比较和使用各种 AI 模型。2026 年，DeepSeek 继续发布 V4 Pro 和 V4 Flash 等更新，并向公众开放这些权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/openrouter">OpenRouter API and Models | OpenRouter</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open - Weights Model? | AI 21</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#llm`, `#open-weights`, `#ai`, `#machine-learning`

---

<a id="item-3"></a>
## [DeepMind 手语转文字模型 SL2T 首次登陆 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 9.0/10

谷歌 DeepMind 发布了大规模多语言手语转文字模型 SL2T，并将其部署在 Pixel 11 的 Gboard 和 Live Transcribe 中。该模型目前支持美国手语（ASL）到英语的翻译。 这标志着手语 AI 首次集成到消费级智能手机中，为失聪及听障用户提供了相当于语音听写的功能。它为无障碍功能进入主流设备开创了先例，并有望扩展到更多语言和平台。 该模型使用超过 10 万小时、涵盖 50 多种手语的数据进行训练，在 FLEURS-ASL 基准上的零样本得分为 70 BLEURT。为保护隐私，它仅处理手部和身体姿态关键点，而不读取原始视频。

telegram · zaihuapd · 8月13日 08:55

**背景**: FLEURS-ASL 是一个基准数据集，将 FLORES/FLEURS 多语言平行语料库扩展到以视频形式呈现的美国手语。BLEURT 是一种用于自然语言生成的学习型评估指标，用于衡量候选文本与参考文本的匹配程度。由于缺乏大规模训练数据和基准，手语转文字 AI 一直落后于语音和文本翻译。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://arxiv.org/abs/2408.13585">[2408.13585] FLEURS-ASL: Including American Sign Language in Massively Multilingual Multitask Evaluation</a></li>
<li><a href="https://www.techtimes.com/articles/324242/20260813/sign-language-dictation-reaches-smartphones-last-via-googles-gloss-free-ai.htm">Sign Language Dictation Reaches Smartphones at Last, via ...</a></li>

</ul>
</details>

**标签**: `#DeepMind`, `#sign language AI`, `#accessibility`, `#Pixel`, `#NLP`

---

<a id="item-4"></a>
## [DeepSeek 开源 Harness，并发布 V4-Pro-0813 权重](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 9.0/10

DeepSeek 以 MIT 协议开源了 Harness 应用，并在 Hugging Face 上开放了 DeepSeek-V4-Pro-0813 模型权重。Harness 开发者预览版采用由 Cordis 驱动的“一切皆插件”架构，提供标准、PTC、极简和创造四种运行模式。 这对 AI/ML 社区意义重大，因为它降低了构建自定义 agent harness 的门槛，并让研究人员可以访问一个强大的新模型。插件架构允许开发者在不修改主代码库的情况下替换模型、工具和 UI 组件，有望加速 agent 工程工作流。 该项目以 npm 包（`@deepseek-ai/dsh`）的形式发布，源代码托管在 GitHub 上，会话、沙箱、存储、调度和 UI 等功能都可作为可替换插件实现。DeepSeek-V4-Pro-0813 的 Hugging Face 页面曾短暂返回 404，随后恢复，表明可能存在部署方面的小问题。

telegram · zaihuapd · 8月13日 12:39

**背景**: Agent harness 是编排 AI agent 与模型、工具和外部服务交互的运行时环境。DeepSeek Harness（dsh）基于 Cordis 构建，Cordis 是一个负责插件挂载、卸载和依赖解析的插件框架，其设计在《A Programming Paradigm for Spatiotemporal Composability》中有所描述。MIT 协议允许商业和个人使用且限制很少，因此这一发布引起了广泛关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">DeepSeek Harness - GitHub</a></li>
<li><a href="https://deepseek-harness.github.io/deepseek-harness/en/reference/cordis-primer">Cordis Primer | DeepSeek Harness</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#open-source`, `#AI`, `#Hugging Face`, `#model release`

---

<a id="item-5"></a>
## [谷歌发布 Gemini 3.7 Flash，视觉转 HTML 能力突出](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

谷歌发布了其最新的主力 AI 模型 Gemini 3.7 Flash，它在推理能力、可自定义思考级别以及视觉转 HTML 方面表现突出。根据 OpenRouter，输入价格每百万 token 仅需 0.375 美元，输出价格每百万 token 1.875 美元，但这一首发价格将在 2026 年 12 月 31 日翻倍。 此次发布加剧了 AI 模型市场的竞争，尤其是社区测试验证了 Gemini 在视觉转 HTML 方面的强大能力，且价格低于竞争对手。对于需要高性价比、大规模文本和视觉任务的开发者来说，Flash 系列模型的吸引力大增，这可能扰乱现有大语言模型的定价体系。 Gemini 3.7 Flash 拥有 1,048,576 token 的上下文窗口，最大输出 65,536 token，并支持低、中、高三种思考配置。模型卡强调其核心推理基础获得算法级改进；社区评论指出，该模型在 Gemini 3.6 Flash 发布仅三周后便推出，因此这个首发定价的时间安排显得颇为奇怪。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini Flash 系列模型定位为快速、低成本的「主力」模型，适合处理摘要、解析、agent 工作流等高容量任务。视觉转 HTML 是一项让模型将图片或截图转换为可用 HTML 代码的测试，常用于网页原型制作和无障碍化；Gemini 历来在此任务上表现出色。3.7 Flash 模型卡指出，它是 Gemini 3 系列的下一个迭代版本，在多步规划和工具调用准确性方面有所提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://openrouter.ai/google/gemini-3.7-flash">Gemini 3 . 7 Flash - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3 . 7 Flash - Model Card — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一，但讨论积极。测试者 jjcm 发现，Opus 5 在图像转 HTML 任务上仍是同类最佳，但 Gemini 3.7 在这个价位上的表现令人惊喜；simonw 则认为这个首发定价安排「很怪」，并指出 3.6 与 3.7 发布间隔太短。还有人将其与 GPT-5.6 Luna 对比，认为 Luna 更便宜且在 DeepSWE 1.1 上性能更好；另有评论者认为，从基准测试看，它更像是 Terra 的对手而非 Luna 的对手。

**标签**: `#Google Gemini`, `#AI model release`, `#LLM`, `#benchmarks`, `#pricing`

---

<a id="item-6"></a>
## [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度提升 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 发布了 GPT-5.6 Sol Ultrafast，这是一个由 Cerebras 硬件驱动的新服务层级，运行 GPT-5.6 Sol 的速度比标准处理快达 14 倍，在 HLE 等前沿基准上实现了约 7 倍的推理加速。该预览版首先在 OpenAI API 中推出。 这标志着 LLM 推理速度的重大进步，可能助力事件响应、客户服务、金融分析和电子商务等领域的实时 AI 应用。同时，它也凸显了软硬件协同设计日益重要，Cerebras 的晶圆级引擎正在挑战 NVIDIA 在 AI 加速领域的主导地位。 OpenAI 表示 Ultrafast 每秒最多可生成 750 个输出令牌，比标准处理快达 14 倍。该合作在 2500 道题的 HLE 基准上以 11 小时 11 分钟完成并获得相当精度，而 Claude Fable 5 需要 78 小时 27 分钟，但社区成员指出官方并未明确确认其输出质量与常规 GPT-5.6 Sol 完全一致。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras 制造晶圆级引擎（WSE），这是全球最大的 AI 处理器，例如 CS-3 拥有 90 万个 AI 优化核心和 44GB 片上 SRAM。Ultrafast 服务层级顺应了 AI 实验室（如 OpenAI 和 Anthropic）提供加速模型版本的潮流，OpenAI 将其定位为“每秒更有用的工作”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/08/13/openai-introduces-ultrafast-a-new-mode-that-makes-gpt-5-6-sol-work-at-14x-the-speed/">OpenAI introduces 'Ultrafast,' a new mode that makes GPT-5.6 Sol work at 14x the speed | TechCrunch</a></li>

</ul>
</details>

**社区讨论**: 社区总体反应积极但谨慎。一些用户称赞加速可能促进迭代式思考，而另一些人（如 Topfi）指出 Cerebras 和 OpenAI 都没有明确说明 Ultrafast 与标准 GPT-5.6 Sol 性能完全相同，暗示如果是一比一等同，他们“早就大声宣扬了”。还有评论者注意到没有定价信息，意味着可能很昂贵或仍在试探市场兴趣。

**标签**: `#AI`, `#LLM`, `#Inference`, `#Hardware`, `#OpenAI`

---

<a id="item-7"></a>
## [选择无聊技术：明智花费创新代币](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

Dan McKinley 在 2015 年发表的文章《选择无聊技术》主张，公司应优先采用成熟、易懂的“无聊”技术，以节省有限的“创新代币”，把它们用在真正需要新颖性的地方。这篇文章已成为关于技术选型与风险管理的经典、极具影响力的作品。 这篇文章为工程领导者提供了一个便于记忆的思维模型，用于做出并解释技术权衡，在创新与运维风险之间取得平衡。它在当下依然高度相关，尤其是在 AI 生成代码的时代，选择“无聊”技术能让 AI 输出的审查和验证更加容易。 McKinley 提出，每家公司大约拥有三枚“创新代币”，每采用一种新技术就花费一枚，而选择“无聊”的技术则无需花费。他建议把代币节省下来，用在真正能形成业务差异化的少数领域。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: McKinley 在 Etsy 工作期间形成了这一理念，该公司的工程团队以高产出著称，原因就在于他们偏向使用成熟、经过验证的技术。“创新代币”这一比喻此后被广泛采用和讨论，有人用它来指导技术决策，也有人批评它过于简单化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/technical-debt-innovation-tokens-case-boring-technology-jeffrey-henry-lhexe">Technical Debt, Innovation Tokens , and the Case for Boring...</a></li>
<li><a href="https://blog.glyph.im/2024/07/against-innovation-tokens.html">Deciphering Glyph :: Against Innovation Tokens</a></li>
<li><a href="https://mattrickard.com/innovation-tokens">Innovation Tokens | Matt Rickard</a></li>

</ul>
</details>

**社区讨论**: 评论者大多持肯定态度，NickNaraghi 称“创新代币”概念是他作为产品和工程领导者职业生涯中最有用的想法之一。不过也有人提出异议，例如 insanitybit 认为代币模型过于随意，“新”只是权衡的弱代理。还有人如 theptip 指出，在智能体时代，团队或许应该把全部代币花在智能体上以获得杠杆效应。

**标签**: `#technology-strategy`, `#engineering-culture`, `#software-architecture`, `#innovation`, `#decision-making`

---

<a id="item-8"></a>
## [DeepSeek 发布开源智能体 Harness 开发者预览版](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek Harness 的 MIT 许可开发者预览版，这是一个开源智能体 harness，具备可追踪的会话日志和热重载插件功能。 这家主要 AI 实验室的发布直接回应了 AI 智能体工具链对可观测性和灵活性日益增长的需求。可追踪的会话日志和动态插件系统有望让智能体开发在整个生态系统中更加透明和易于维护。 该 harness 使用仅追加的会话日志，记录模型看到的所有内容，包括系统提示、推理过程、工具调用及结果，可在 Trajectory 视图中查看。插件系统基于 Cordis v4，支持热重载，并在卸载时完整清理状态和副作用。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**背景**: Agent harness 是围绕 LLM 的软件基础设施，使其能够作为智能体运行：它管理工具使用、记忆、状态持久化、执行环境和反馈循环。由于 LLM 是无状态的且仅生成文本，harness 是让模型能够执行多步操作、使用外部工具并维持长期任务的关键。本次发布的 DeepSeek Harness 主要面向构建此类智能体系统的开发者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://harness-engineering.ai/blog/agent-harness-complete-guide/">The Complete Guide to Agent Harness: What It Is and Why It ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，评论者称赞仅追加的会话日志是“杀手级功能”，并指出与美国某些模型不同，其追踪数据不会被加密或混淆。DeepSeek Harness 的作者确认这是早期开发者预览版，可能存在瑕疵，并欢迎大家提供反馈。还有一些评论讨论了 Cordis v4 基础，并将其与字节跳动的 Eino 等现有库进行比较。

**标签**: `#DeepSeek`, `#AI agents`, `#developer tools`, `#open source`, `#LLM`

---

<a id="item-9"></a>
## [像素指标无法对机器人视频上的世界模型排序；开源工具诊断原因](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

作者发布了开源诊断工具 worldproof，用于将世界模型的 rollout 与真实结果及物理不变量进行比较。在真实机器人视频上，作者用一个简单的“复制最后一帧”基线进行验证，结果显示该基线获得了接近完美的 SSIM（0.983）和 PSNR（53.9 dB）分数，并且误差随预测步长保持平稳，证明在这些场景下像素指标无法对模型进行排序。 这一发现挑战了在真实机器人数据上使用 SSIM 和 PSNR 评估视频预测与世界模型的常见做法。它表明，当帧率相对于任务速度过高时，评估设置会失去区分能力，这可能推动社区转向更有意义的评估窗口和诊断指标。 在真实的 SO-101 机械臂录像上，使用 30fps、64 条 rollout、6 步预测窗口，并且只在动态区域评分时，基线达到了 0.983 SSIM 和 53.9 dB PSNR，且误差不随步数增长。在 DROID 视频上扩展到 48 步时，SSIM 仅在大约第 4 到第 24 步之间单调下降，随后在 0.20 附近触底震荡，说明可用的评估窗口约为 8 到 24 步；LPIPS 未能区分两个数据集，且在掩码版本中指向相反方向。

reddit · r/MachineLearning · /u/georgia_bucea · 8月13日 19:58

**背景**: 世界模型是一类机器学习系统，它学习环境的内部表征，并预测环境如何随动作变化，通常用于支持智能体的规划与推理。SSIM 和 PSNR 是经典的图像相似度指标，但人们已知它们与感知质量的相关性较差，并且在场景接近静态时可能对有意义的变化不敏感。在高帧率机器人视频中，预测接下来几帧可能几乎与复制最后一帧一样容易，因此任何“预测画面不变”的模型都能获得接近满分的成绩，导致更复杂的模型无法被区分排序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Structural_similarity_index_measure">Structural similarity index measure - Wikipedia</a></li>
<li><a href="https://uk.mathworks.com/help/images/ref/psnr.html">psnr - Peak signal - to - noise ratio ( PSNR ) - MATLAB</a></li>

</ul>
</details>

**标签**: `#world models`, `#evaluation metrics`, `#robotics`, `#open-source`, `#machine learning`

---

<a id="item-10"></a>
## [OpenAI 推出 GPT-5.6 系列，新增 Think 按钮并扩大免费权限](https://t.me/zaihuapd/43176) ⭐️ 8.0/10

OpenAI 宣布推出 GPT-5.6 系列模型，Plus 和 Pro 订阅用户可使用 GPT-5.6 Sol，其事实回答更可靠，并新增滑块控制思考深度。免费用户本周起默认升级至 GPT-5.6 Luna，下周起可无限文本对话，并新增 Think 按钮以应对复杂推理问题。 此次更新将高级推理功能带给更广泛的用户，尤其是免费用户，也表明 OpenAI 在模型能力与成本效率之间寻求平衡。免费用户获得无限文本对话可能显著提升 ChatGPT 的用户活跃度，并加剧 AI 助手之间的竞争。 据报道，GPT-5.6 系列包含三个层级：Sol（旗舰版，面向付费用户）、Terra（均衡版）和 Luna（快速廉价版，面向免费用户）。内部评估显示，在财经、医疗和法律等问题上，Luna 的事实错误较此前模型有所减少；新增的 Think 按钮可显式触发深度推理。

telegram · zaihuapd · 8月13日 17:04

**背景**: OpenAI 会定期更新 ChatGPT 的底层模型，GPT-5.6 系列似乎是类似此前模型家族的多层级发布，在智能、速度和成本之间进行不同取舍。Think 按钮此前已出现在 o1 等推理模型上，供用户显式要求模型在回答前进行逐步推理。据报道，Luna 层级的按 token 定价较低，适合高用量或免费场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/gpt-5-6-luna">GPT - 5 . 6 Luna : OpenAI ' s fastest, cheapest model tier... | eesel AI</a></li>
<li><a href="https://qcode.cc/en/gpt-5-6-guide">GPT - 5 . 6 Sol , Terra & Luna — Benchmarks, Pricing... | QCode.cc</a></li>
<li><a href="https://appleinsider.com/articles/26/08/06/new-chatgpt-version-has-a-think-button-will-find-more-reliable-facts">New ChatGPT version has a 'Think' button, will find 'more reliable facts'</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#ChatGPT`, `#AI model release`, `#Free access`

---