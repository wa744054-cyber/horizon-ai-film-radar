---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 33 条内容中筛选出 11 条重要资讯。

---

1. [GLM-5.3：前沿编程与涌现的网络安全能力](#item-1) ⭐️ 9.0/10
2. [将 Doom 渲染器编译为 210 亿参数 Transformer，无需训练](#item-2) ⭐️ 9.0/10
3. [苹果联手阿里为中国自研 AI 模型，或成首个获批外企](#item-3) ⭐️ 9.0/10
4. [Qwen 3.8 27B：紧凑模型本地跑赢更大对手](#item-4) ⭐️ 8.0/10
5. [讽刺页『Every Fucking Website』嘲弄现代网页 UX 槽点](#item-5) ⭐️ 8.0/10
6. [torch-preflight：检测 PyTorch 训练错误与显存占用的静态检查器](#item-6) ⭐️ 8.0/10
7. [Vivodyne 的 AI 人体组织实验室有望终结动物测试](#item-7) ⭐️ 8.0/10
8. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-8) ⭐️ 8.0/10
9. [美国法官责令谷歌一周内取消第三方应用商店安装障碍](#item-9) ⭐️ 8.0/10
10. [苹果官宣换帅：库克卸任 CEO，特努斯 2026 年接任](#item-10) ⭐️ 8.0/10
11. [PostgreSQL 修复高危 to_char 缓冲区溢出漏洞，可执行任意代码](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GLM-5.3：前沿编程与涌现的网络安全能力](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.AI 发布了 GLM-5.3，这是一个基于 743B 参数基座模型的旗舰编程模型，官方称其在 Z.ai Code Bench 上比 GLM-5.2 提升 50%，并在 Terminal-Bench 3.0 和 Agents' Last Exam (CLI) 上达到开源 SOTA 结果。该发布还突出了涌现的网络安全能力，社区用户报告该模型可自主执行红队场景，包括发现 WordPress 插件的 0-day 漏洞和适配 6.8 内核漏洞利用。 这一发布意义重大，因为它标志着前沿大语言模型正在从代码生成走向自主的进攻性安全操作，模型可以独立发现并利用漏洞。如果得到验证，这种能力可能重塑网络安全工作流程，降低漏洞发现的门槛，同时也带来关于 AI 双重用途的新风险。 该模型支持 1M token 的上下文窗口，根据社区报告，原本为 GLM-5.2 设置的订阅已可切换到新版本。Z.AI 还在 cvd.z.ai 维护了一个协调漏洞披露（CVD）门户，安全研究者称模型已在扫描流行开源软件并提交了大量严重/高危 CVE，其中许多仍处于保密期。一些用户指出 GLM-5.3 "本质上仍只是 GLM 5.2 加后训练魔法"，并在某些漏洞利用链基准上仍落后于 Sol 和 Fable 等专有模型。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**背景**: 大语言模型中的涌现能力是指那些在小模型中不存在、只有足够大的模型才具备的能力，有时这种能力难以预测。GLM-5.3 似乎在网络安全领域展现了这种涌现：尽管它主要针对编程和长周期智能体任务进行训练，社区测试显示它能执行端到端的红队操作，例如发现 0-day 漏洞、实现远程代码执行以及适配内核漏洞利用。自主红队本身是一个快速发展的领域，AI 智能体持续探测系统漏洞，而 Z.AI 报告的 CVD 门户表明该模型正在被用于大规模主动发现并披露漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing & Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://arxiv.org/abs/2206.07682">[2206.07682] Emergent Abilities of Large Language Models</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈但态度不一。一位用户报告说 GLM-5.3 执行了完整的红队场景，包括 WordPress 插件中的 0-day 和 6.8 内核漏洞利用，并随即升级了订阅；其他人指出 Z.AI 似乎在规模化扫描开源软件并提交大量 CVE。怀疑者指出该模型在某些基准上仍落后于 Sol 和 Fable 等领先者，也有人称赞发布公告的文风——更像研究者所写，而不是典型的市场宣传说辞。

**标签**: `#AI`, `#LLM`, `#cybersecurity`, `#GLM-5.3`, `#frontier models`

---

<a id="item-2"></a>
## [将 Doom 渲染器编译为 210 亿参数 Transformer，无需训练](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 9.0/10

作者使用自研编译器 Torchwright，将《毁灭战士》的渲染算法直接编译为 210 亿参数的 Transformer 权重，整个过程中没有任何训练。向模型输入表示场景数据的 token 提示，即可生成包含像素绘制指令的 token 序列，进而还原出游戏 E1M1 关卡的画面，尽管在 B200 GPU 上大约每天只能渲染 35 帧。 这项工作表明，无需训练即可将复杂的真实世界算法直接编译为神经网络权重，为程序合成、模型可解释性和推理时计算开辟了新可能。它挑战了“Transformer 必须通过数据训练才能执行任务”的传统假设，并提出了一种将经典代码与神经架构相结合的新路线。 渲染一帧需要 3,614 个 token 的提示加上 53,747 个生成 token，在 B200 上耗时约 40 分钟；用于加载检查点并解析输出的宿主 Python 代码只有 43 行。权重以标准 Hugging Face 检查点格式发布，无需 trust_remote_code 即可加载，被编译的计算图源代码也已公开在 GitHub 上。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**背景**: Transformer 是一种通过注意力机制和全连接层处理 token 序列的神经网络，通常需要在大规模数据上训练才能学会执行任务。此前的 RASP、Tracr 和 ALTA 等框架已经证明，可以利用解析推导的参数将小型符号程序手动编译为 Transformer 权重。Torchwright 则将这一思想推广到通用计算图，可直接将计算图转换为 Transformer 权重；而本项目进一步将真实游戏引擎的渲染器——《毁灭战士》的算法——嵌入到模型中，证明了即使是复杂的过程式代码也能以 Transformer 参数的形式表达。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2410.18077">[2410.18077] ALTA: Compiler-Based Analysis of Transformers GitHub - Percepta-Core/transformer-vm: Compile programs ... ALTA: Compiler-Based Analysis of Transformers - OpenReview ALTA:Compiler-BasedAnalysisofTransformers - OpenReview ALTA: Compiler-Based Analysis of Transformers | ML Anthology ALTA: Compiler-Based Analysis of Transformers (arXiv:2410. ...</a></li>
<li><a href="https://ood.dev/posts/calculator/">A calculator, compiled into a transformer — Out of Distribution</a></li>
<li><a href="https://towardsdatascience.com/i-built-a-tiny-computer-inside-a-transformer/">I Built a Tiny Computer Inside a Transformer | Towards Data Science</a></li>

</ul>
</details>

**标签**: `#transformer`, `#compilation`, `#program synthesis`, `#AI research`, `#Doom`

---

<a id="item-3"></a>
## [苹果联手阿里为中国自研 AI 模型，或成首个获批外企](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 9.0/10

据知情人士透露，苹果已在阿里巴巴支持下专门为中国市场训练了一款大语言模型，改变了此前依赖第三方模型的策略。Apple Intelligence 预计将在未来数月随 iOS 更新在中国上线。 若成功落地，苹果将成为首个获北京批准在华提供自有 AI 模型的外国公司，从而更好地掌控中国市场的 AI 体验。这对 AI 行业和跨国科技公司在华战略都具有重要意义。 苹果自研模型并获得阿里巴巴支持，一改此前依赖第三方模型的策略。中国网信办已于上月备案其生成式 AI 服务。

telegram · zaihuapd · 8月14日 14:47

**背景**: Apple Intelligence 是苹果在 2024 年 WWDC 上发布的 AI 功能套件，结合端侧与服务器处理。在中国，根据《生成式人工智能服务管理暂行办法》，生成式 AI 服务须在网信办完成备案后方可向公众提供服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>
<li><a href="https://www.cac.gov.cn/2025-09/10/c_1759222982377536.htm">关于发布生成式人工智能服务已备案信息的公告（2025年7月至8月）_中央...</a></li>

</ul>
</details>

**标签**: `#苹果`, `#AI`, `#阿里巴巴`, `#中国市场`, `#大模型`

---

<a id="item-4"></a>
## [Qwen 3.8 27B：紧凑模型本地跑赢更大对手](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

阿里巴巴 Qwen 团队发布了 Qwen 3.8 27B，这是一个参数规模为 270 亿的稠密模型，在 DeepSWE 基准上取得 42.2 分，略高于 Claude Opus 4.7 Max 的 40 分。该模型经过量化后足够紧凑，可以在高端笔记本上本地运行。 这一发布表明，较小的开源模型可以在专业智能体编程基准上与前沿闭源模型一争高下。它可能加速本地、私有推理的趋势，并减少对昂贵 API 额度的依赖。 FP8 检查点已上架 Hugging Face，Unsloth 也发布了适用于 llama.cpp 的 GGUF 量化版本。DeepSWE 分数对比中 Claude Opus 4.7 Max 使用了 Claude Code，因此差异同时反映了工具链和模型本身能力；用户也提醒应谨慎解读基准结果。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: Qwen 是阿里巴巴的开源权重大语言模型系列，27B 属于中等规模的稠密配置，在能力与硬件需求之间取得平衡。DeepSWE 是一个智能体基准，测试模型自主解决真实软件工程问题的能力。本地推理需要借助量化（如 GGUF/IQ4）将模型压缩进消费级 GPU/CPU 内存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen / Qwen 3 . 8 - 27 B · Hugging Face</a></li>
<li><a href="https://ollama.com/library/qwen3.8">qwen 3 . 8</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-7">Introducing Claude Opus 4.7 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍印象深刻：simonw 称这是‘笔记本上跑过的模型画出的最好的鹈鹕’，scrlk 指出它在 DeepSWE 上击败了 Opus 4.7 Max。ramon156 等人认为跨厂商基准对比不如速度、成本和提示效率重要，KronisLV 则希望看到更多 MoE 变体，比如 35B A3B 模型。

**标签**: `#AI/ML`, `#open-source-models`, `#benchmarks`, `#Qwen`, `#local-inference`

---

<a id="item-5"></a>
## [讽刺页『Every Fucking Website』嘲弄现代网页 UX 槽点](https://lxe.github.io/everywebsite/) ⭐️ 8.0/10

讽刺网站『Every Fucking Website』夸张呈现弹窗、自动播放视频和付费墙等常见网页恼人设计。该站在 Hacker News 引发热议，获得 693 分和 389 条评论。 这一讽刺凸显了用户对欺骗性设计模式的普遍不满。Hacker News 上的讨论揭示了这些模式为何持续存在——例如弹窗能提升转化率——使其成为对 Web 开发者和 UX 设计师的有意义批评。 该网站托管在 GitHub Pages 上，加载速度快，仅使用来自 lxe.github.io 的 JavaScript。评论者指出缺少诸如随滚动跟随的自动播放视频和“在应用中更好”的提示等元素，而 everyfuckingwebsite.com 上的相关文章扩展了这种批评。

hackernews · doubletwoyou · 8月14日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=49299222)

**背景**: 暗黑模式（Dark patterns），又称欺骗性设计模式，是故意诱使用户进行非自愿操作（如不必要的购买或订阅）的界面。『Every Fucking Website』通过将这些模式堆叠到一个页面上来讽刺它们。该网站融入了关于 Web 设计同质化以及操纵性 UX 伦理影响的广泛讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lxe.github.io/everywebsite/">Every Fucking Website - GitHub Pages</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dark_pattern">Dark pattern</a></li>
<li><a href="https://deceptive.design/">Deceptive Patterns — spreading awareness since 2010</a></li>

</ul>
</details>

**社区讨论**: 评论者补充了缺失的恼人元素，如随滚动跟随的自动播放视频和“在应用中更好”的提示。一位用户分享称，在其 Shopify 商店添加“有人购买了 X”的弹窗显著提升了转化率，尽管这让他感到自我厌恶。还有人幽默地用 w3m 测试该网站，并指出它加载太快、使用的域名太少。

**标签**: `#web-design`, `#ux`, `#satire`, `#web-development`, `#popups`

---

<a id="item-6"></a>
## [torch-preflight：检测 PyTorch 训练错误与显存占用的静态检查器](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 8.0/10

torch-preflight 是一个新发布的开源检查工具，它通过静态分析 PyTorch 代码来发现常见训练错误，并估算 GPU 显存占用，且无需执行代码。它不需要 GPU，也不需要本地安装 torch，可以通过 pip 安装。 该工具能帮助机器学习从业者在启动训练前发现浪费 GPU 机时的昂贵错误，并在为云实例付费前估算显存占用。它填补了 PyTorch 工具链中的一个明显空白，可为研究人员和工程师节省大量时间与金钱。 目前 torch-preflight 实现了 13 条检测规则，包括通过 loss.append(loss) 保留 autograd 计算图、缺少 optimizer.zero_grad()、梯度累积未除以 loss，以及使用 DDP 但未配 DistributedSampler 等问题。作者表示，在单张 T4 上对四个模型的显存估算与实测峰值误差在 4% 以内，但该项目仍在开发中，可能存在误报。

reddit · r/MachineLearning · /u/LeJanbandhu · 8月14日 14:30

**背景**: Linter（代码检查器）是一种进行静态分析的工具，它在不编译或执行代码的情况下扫描源码，寻找可能表示缺陷的模式。PyTorch 的 autograd 引擎会在计算图中记录张量操作，以便在反向传播时计算梯度；如果 loss 被追加到列表中，每一步的计算图都会被保留，导致显存不断增长直至耗尽。在分布式训练中，DistributedDataParallel（DDP）通常需要搭配 DistributedSampler 使用，使每个进程获得不同的数据子集；否则每个 rank 会在相同的批次上重复训练。由于 torch-preflight 从不运行用户代码，因此可以在没有 GPU 或未安装 PyTorch 的环境中使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.pytorch.org/docs/2.13/autograd.html">Automatic differentiation package - torch. autograd — PyTorch 2.13...</a></li>
<li><a href="https://docs.pytorch.org/tutorials/intermediate/ddp_tutorial.html">Getting Started with Distributed Data Parallel - PyTorch</a></li>
<li><a href="https://github.com/pytorch/pytorch/blob/main/torch/utils/data/distributed.py">pytorch/torch/utils/data/distributed.py at main · pytorch ...</a></li>

</ul>
</details>

**标签**: `#PyTorch`, `#Linter`, `#ML Tooling`, `#GPU`, `#Static Analysis`

---

<a id="item-7"></a>
## [Vivodyne 的 AI 人体组织实验室有望终结动物测试](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 8.0/10

Vivodyne 推出了由 12 个机器人“蜂巢”实验室组成的网络，每年可对 300 多万个人体组织样本开展受控实验，并由 AI 设计实验以更好地预测药物的有效性和安全性。 约有 90% 的临床试验在通过动物测试后仍会失败，因为动物模型往往无法反映人体生物学。将 AI 指导的人体组织测试规模化，有望淘汰动物测试、降低药物研发成本，并减少后期试验失败。 每个 HIVE 都是完整的端到端机器人实验室，一次可测试 10,000 个人体组织，并在一到两周内生成数据，为强化学习循环提供燃料。据报道，Vivodyne 的年测试能力相当于美国全部临床试验总容量的两倍。

telegram · zaihuapd · 8月14日 01:48

**背景**: 药物研发传统上依赖动物测试来预测人体的反应，但动物模型并不能很好地代表人类的疾病和药物安全性。在实验室中培养的人体组织能提供更真实的数据，但以往难以大规模生产与测试。Vivodyne 将自动化实验室与 AI 结合，运行数百万次此类测试，并基于人类数据训练“医疗超级智能”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://www.businesswire.com/news/home/20260812148428/en/Vivodyne-Launches-the-Worlds-Largest-Human-Biological-Datacenter-to-Train-the-First-World-Model-of-Human-Biology">Vivodyne Launches the World’s Largest Human Biological Datacenter...</a></li>

</ul>
</details>

**标签**: `#AI`, `#drug discovery`, `#lab automation`, `#human tissue testing`, `#biomedical research`

---

<a id="item-8"></a>
## [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型。该模型总参数量达 280B，但每次仅激活 16B 参数，支持 512K 上下文，并可处理文本、图片、视频和音频。 此次发布意义重大，因为它为社区提供了一个参数量很大但推理成本极低的开源 MoE 模型，并具备多模态和长上下文能力。配套的 TEMPO 强化学习方法以及真实场景智能体基准，也可能推动长程智能体 AI 的研究。 据公告介绍，TEMPO 是一种新的强化学习方法，通过自批判和测试时价值估计来训练长程智能体。此次发布还包含 VibeSearchBench 和 VibeLifeBench 两个基准，模型权重已在 Hugging Face 上开放。

telegram · zaihuapd · 8月14日 08:27

**背景**: 混合专家（MoE）模型将参数划分为多个专家子网络，每个输入 token 仅激活其中的一小部分，因此超大模型也能以较少的激活参数高效运行。VibeSearchBench 和 VibeLifeBench 这两个基准旨在评估真实世界中的长程智能体任务：VibeSearchBench 包含 200 个双语任务，采用人格驱动的渐进披露和知识图谱评估；VibeLifeBench 则在模拟服务后端之上构建了跨日常领域、为期多周的任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/VibeBench/VibeSearchBench">GitHub - VibeBench/VibeSearchBench: The hardest search ...</a></li>
<li><a href="https://github.com/evolvent-ai/VibeLifeBench/tree/main">GitHub - evolvent-ai/VibeLifeBench: ️ The hardest life-admin ...</a></li>

</ul>
</details>

**标签**: `#MoE`, `#Open Source`, `#Multimodal`, `#LLM`, `#Reinforcement Learning`

---

<a id="item-9"></a>
## [美国法官责令谷歌一周内取消第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 8.0/10

美国地区法官 James Donato 下令谷歌简化竞争性安卓应用商店的安装流程，并要求在一周内删除 Play Store 中多余的警告步骤和摩擦。该命令源自 Epic 诉谷歌反垄断案，陪审团此前裁定谷歌在安卓应用分发领域构成非法垄断。 这项裁决直接削弱了谷歌对安卓应用分发的控制权，可能让第三方应用商店与 Play Store 的竞争变得容易得多。它还可能为法院如何对待平台设计中的“暗黑模式”和反竞争摩擦开创先例。 法院将这种多步骤流程（用户必须点击多屏，安装按钮被藏在警告之后）描述为蓄意制造的“反竞争摩擦”，用来吓退普通用户。谷歌必须让安装第三方应用商店像安装普通安卓应用一样直接。

telegram · zaihuapd · 8月14日 09:55

**背景**: 该命令是 Epic Games 诉谷歌反垄断案的一部分，Epic 起诉谷歌强制使用 Play Store 支付系统并限制竞争对手商店。安卓本来就允许侧载，但多年来谷歌不断增加警告屏幕，批评者认为这些警告旨在劝阻用户离开 Play Store。法官的裁决要求谷歌在一周内删除这些额外步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.justice.gov/atr/case/epic-games-inc-v-google-llc">Antitrust Division | Epic Games, Inc. v. Google LLC | United States Department of Justice</a></li>
<li><a href="https://byteiota.com/android-sideloading-gets-high-friction-warnings-in-2026/">Android Sideloading Gets “High-Friction” Warnings in 2026 | byteiota</a></li>

</ul>
</details>

**标签**: `#Google`, `#Antitrust`, `#Play Store`, `#Epic Games`, `#App Stores`

---

<a id="item-10"></a>
## [苹果官宣换帅：库克卸任 CEO，特努斯 2026 年接任](https://t.me/zaihuapd/43191) ⭐️ 8.0/10

苹果宣布管理层交接，现任 CEO 蒂姆·库克将卸任 CEO 并出任董事会执行董事长，硬件工程高级副总裁约翰·特努斯将从 2026 年 9 月 1 日起担任新任 CEO。董事会已一致批准这项安排，库克将在整个夏天继续担任 CEO，与特努斯完成过渡。 这是自 2011 年蒂姆·库克接替史蒂夫·乔布斯以来，苹果首次更换 CEO，对全球最具影响力的科技公司之一而言是历史性时刻。此次交接将影响苹果未来多年的产品战略和企业方向，整个科技行业和苹果生态系统都在密切关注。 约翰·特努斯于 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入高管团队，近年负责 iPhone、Mac、iPad、AirPods 等产品的研发。现任董事长阿瑟·莱文森将于 9 月 1 日转任首席独立董事，特努斯同日加入董事会。

telegram · zaihuapd · 8月14日 11:00

**背景**: 苹果是全球最具价值和影响力的科技公司之一，以 iPhone、Mac、iPad 等硬件产品及 App Store 等服务著称。蒂姆·库克担任 CEO 超过 15 年，带领苹果实现了营收和市值的巨大增长。特努斯是硬件工程领域的资深高管，这暗示苹果将继续重视硬件创新和产品整合。此次公告不仅关乎领导层更替，也体现出平稳、长期规划的过渡安排。

**标签**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#John Ternus`, `#tech industry`

---

<a id="item-11"></a>
## [PostgreSQL 修复高危 to_char 缓冲区溢出漏洞，可执行任意代码](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 披露并修复了 CVE-2026-14669，该漏洞是 to_char(timestamptz) 函数在处理超长 POSIX 时区缩写时出现的堆缓冲区溢出。该漏洞的 CVSS 评分为 8.8，允许已认证的低权限用户执行任意代码。 该漏洞之所以重要，是因为任何能设置时区的已认证数据库用户，都可能以 PostgreSQL 服务进程的操作系统权限执行任意代码，从而导致数据库服务器被完全攻陷。运行受影响版本的组织应及时应用小版本更新。 受影响版本包括 PostgreSQL 18.5、17.11、16.15、15.19 和 14.24 之前的版本。由于 18.5 因回归问题未正式发布，18 系列用户应直接升级至 18.6；该修复只需更新程序文件并重启服务，无需转储数据库或运行 pg_upgrade。

telegram · zaihuapd · 8月14日 14:35

**背景**: to_char 是 PostgreSQL 的格式化函数，可根据用户指定的格式模式将时间戳、间隔或数字转换为字符串。timestamptz 是带时区的时间戳数据类型，POSIX 时区字符串可包含用户自定义的缩写和 UTC 偏移量。该漏洞源于处理超长时区缩写时发生堆缓冲区溢出。PostgreSQL 是广泛使用的开源关系型数据库，安全修复通常随小版本发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.enterprisedb.com/docs/epas/latest/reference/sql_reference/03_functions_and_operators/07_data_type_formatting_functions/">EDB Postgres Advanced Server v18 - Data type formatting functions</a></li>
<li><a href="https://www.sqliz.com/postgresql-ref/to_char/">PostgreSQL to _ char () Function</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">List of tz database time zones - Wikipedia</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#Security`, `#CVE`, `#Vulnerability`, `#Database`

---