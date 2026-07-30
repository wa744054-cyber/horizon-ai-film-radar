---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> 从 42 条内容中筛选出 15 条重要资讯。

---

1. [开源引擎：在任意 M 系列 Mac 上用 2GB 内存运行 Gemma 4 26B](#item-1) ⭐️ 9.0/10
2. [AI 蠕虫通过提示注入在 Word 中传播](#item-2) ⭐️ 9.0/10
3. [AI 发现 NIST 后量子候选算法 HAWK 严重弱点](#item-3) ⭐️ 9.0/10
4. [AI 初创企业愈发不愿公开研究成果](#item-4) ⭐️ 8.0/10
5. [Mitchell Hashimoto 基于开源 libghostty 创立 Superlogical](#item-5) ⭐️ 8.0/10
6. [生产力幻象：专注于工作本身](#item-6) ⭐️ 8.0/10
7. [AI 公司为数据中心招聘数千电工木匠](#item-7) ⭐️ 8.0/10
8. [Kimi K3-256k 推出突发上下文定价模式](#item-8) ⭐️ 8.0/10
9. [格林：后量子密码转型正适合 AI 密码分析](#item-9) ⭐️ 8.0/10
10. [AI 安全排行榜：评测模型对越狱攻击的鲁棒性](#item-10) ⭐️ 8.0/10
11. [使用 ncnn Vulkan 实现跨厂商边缘设备 GPU 推理](#item-11) ⭐️ 8.0/10
12. [月之暗面寻求 20 亿美元融资，估值 300 亿](#item-12) ⭐️ 8.0/10
13. [反网络暴力法征求意见稿出台，AI 网暴纳入监管](#item-13) ⭐️ 8.0/10
14. [OpenAI 向十万学者免费提供前沿模型](#item-14) ⭐️ 8.0/10
15. [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [开源引擎：在任意 M 系列 Mac 上用 2GB 内存运行 Gemma 4 26B](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare 是一个用 Swift 和 Metal 编写的开源推理引擎，通过从 SSD 流式传输专家权重，在任意 M 系列 Mac 上仅用约 2 GB 内存即可运行 4 位量化的 Gemma 4 26B-A4B-IT 模型。 这一突破使得在内存有限的消费级硬件上运行大型混合专家模型成为可能，推动了设备端 AI 的普及，减少了对昂贵高内存机器的需求。 该引擎在 8 GB 的 M2 MacBook Air 上达到 5–6 tok/s，在 M5 MacBook Pro 上达到 31–35 tok/s，通过小容量专家缓存和有界并行 pread 系统调用来隐藏 SSD 延迟。

hackernews · gitpusher42 · 7月29日 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: Gemma 4 26B 是一个混合专家（MoE）语言模型，每个 token 仅激活一部分参数（专家）。传统推理需要将所有 14 GB 的 4 位量化权重加载到内存中，超出常见消费级 Mac 的内存容量。TurboFieldfare 将共享核心和 KV 缓存保留在内存中，仅从 SSD 流式传输被路由到的专家，利用 MoE 的稀疏性大幅降低内存使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://wpnews.pro/news/a-26b-model-in-2-gb-of-ram-courtesy-of-your-ssd">A 26B Model in 2 GB of RAM, Courtesy of Your SSD — Web Pulse</a></li>

</ul>
</details>

**社区讨论**: 社区对该项目创新的内存高效方法表示赞赏，用户分享了在不同 M 系列 Mac 上的性能数据。评论提到在 M4 Max 上获得了 48 tok/s 的良好速度，并讨论了与 llama.cpp 的 mmap 方法的比较。macOS 15 的兼容性问题已解决，还有人建议与其他项目如 DiffusionGemma 集成。

**标签**: `#LLM inference`, `#on-device AI`, `#Mac`, `#open-source`, `#memory efficiency`

---

<a id="item-2"></a>
## [AI 蠕虫通过提示注入在 Word 中传播](https://simonwillison.net/2026/Jul/29/ai-worming-through-word/#atom-everything) ⭐️ 9.0/10

研究员 Håkon Måløy 发现了一种提示注入变种，将隐藏指令嵌入 Word 文档中，导致 Microsoft Copilot 操纵文档并复制指令，形成自复制 AI 蠕虫。 这是首次展示针对广泛使用的企业软件通过 AI 助手的自复制蠕虫，对依赖 Copilot 的组织构成重大安全风险。 该攻击利用隐藏的白底白字文本指令，Copilot 将其视为用户请求，且指令设计为传播到 Copilot 生成的新文档中。

rss · Simon Willison · 7月29日 18:43

**背景**: 提示注入是一种安全漏洞，恶意输入导致 LLM 产生非预期行为。早期攻击需要诱骗用户，而这种变种在 AI 生态系统中实现自动传播，类似计算机蠕虫。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://thehackernews.com/2026/06/researchers-build-self-replicating-ai.html">Researchers Build Self-Replicating AI Worm That Operates Entirely on Local, Open-Weight Models</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#AI security`, `#Microsoft Word`, `#self-replicating worm`, `#Copilot`

---

<a id="item-3"></a>
## [AI 发现 NIST 后量子候选算法 HAWK 严重弱点](https://startupfortune.com/claude-mythos-broke-hawk-and-the-nist-post-quantum-timeline-may-not-survive-it/) ⭐️ 9.0/10

Anthropic 的 Claude Mythos Preview AI 在约 60 小时内发现了 NIST 后量子数字签名候选算法 HAWK-256 的严重漏洞，将其有效密钥强度从 2^64 降至 2^38，花费约 10 万美元 API 费用。该漏洞此前两年未被人类专家发现。 这一事件表明，AI 现在在发现密码算法弱点方面已超越人类密码分析员，可能加速后量子标准化进程，并促使各方更早采用密码敏捷性。同时，它也引发了对其他 NIST 候选算法安全性的质疑。 该攻击并非多项式时间，因此更大的 HAWK 参数仍然安全；HAWK 尚未被公开撤回。Anthropic 还报告了对 7 轮 AES-128 的改进攻击，但完整的 AES-128（10 轮）不受影响。该研究使用了 Claude Mythos Preview 模型，该模型仅对特定合作伙伴开放。

telegram · zaihuapd · 7月30日 05:47

**背景**: 后量子密码学旨在开发能抵抗量子计算机的算法，量子计算机可能破解当前加密。NIST 一直在运行竞赛以选择后量子标准；HAWK 是第三轮中的候选数字签名方案。密码敏捷性是指在不造成重大中断的情况下切换算法，这对于迁移到后量子系统至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://korben.info/en/claude-breaks-post-quantum-algorithm-60-hours.html">Claude breaks a post - quantum algorithm in 60 hours - Korben</a></li>
<li><a href="https://www.borsaya.com/en/news/ai-weakens-post-quantum-algorithm-candidate-hawk-in-60-hours">AI Weakens Post - Quantum Algorithm Candidate HAWK in 60 Hours</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cryptographic_agility">Cryptographic agility</a></li>

</ul>
</details>

**标签**: `#AI`, `#cryptography`, `#post-quantum`, `#NIST`, `#security`

---

<a id="item-4"></a>
## [AI 初创企业愈发不愿公开研究成果](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

近期分析显示，顶尖人工智能初创企业的研究论文发表量正在减少，引发了对该领域透明性和可重复性的担忧。 这一趋势威胁到推动人工智能进步的开放科学文化，可能减缓创新速度，并使更广泛的社区难以在初创企业的发现基础上进一步发展。 该论文列出 OpenAI、MEGVII、Hugging Face、Waymo 和 Anthropic 等公司的引用量位居前列，但其论文发表数量并非最高，统计的是引用次数而非发表数量。

hackernews · YeGoblynQueenne · 7月29日 21:25 · [社区讨论](https://news.ycombinator.com/item?id=49103285)

**背景**: 历史上，人工智能研究通常通过会议和期刊公开发表，以促进同行评审和重复验证。然而，随着 AI 应用商业价值提升，初创企业有动机保持方法专有，以维持竞争优势。

**社区讨论**: 评论者指出了相互矛盾的动机：一些初创企业通过发表研究来获得信誉和合作机会，而另一些则隐瞒成果以避免被 OpenAI 和 Anthropic 等竞争对手抄袭。还有人担忧 AI 研究的“博客化”导致低质量论断泛滥。

**标签**: `#AI research`, `#open science`, `#startups`, `#reproducibility`

---

<a id="item-5"></a>
## [Mitchell Hashimoto 基于开源 libghostty 创立 Superlogical](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto 宣布成立新公司 Superlogical，将在开源库 libghostty 之上构建商业产品，此前他已将 Ghostty 终端模拟器的所有权转让给一个非营利组织。 此举展示了一种可持续的开源商业模式：核心基础设施由社区拥有，公司在此基础上构建增值服务。鉴于 Hashimoto 在 Vagrant 和 Terraform 上的成就，Superlogical 可能影响终端和基于 Agent 的工具的开发方式。 Superlogical 将使用与其他所有人相同的 MIT 许可的 libghostty 组件，并继续向上游贡献共享终端工作。该公司旨在创建一个能够自主管理终端会话的代理型多路复用器。

hackernews · yan · 7月29日 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Mitchell Hashimoto 是广受欢迎的 DevOps 工具 Vagrant 和 Terraform 的创建者。Ghostty 是他构建的一个快速、GPU 加速的终端模拟器；libghostty 是从 Ghostty 中提取的 C 库，允许在任何应用程序中嵌入终端模拟功能。将 Ghostty 转让给非营利组织确保了其独立性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍称赞这种开源方式，有人指出在公共依赖上建立公司是明智之举。一些人将其与 OLE/COM 的组件嵌入进行类比，也有少数人批评含糊的标题是点击诱饵。

**标签**: `#Mitchell Hashimoto`, `#Ghostty`, `#terminal`, `#open source`, `#startup`

---

<a id="item-6"></a>
## [生产力幻象：专注于工作本身](https://frantic.im/mirage/) ⭐️ 8.0/10

一篇批评文章认为，过度痴迷于生产力工具适得其反；真正的生产力来自于专注于实际工作，而不是无休止地优化工具。 这挑战了软件工程师和知识工作者中常见的观念，鼓励从以工具为中心转向以工作为中心的生产力，可能导致更有效的结果。 作者强调，思考和阅读比打字速度更重要；许多工程师花更多时间调整他们的设置，而不是做有意义的工作。

hackernews · msephton · 7月29日 23:18 · [社区讨论](https://news.ycombinator.com/item?id=49104335)

**背景**: 生产力工具包括文本编辑器、任务管理器和自动化脚本。“生产力色情”现象指的是不断优化工具而不是做工作的习惯。这篇文章批评了这种行为，建议简约主义并专注于问题领域。

**社区讨论**: 评论者普遍同意这一批评。一些人指出工具很重要，但应该为工作服务，而不是成为干扰。另一些人注意到减少屏幕时间和显示器数量可以提高生产力。

**标签**: `#productivity`, `#tooling`, `#software engineering`, `#work habits`, `#minimalism`

---

<a id="item-7"></a>
## [AI 公司为数据中心招聘数千电工木匠](https://www.nytimes.com/2026/07/29/business/economy/data-center-electricians-training.html) ⭐️ 8.0/10

人工智能公司正在为数据中心建设招聘数千名电工和木匠，反映出其业务模式向基础设施方向的转变。 这一趋势凸显了人工智能基础设施大规模建设对劳动力的巨大需求，影响着建筑行业，并可能重塑技术劳动力市场。 招聘热潮源于建设和维护实体数据中心的需求，而非 AI 软件开发本身。评论者警告说，数据中心建设具有周期性，易经历繁荣与萧条。

hackernews · thm · 7月29日 14:43 · [社区讨论](https://news.ycombinator.com/item?id=49098198)

**背景**: 人工智能的快速发展导致数据中心建设激增，主要科技公司纷纷扩展云端和 AI 基础设施。这些设施需要大量熟练技工，如电工和木匠，进行安装和维护。这与早期主要招聘软件工程师的科技繁荣形成对比。

**社区讨论**: 社区评论表达了不同观点：一些人高兴看到技工获得高薪工作，而另一些人则警告繁荣-萧条周期，并指出这些“AI 公司”本质上是基础设施公司。

**标签**: `#AI infrastructure`, `#data centers`, `#labor market`, `#trades`, `#technology industry`

---

<a id="item-8"></a>
## [Kimi K3-256k 推出突发上下文定价模式](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Kimi K3-256k 推出了新的定价层级，提供 256k 上下文窗口，并可无缝切换到 1M 上下文模型，从而在 API 使用中实现了“突发上下文”模式。 这种定价模式可以显著降低典型用户的成本，同时允许偶尔处理大上下文任务，可能改变开发者管理 LLM 上下文使用的方式，并降低使用 1M 上下文模型的门槛。 256k 层级在切换到 1M 时不会使 KV 缓存失效，从而实现平滑扩展；但底层 Kimi K3 模型需要 1.5TB 显存才能进行完整推理，不过量化可将内存降低至约 570GB，精度为 75%。

hackernews · monneyboi · 7月29日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49101852)

**背景**: 大型语言模型（LLM）处理上下文窗口——即它们一次能考虑的文字量。更长的上下文窗口需要更多内存和计算资源。“突发上下文”借鉴了云计算中的概念，即资源可以临时超过基线限制。Kimi K3 是 Moonshot AI 推出的 2.8 万亿参数模型，支持高达 100 万 token 的上下文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/code/docs/en/kimi-code/models">Model Configuration | Kimi Code Docs</a></li>
<li><a href="https://kie.ai/blog/what-is-kimi-k3">What Is Kimi K3? Moonshot's 2.8T, 1M-Context Flagship</a></li>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了定价和突发上下文的想法，认为这与 OpenAI 的分层定价相似。一些人对模型因需要巨大显存而并非真正开源感到失望，不过 1 比特量化等压缩方法可将内存降至 570GB。

**标签**: `#LLM`, `#context window`, `#pricing`, `#Kimi`, `#AI`

---

<a id="item-9"></a>
## [格林：后量子密码转型正适合 AI 密码分析](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

著名密码学家 Matthew Green 指出，当前从传统公钥算法向后量子算法的历史性转型，正是借助 AI 密码分析来增强对新标准信心的绝佳时机。 这一评论具有时效性，因为后量子密码的采用对于保护数据免受未来量子计算机攻击至关重要，而 AI 密码分析有助于验证 HAWK 等新算法的安全性。 格林特别提到了 HAWK 签名方案（目前处于 NIST 后量子签名评估的第三轮），并提及 Impagliazzo 的 Minicrypt 世界（一种 AI 可能无法攻破所有问题的场景）。

rss · Simon Willison · 7月29日 18:18

**背景**: 后量子密码学旨在开发能抵抗量子计算机的加密算法。HAWK 是一种基于格的签名方案，正在被 NIST 评估。Impagliazzo 的五种世界是根据计算复杂性假设对可能密码世界进行的分类。向后量子标准的转型是保护数字基础设施的历史性努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://decrypt.co/374600/claude-mythos-cracked-post-quantum-cryptography">Claude Mythos Cracked Post - Quantum Cryptography That... - Decrypt</a></li>
<li><a href="https://thehackernews.com/2026/07/claude-ai-just-cracked-post-quantum.html?m=1">Claude AI Just Cracked a Post - Quantum Test Scheme and Found...</a></li>
<li><a href="https://blog.computationalcomplexity.org/2004/06/impagliazzos-five-worlds.html">Computational Complexity: Impagliazzo 's Five Worlds</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#post-quantum`, `#AI`, `#cryptanalysis`

---

<a id="item-10"></a>
## [AI 安全排行榜：评测模型对越狱攻击的鲁棒性](https://www.reddit.com/r/MachineLearning/comments/1vaargb/ai_security_leaderboard_benchmarking_model/) ⭐️ 8.0/10

一个新的排行榜通过 1500 个自动生成的越狱攻击测试，评估前沿 AI 模型对自动越狱攻击的鲁棒性。 该基准测试填补了 AI 安全领域的关键空白，随着对抗性威胁的增加，模型安全性对部署决策变得越来越重要。 测试套件衡量通用越狱的成功率——提示词引发模型对某个领域内超过 75%的明显有害问题给出顺从且详细的响应——覆盖领域包括 CBRNE 和进攻性网络安全。

reddit · r/MachineLearning · /u/ARGleave · 7月29日 22:09

**背景**: AI 越狱攻击是利用 AI 系统漏洞绕过伦理准则并执行受限操作的攻击方式，通常通过提示注入或角色扮演场景实现。对抗鲁棒性指的是模型抵抗这类有意对抗的能力。该排行榜旨在提供一个系统化的基准来比较模型安全性，尽管已有众多能力排行榜，但安全性基准一直缺失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/insights/ai-jailbreak">AI Jailbreak | IBM</a></li>
<li><a href="https://adversarial-ml-tutorial.org/introduction/">Chapter 1 - Introduction to adversarial robustness</a></li>

</ul>
</details>

**标签**: `#AI security`, `#adversarial robustness`, `#benchmarking`, `#jailbreak`, `#model security`

---

<a id="item-11"></a>
## [使用 ncnn Vulkan 实现跨厂商边缘设备 GPU 推理](https://www.reddit.com/r/MachineLearning/comments/1v9s4mz/vendoragnostic_ml_inference_on_production_edge/) ⭐️ 8.0/10

视频编辑工具 PostSlate 现在使用 ncnn 的 Vulkan 后端在设备上运行机器学习推理，在无需特定厂商运行时的情况下，面部检测和嵌入实现了高达 10 倍的加速。 这种方法消除了厂商锁定并简化了部署，使得在从 NVIDIA 到 Apple Silicon 的任何消费级边缘设备上实现高性能机器学习推理成为可能。 在 RTX 4070 上，ArcFace R50 面部嵌入从 30 毫秒（ONNX CPU）降至 3 毫秒（ncnn Vulkan），SCRFD 面部检测从 25 毫秒降至 2.5 毫秒，通过 fp16 权重存储模型大小减半。

reddit · r/MachineLearning · /u/ppchaos · 7月29日 10:22

**背景**: ncnn 是一个为移动和边缘设备优化的开源神经网络推理框架。Vulkan 是一个跨平台 GPU API，支持底层硬件访问，允许无需额外运行时即可在不同厂商的 GPU 上运行机器学习推理。将二者结合为跨厂商边缘人工智能提供了统一解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/topics/ncnn?o=asc&s=stars">ncnn · GitHub Topics · GitHub</a></li>
<li><a href="https://codelabs.viam.com/guide/ncnn-edge-ai/">Optimize using AI models at the edge with ncnn runtime</a></li>
<li><a href="https://www.insightface.ai/research/scrfd">InsightFace SCRFD Paper Explained: Efficient Face Detection</a></li>

</ul>
</details>

**标签**: `#ML inference`, `#Vulkan`, `#edge devices`, `#cross-platform`, `#GPU acceleration`

---

<a id="item-12"></a>
## [月之暗面寻求 20 亿美元融资，估值 300 亿](https://t.me/zaihuapd/42845) ⭐️ 8.0/10

月之暗面（Moonshot AI）正寻求至多 20 亿美元的新融资，目标估值 300 亿美元，这已是其六个月内启动的第三轮融资。公司 4 月年度经常性收入突破 2 亿美元，并正在拆除境外架构筹备香港上市。 如此快速的估值飙升（从 40 亿到 300 亿美元）反映了对 AI 聊天机器人和大模型的爆炸性需求，使月之暗面成为中国 AI 领域的重要参与者。计划中的香港上市表明亚洲投资者对 AI 初创公司的兴趣日益增长。 此前由美团领投的一轮融资对月之暗面的投后估值为 200 亿美元，而去年 12 月仅为 40 亿美元。该公司还推出了 Kimi Work，这是一款用于深度工作流程的桌面 AI 代理，可挂载本地文件夹并自主运行 Python 代码。

telegram · zaihuapd · 7月29日 10:12

**背景**: 月之暗面是热门中文聊天机器人 Kimi 的开发商，其背后是自研的大语言模型。随着企业和消费者采用其 AI 工具，公司实现了爆炸性增长。2026 年推出的 Kimi Work 是一款面向知识工作者的本地代理，能够运行数百个并行代理并自动化浏览器任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/products/kimi-work">Kimi Work: Next-Gen Desktop AI Agent for Knowledge Workers</a></li>
<li><a href="https://www.kimi.com/resources/kimi-work-introduction">Kimi Work: The Local AI Agent for Your Desktop</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#Chinese tech`, `#startup`, `#valuation`

---

<a id="item-13"></a>
## [反网络暴力法征求意见稿出台，AI 网暴纳入监管](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

2026 年 7 月 29 日，国家互联网信息办公室公布反网络暴力法征求意见稿，专门规制利用 AI 技术制作和传播网络暴力信息的行为。 该法律是 AI 治理的重要里程碑，直接应对日益严重的 AI 生成辱骂内容问题，明确了平台的法律责任，并为受害者提供了更强有力的保护。 草案共七章六十条，涵盖名誉权、隐私权、肖像权和个人信息等权益侵害。要求网络服务提供者建立监测识别和防护机制，并引入人格权侵害禁令和精神损害赔偿。

telegram · zaihuapd · 7月29日 10:59

**背景**: 网络暴力在中国已成为严重的社会问题，AI 工具使得大规模生成辱骂内容变得更加容易。现有法律在应对 AI 生成伤害方面存在空白，因此该草案是及时的监管回应。

**标签**: `#cyber violence`, `#AI regulation`, `#draft law`, `#online safety`

---

<a id="item-14"></a>
## [OpenAI 向十万学者免费提供前沿模型](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 8.0/10

2026 年 7 月 29 日，OpenAI 宣布推出 ChatGPT for Academic Researchers 项目，计划在 2027 年前向 10 万名研究人员免费提供 GPT-5.6 等前沿模型，今夏首批开放 1 万人。 该计划大幅降低了学术研究人员在基因组学、蛋白质建模等领域使用先进 AI 的门槛，有望加速科学发现，并促进学术界与产业界的新合作。 参与者可使用 GPT-5.6 系列模型（Sol、Terra、Luna），并可邀请最多 4 位合作者，工作区默认不将数据用于模型训练。OpenAI 承诺到 2027 年投入超 2.5 亿美元支持外部研究。

telegram · zaihuapd · 7月30日 00:17

**背景**: GPT-5.6 于 2026 年 7 月 9 日发布，是 OpenAI 最新的前沿模型，提供三个版本：Sol（旗舰版）、Terra（均衡版）和 Luna（最快、最便宜版）。前沿模型是推动能力边界的先进 AI 系统，该项目旨在为学术研究人员提供这些模型以支持科研工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/api/">API Platform | OpenAI</a></li>
<li><a href="https://www.vellum.ai/blog/gpt-5-6-benchmarks-explained">GPT - 5 . 6 Sol vs Terra vs Luna: Which Tier Should You Actually Use?</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI for Science`, `#Research`, `#GPT-5`

---

<a id="item-15"></a>
## [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](https://t.me/zaihuapd/42859) ⭐️ 8.0/10

7 月 29 日，俄罗斯联邦安全局（FSB）依据《刑法》第 205.1 条指控 Telegram 创始人帕维尔·杜罗夫协助恐怖活动，并将其列入国际通缉名单。 这标志着国家对科技创始人采取的重大升级行动，可能为平台创作者因用户内容承担刑事责任开创先例。同时也引发了对加密、言论自由以及国家法律全球影响力的严重关切。 FSB 声称 Telegram 拒绝删除被乌克兰情报机构和恐怖组织用于协调破坏活动、恐怖袭击和诈骗的频道与机器人，导致平民伤亡和数十亿卢布损失。该指控最高可判处终身监禁。

telegram · zaihuapd · 7月30日 03:45

**背景**: 俄罗斯《刑法》第 205.1 条将协助恐怖活动定为犯罪，刑罚从 15 年到终身监禁。Telegram 是一款在俄罗斯和乌克兰广泛使用的加密通讯应用；其创始人帕维尔·杜罗夫一直公开批评俄罗斯政府的监控政策，并已移居海外多年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zerohedge.com/geopolitical/russia-charges-telegram-founder-durov-facilitating-terrorism">Russia Charges Telegram Founder Pavel Durov With... | ZeroHedge</a></li>
<li><a href="https://news.bitcoin.com/featured/telegrams-pavel-durov-lands-on-russias-wanted-list-as-terror-charges-ignite-new-showdown/">Telegram's Pavel Durov Lands on Russia 's Wanted List as Terror ...</a></li>
<li><a href="https://www.republicworld.com/tech/russia-escalates-terrorism-case-against-telegram-founder-pavel-durov-2026-07-29-133660">Russia Escalates Terrorism Case Against Telegram... | Republic World</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#Pavel Durov`, `#Russia`, `#legal`, `#terrorism`

---