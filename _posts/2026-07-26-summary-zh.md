---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 31 条内容中筛选出 13 条重要资讯。

---

1. [Science 曝光中国基因编辑试验致儿童死亡被掩盖](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 支持 Inkling 模型、提升 DeepSeek-V4 性能、灵活注意力后端](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude 5 上下文工程新规则](#item-3) ⭐️ 8.0/10
4. [JetZero 的混合翼飞机承诺提高 50%燃油效率](#item-4) ⭐️ 8.0/10
5. [在 8 美元微控制器上运行 2890 万参数大语言模型](#item-5) ⭐️ 8.0/10
6. [通用汽车投资钠离子电池用于美国电网储能](#item-6) ⭐️ 8.0/10
7. [Fly.io 转向 AI 沙盒，因 Sprite 漏洞更换 CEO](#item-7) ⭐️ 8.0/10
8. [Ruff v0.16.0 将默认规则从 59 条增加到 413 条](#item-8) ⭐️ 8.0/10
9. [从头在 ARM64 汇编中实现 YOLO26n 推理](#item-9) ⭐️ 8.0/10
10. [LLM 在 IMO 2026 上测试：框架提升小型模型表现](#item-10) ⭐️ 8.0/10
11. [微软将用 TPM 芯片封堵盗版 Windows 激活](#item-11) ⭐️ 8.0/10
12. [DeepSeek 因内部言论外泄暂停新一轮融资](#item-12) ⭐️ 8.0/10
13. [近 200 家硅谷公司敦促特朗普不要禁止中国开放权重 AI](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Science 曝光中国基因编辑试验致儿童死亡被掩盖](https://t.me/zaihuapd/42777) ⭐️ 10.0/10

《科学》杂志于 2026 年 7 月 23 日发布独家调查，披露一名 6 岁女童 2025 年 3 月在上海新华医院接受实验性碱基编辑基因治疗后死亡，该事件从未被公开。 该事件严重违反科研伦理和监管规定，可能削弱公众对基因疗法的信任，并凸显不受监管的临床试验的危险性。 该女童患有一种罕见的单碱基突变遗传病，通过脊髓液注射数万亿 AAV 病毒载体靶向脑部神经元；7 天后因严重免疫反应死亡。其父母自费逾 80 万美元，ClinicalTrials.gov 记录已逾一年未更新。

telegram · zaihuapd · 7月26日 06:01

**背景**: 碱基编辑是一种无需产生双链断裂即可精确改变单个 DNA 碱基的基因组编辑技术。AAV（腺相关病毒）载体常用于递送治疗基因，但高剂量可能引发免疫反应。鞘内注射将药物直接注入脑脊液以绕过血脑屏障。中国的临床试验受法规约束，但该案例据报绕过了适当的监管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Base_editing">Base editing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adeno-associated_virus">Adeno-associated virus - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intrathecal_injection">Intrathecal injection</a></li>

</ul>
</details>

**标签**: `#gene editing`, `#bioethics`, `#clinical trial`, `#regulation`, `#science misconduct`

---

<a id="item-2"></a>
## [vLLM v0.26.0 支持 Inkling 模型、提升 DeepSeek-V4 性能、灵活注意力后端](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 新增了对 Inkling 模型系列的支持，包括基础建模、分段 CUDA 图以及推测解码，并通过专门的路由内核和融合操作显著提升了 DeepSeek-V4 的性能。该版本还添加了 fp32 lm_head 选择、按 KV 缓存组灵活选择注意力后端，并完善了 KV 卸载基础设施。 此版本显著扩展了 vLLM 的模型支持和性能优化能力，使其成为最新大型语言模型更通用且高效的推理引擎。Inkling 系列（采用 Mamba-hybrid 和 MoE 架构）以及 DeepSeek-V4 的改进将使在生产环境中部署高级 LLM 的广大用户受益。 Inkling 模型系列获得了完整的支持堆栈，包括分段 CUDA 图支持、Hopper FA4 相对注意力、MTP=1 推测解码、LoRA 和 NVFP4 量化。DeepSeek-V4 获得了专门的路由内核（E2E TPOT 提升 2.94%）、fused_topk_bias 内核（1.5-2 倍加速），以及在 Nvidia、AMD 和 Intel XPU 上的稀疏解码/预填充优化。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个用于高吞吐量 LLM 推理的开源库，以其 PagedAttention 和高效内存管理而闻名。它支持多种模型架构，包括密集变压器和混合专家（MoE）。Thinking Machines Lab 开发的 Inkling 模型是一个 Mamba-hybrid、256 专家 MoE 模型，具有多模态能力。推测解码技术如多令牌预测（MTP）使用草稿模型每次前向传递预测多个令牌，从而降低延迟。内核融合将多个 GPU 操作合并为一个，以减少内存流量并提高性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/vllm-project_inkling-our-open-weights-model-activity-7483227870585311232-81uL">Thinking Machines Lab Releases TML Inkling 1T-Parameter Model</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/inkling/nvidia/moe/">moe - vLLM</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**标签**: `#LLM`, `#inference`, `#vllm`, `#open-source`, `#performance`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude 5 上下文工程新规则](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic 发布了针对 Claude 5 模型的新上下文工程指南，重点优化指令和记忆管理。社区反馈指出了数据保留限制和 AutoMemory 功能可靠性的担忧。 这些指南代表了 Anthropic 为高级模型标准化有效提示的努力，但社区批评暴露了可能削弱信任的潜在缺陷。关于数据保留和自动记忆可靠性的争论对 AI 智能体开发有实际影响。 据报道，Claude Code 工具默认在 30-45 天后删除上下文历史记录，用户认为这存在问题。社区成员还指出 AutoMemory 会做出不可靠的上下文跳跃，尤其是在推理轨迹隐藏时。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 上下文工程是指为大型语言模型设计和优化指令及相关上下文以有效执行任务的过程。它包括管理短期和长期记忆，其中 AutoMemory 等技术旨在帮助 AI 智能体回忆相关信息。Anthropic 的 Claude 5 是新一代具备高级能力的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://weaviate.io/blog/context-engineering">Context Engineering - LLM Memory and Retrieval for AI Agents | Weaviate</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示了混合反应：有人建议设计显式语言以实现精确控制，而其他人则批评对 AutoMemory 的依赖不可靠。一位用户报告称 Claude Code 在 30-45 天后删除上下文历史记录，他们认为这不可接受；另一位警告说 AutoMemory 会做出大的上下文跳跃，可能导致意外决策。

**标签**: `#Claude 5`, `#context engineering`, `#AI prompting`, `#Anthropic`, `#LLM best practices`

---

<a id="item-4"></a>
## [JetZero 的混合翼飞机承诺提高 50%燃油效率](https://www.jetzero.aero/) ⭐️ 8.0/10

JetZero 成立于 2020 年，正在开发全球首款商用全翼飞机 Z4，其燃油效率比传统客机提高多达 50%。 这一突破可大幅降低航空业的碳足迹，为 2050 年实现净零排放提供可行路径，同时可能降低航空公司的运营成本。 混合翼设计面临结构增压、紧急疏散以及与现有机场登机口兼容性等挑战。JetZero 的 Z4 计划通过创新方案解决这些问题，例如用大型客舱屏幕取代窗户。

hackernews · lisper · 7月26日 02:55 · [社区讨论](https://news.ycombinator.com/item?id=49054224)

**背景**: 传统商用飞机采用管状机身加机翼设计，气动效率较低。混合翼身（BWB）飞机将机身与机翼融合为一个升力体，减少阻力并提高燃油效率。这一概念可追溯到 20 世纪 20 年代末的德国，但尚未在客运航空领域实现商业化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/future/article/20251107-blended-wings-the-sci-fi-look-that-may-shape-tomorrows-airliners">Blended wings : The sci-fi aircraft concept that could appear at an...</a></li>
<li><a href="https://natilus.co/">Sustainable Aircraft for a Greener Future</a></li>
<li><a href="https://www.aol.com/jetzero-groundbreaking-blended-wing-demonstrator-095758049.html">JetZero: Groundbreaking ‘ blended - wing ’ demonstrator plane... - AOL</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区的讨论突出了几个问题：一位评论者指出，改变飞行路线以避免形成凝结尾迹可将尾迹变暖效应减半，但这一做法尚未广泛采用。另一位建议采用模块化客舱以加快登机速度。还有一位指出增压、疏散和登机口兼容性方面的挑战。总体来看，社区对此技术持谨慎乐观态度，但对实际实施表示怀疑。

**标签**: `#aviation`, `#sustainability`, `#aircraft-design`, `#climate-tech`, `#startups`

---

<a id="item-5"></a>
## [在 8 美元微控制器上运行 2890 万参数大语言模型](https://github.com/slvDev/esp32-ai) ⭐️ 8.0/10

一个项目展示了如何在售价 8 美元的 ESP32 微控制器上运行一个 2890 万参数的大语言模型，通过逐层嵌入技巧将模型适配到有限的内存中。 这一突破首次将大语言模型推理推向超低成本硬件，扩展了边缘 AI 的边界。它有望使物联网设备普惠 AI 能力，并开启离线语音助手或智能传感器等新应用。 该模型采用逐层嵌入技巧减少内存占用，使其适配仅 520KB SRAM 的 ESP32。ESP32 是一款双核微控制器，配备 Wi-Fi 和蓝牙，但没有 AI 硬件加速器。

hackernews · boveyking · 7月25日 18:59 · [社区讨论](https://news.ycombinator.com/item?id=49050512)

**背景**: ESP32 是乐鑫科技推出的一款流行的低成本微控制器，广泛用于物联网项目。边缘 AI 是指在设备本地运行机器学习模型，而非在云端。大语言模型通常需要强大的 GPU；在微控制器上运行它们需要量化、内存共享等极致优化技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://micropython.org/download/">MicroPython - Python for microcontrollers</a></li>
<li><a href="https://precisionaiacademy.com/blog/edge-ai-explained">Edge AI Explained 2026: Running ML on Tiny Devices</a></li>
<li><a href="https://zbotic.in/esp32-edge-ai-run-tensorflow-lite-micro-on-microcontroller/">ESP32 Edge AI : Run TensorFlow Lite Micro on Microcontroller - Zbotic</a></li>

</ul>
</details>

**社区讨论**: 评论者认为该项目令人印象深刻，并提到存在如 Milk-V 等内存更大、带 TPU 的廉价微控制器。一些人讨论了将大语言模型与小 TTS 模型结合以实现离线语音交互。另一些人则对产生这些权重的训练过程比推理本身更感到惊叹。

**标签**: `#edge AI`, `#microcontroller`, `#LLM`, `#efficiency`, `#embedded ML`

---

<a id="item-6"></a>
## [通用汽车投资钠离子电池用于美国电网储能](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 8.0/10

通用汽车宣布支持将钠离子电池用于美国电网储能，强调相比 LFP 电池，可通过减少 HVAC 能耗实现运营成本节约。 这一投资表明对钠离子技术的兴趣日益增长，该技术可降低电网储能成本并减少对锂的依赖，尤其在热管理成本高昂的应用场景中。 钠离子电池在更宽的温度范围内性能稳定，无需昂贵的加热和冷却系统，但能量密度较低且放电电压曲线不够平坦。

hackernews · rbanffy · 7月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=49051947)

**背景**: 锂离子电池（尤其是 LFP）主导电网储能市场，但需要热管理来维持性能。钠离子电池使用储量丰富的钠，可能降低成本并降低供应链风险，但现有生产线为锂而优化，阻碍了其采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_battery">Sodium-ion battery - Wikipedia</a></li>
<li><a href="https://battlebornbatteries.com/blogs/articles/sodium-ion-vs-lithium-batteries">Sodium-Ion Batteries: The Hype vs. Reality</a></li>
<li><a href="https://physics.aps.org/articles/v17/73">Physics - Sodium as a Green Substitute for Lithium in Batteries</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论因锂价下跌导致的制造惯性以及放电曲线等技术权衡。一些人认为 HVAC 节能是重要驱动力，而另一些人质疑通用汽车的角色及可能对中国硬件的依赖。

**标签**: `#sodium-ion batteries`, `#grid storage`, `#energy storage`, `#GM`, `#battery technology`

---

<a id="item-7"></a>
## [Fly.io 转向 AI 沙盒，因 Sprite 漏洞更换 CEO](https://fly.io/blog/kurt-scott-money-sprites/) ⭐️ 8.0/10

Fly.io 宣布战略转向 AI 沙盒，承认其 Sprite 产品存在严重漏洞，并更换 CEO 为 Scott Johnston。 这一转变反映了 AI 代理对可靠、持久代码执行环境日益增长的需求，该领域竞争激烈。CEO 变动表明在产品可靠性失败后，公司正转向运营稳定。 Sprite 是持久化、硬件隔离的 Linux 微 VM，空闲时休眠并按需唤醒，但初始版本存在数据丢失和僵尸状态问题。新版本将面向 AI 代理和评估场景。

hackernews · subarctic · 7月25日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=49051369)

**背景**: Fly.io 是一家以托管 Elixir 应用和边缘计算闻名的云平台。Sprite 是一种有状态沙盒，用于运行任意代码，与 E2B、Docker 沙盒等产品竞争。此次转型旨在占领日益增长的 AI 代码执行市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fly.io/">Computers for agents · Fly</a></li>
<li><a href="https://lewoudar.medium.com/lets-talk-about-fly-io-sprites-aka-stateful-sandboxes-509796942fdd">Let’s talk about Fly . io Sprites aka stateful sandboxes | Medium</a></li>
<li><a href="https://northflank.com/blog/e2b-vs-sprites-dev">E2B vs Sprites dev: comparing AI code execution... — Northflank</a></li>

</ul>
</details>

**社区讨论**: 社区成员报告了 Sprite 的严重可靠性问题，包括数据丢失和状态不一致，导致用户不满。一些人认为转向竞争激烈的市场是无奈之举，而另一些人则认为这是对 AI 趋势的必要适应。

**标签**: `#fly.io`, `#sprites`, `#infrastructure`, `#AI sandboxes`, `#CEO change`

---

<a id="item-8"></a>
## [Ruff v0.16.0 将默认规则从 59 条增加到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 7 月 23 日发布，将默认规则集从 59 条增加到 413 条。这意味着许多以前可选的检查现在默认启用，可能会破坏依赖旧配置的 CI 流水线。 这一重大版本更新显著影响开发者工作流程，无需任何配置即可捕获更多严重问题，如语法错误和运行时错误。然而，它可能导致现有 CI 流水线因新的违规而失败，项目维护者需要修复问题或更新 linter 设置。 自 v0.1.0 以来，Ruff 的规则总数已从 708 条增加到 968 条，许多新的默认规则会捕获诸如不带 'tz' 参数的 'datetime.datetime.now()'、盲目捕获异常和无效属性访问等问题。升级命令 'uvx ruff@latest check . --fix --unsafe-fixes' 可以自动修复许多违规，例如在 sqlite-utils 上修复了 1618 个错误中的 1538 个。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是一个用 Rust 编写的快速 Python linter，以其性能和广泛的规则集而闻名。以前默认仅启用 59 条规则，用户需要手动启用额外规则。在 v0.16.0 中，Astral 团队将默认集扩展到包括许多捕获严重问题的规则，旨在开箱即用地提高代码质量。

**标签**: `#Python`, `#linter`, `#Ruff`, `#tooling`, `#release`

---

<a id="item-9"></a>
## [从头在 ARM64 汇编中实现 YOLO26n 推理](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/) ⭐️ 8.0/10

一位开发者完全使用 ARM64 汇编和 C 语言实现了 YOLO26n 神经网络推理，不依赖任何框架，并为树莓派 4 上的边缘 AI 进行了优化。 这项工作展示了底层优化技术（Winograd 卷积、NEON SIMD、缓存感知分块），可以显著加速资源受限设备上的 CNN 推理，有利于边缘 AI 社区。 该实现包括自定义 ARM64 微内核、算子融合以及模型参数的自定义二进制格式，但作者指出性能提升低于预期并寻求反馈。

reddit · r/MachineLearning · /u/Forward_Confusion902 · 7月26日 06:43

**背景**: YOLO（You Only Look Once）是一个流行的实时目标检测模型系列。Winograd 卷积减少了卷积层中的乘法次数，ARM NEON SIMD 实现了 ARM 处理器上的并行数据处理。C2PSA 是 YOLOv11 中引入的双分支注意力模块，用于增强特征表示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winograd-convolution">Winograd Convolution in CNNs</a></li>
<li><a href="https://www.emergentmind.com/topics/c2psa-module">C2PSA Module: Dual-Branch Attention</a></li>
<li><a href="https://docs.ultralytics.com/guides/yolo-architecture">YOLO Architecture Explained | Ultralytics Docs</a></li>

</ul>
</details>

**标签**: `#ARM64`, `#YOLO`, `#edge AI`, `#assembly`, `#inference optimization`

---

<a id="item-10"></a>
## [LLM 在 IMO 2026 上测试：框架提升小型模型表现](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 8.0/10

一项研究比较了 LLM 在全新 IMO 2026 题目上的表现，发现前沿模型（sol 和 fable）无论是否使用框架都获得接近满分，而框架工程（Claude Code、AutoFyn）显著提升了 Sonnet、Opus 和 GLM 等小型模型的性能。 该基准测试提供了严谨证据，表明模型规模和原生推理能力在硬数学中仍占主导地位，但框架可以大幅缩小小型模型的差距，指导 AI 在复杂问题求解中的实际部署。 评分由前沿模型进行并由前 IMO 奖牌得主手动验证；幻觉问题依然存在（例如 Sonnet 在 P3 题上），并且没有亚前沿模型能解决最难问题的关键归约，即使运行了 20 小时。

reddit · r/MachineLearning · /u/pequalnp92 · 7月26日 07:21

**背景**: 国际数学奥林匹克竞赛（IMO）的题目新颖且需要多步推理，能测试通用智能，且不在 LLM 训练数据中。LLM 框架是围绕模型的生态系统，提供检索、验证和多智能体协调，以提升模型在复杂任务上的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/EleutherAI/lm-evaluation-harness">GitHub - EleutherAI/lm-evaluation- harness : A framework for few-shot...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://open-data-analytics.medium.com/what-is-an-agent-harness-and-why-it-decides-how-good-your-ai-agent-is-fe1c120f05af">What Is an Agent Harness , and Why It Decides How Good... | Medium</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#mathematical reasoning`, `#IMO`, `#multi-agent`

---

<a id="item-11"></a>
## [微软将用 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

微软宣布将在其 KMS 批量激活系统中加入基于 TPM 芯片的硬件身份验证，要求 KMS 服务器先证明其硬件身份经微软认证且未被篡改，然后才能处理激活请求。该功能将从下一版 Windows Server 起成为强制要求，并自 2026 年 8 月起在 Windows Server 2025 中推送准备提示。 这一反盗版措施可能有效终结广泛使用的伪造 KMS 激活方法，影响企业软件许可和盗版生态系统。然而，猫鼠游戏仍在继续，像 Massgrave 这样的组织声称已开发出 TSforge 等绕过方法。 TPM 证明机制确保只有经过硬件认证的正版 KMS 主机才能激活客户端。微软已于 2025 年封死了 KMS38 漏洞，新的 TPM 证明可能使需要定期连接伪造服务器的 Online KMS 激活方式失效。

telegram · zaihuapd · 7月25日 15:55

**背景**: TPM（可信平台模块）是一种专用芯片，通过存储设备独有的加密密钥提供硬件级安全，可用于验证硬件身份。KMS（密钥管理服务）是企业用于批量激活多个 Windows 客户端的授权方法，需使用 KMS 主机密钥。盗版激活长期利用伪造 KMS 服务器冒充正版主机来绕过验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys">Key Management Services (KMS) client activation and product keys | Microsoft Learn</a></li>
<li><a href="https://www.notebookcheck.net/Microsoft-Windows-and-Office-activation-cracked-again-TSforge-introduces-a-new-more-permanent-DRM-bypass.963349.0.html">Microsoft Windows and Office activation cracked again: TSforge ...</a></li>

</ul>
</details>

**标签**: `#TPM`, `#Windows activation`, `#DRM`, `#KMS`, `#cybersecurity`

---

<a id="item-12"></a>
## [DeepSeek 因内部言论外泄暂停新一轮融资](https://www.bloomberg.com/news/articles/2026-07-25/deepseek-said-to-tell-backers-of-funding-pause-after-viral-posts) ⭐️ 8.0/10

DeepSeek 已口头通知部分第二轮意向投资者暂停签署投资协议，部分原因是创始人梁文锋对网上流传的内部讨论内容感到不满。 这一融资暂停表明这家中国 AI 初创公司可能存在治理问题，影响其估值和 IPO 时间表，并可能影响投资者对更广泛 AI 领域的信心。 DeepSeek 于 2026 年 6 月完成首轮融资，筹集 70 亿美元；暂停的第二轮融资原计划募资至少 100 亿元人民币，投前估值不低于 4800 亿元人民币。

telegram · zaihuapd · 7月26日 01:17

**背景**: DeepSeek 是一家开发大型语言模型的中国知名人工智能公司。公司近期从腾讯、宁德时代及国家人工智能产业投资基金等投资者处获得了 70 亿美元的首轮融资。此次暂停发生在公司筹备首次公开募股之际，可能最早于 2026 年提交申请。

**标签**: `#AI`, `#DeepSeek`, `#funding`, `#business`, `#China`

---

<a id="item-13"></a>
## [近 200 家硅谷公司敦促特朗普不要禁止中国开放权重 AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

包括 Proton 和 Y Combinator 在内的近 200 家硅谷公司致信特朗普政府，反对可能禁止美国获取中国开放权重 AI 模型。 此类禁令将严重损害依赖低成本中国开放权重模型的美国初创企业，削弱其竞争力并扼杀创新。 该信函由 Little Tech Association 组织，主张采取有针对性的安全措施而非全面禁止。关于可能禁止的报道已在初创企业界引起恐慌。

telegram · zaihuapd · 7月26日 02:00

**背景**: 开放权重 AI 模型是指其训练参数公开发布的模型，任何人都可以下载、检查、修改并在自己的硬件上运行。它们与完全开源模型不同，因为训练数据和代码可能不包含在内。像 DeepSeek 这样的中国公司已经生产了流行的开放权重模型，许多全球初创企业用来构建应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open-weight models`, `#Silicon Valley`, `#geopolitics`, `#startups`

---