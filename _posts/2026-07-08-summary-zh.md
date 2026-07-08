---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 43 条内容中筛选出 14 条重要资讯。

---

1. [MIRA：用于火箭联盟的 50 亿参数世界模型发布](#item-1) ⭐️ 9.0/10
2. [Januscape KVM 逃逸漏洞：影响 Intel 和 AMD 的 16 年旧漏洞](#item-2) ⭐️ 9.0/10
3. [DeepSeek 自研 AI 推理芯片，减少对英伟达和华为依赖](#item-3) ⭐️ 9.0/10
4. [腾达固件隐藏后门可获取管理员权限](#item-4) ⭐️ 8.0/10
5. [欧盟聊天控制提案威胁端到端加密](#item-5) ⭐️ 8.0/10
6. [欧盟强制所有新车安装驾驶员监控摄像头](#item-6) ⭐️ 8.0/10
7. [sqlite-utils 4.0 发布，支持数据库模式迁移](#item-7) ⭐️ 8.0/10
8. [可微分光线追踪用于无线电传播建模的博士论文](#item-8) ⭐️ 8.0/10
9. [可信 LoRA 适配器子空间阻止恶意微调更新](#item-9) ⭐️ 8.0/10
10. [美国生产英伟达 Blackwell 晶圆，但封装仍需台湾](#item-10) ⭐️ 8.0/10
11. [中国考虑对顶级 AI 模型实施出口管制](#item-11) ⭐️ 8.0/10
12. [我国人形机器人年产量 2026 年有望突破 10 万台](#item-12) ⭐️ 8.0/10
13. [Claude Cowork 上线：AI 可后台自动完成复杂任务](#item-13) ⭐️ 8.0/10
14. [阿里下令员工 7 月 10 日前卸载 Claude](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MIRA：用于火箭联盟的 50 亿参数世界模型发布](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 9.0/10

这标志着多智能体世界建模的一个重要里程碑，证明大规模交互式模拟可以在当前硬件上高效训练和运行。它为多智能体规划、模拟和游戏 AI 的 AI 研究开辟了新的可能性，并且开源发布使更广泛的社区能够进行探索。 该模型拥有 50 亿参数，在单个采用 Blackwell 架构的 B200 GPU 上以 20 帧每秒的速度运行 4 人模拟。数据集包含 1000 小时的 4 人火箭联盟游戏记录，技术报告提供了深入的方法论细节。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: 世界模型是一种人工智能系统，它学习环境的内部表示，并预测环境如何随着行动而演变。世界模型用于规划、模拟和强化学习，使智能体无需持续与环境交互就能推理未来的结果。这项工作将世界模型应用于复杂的多人视频游戏，展示了其在多智能体场景中的潜力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>

</ul>
</details>

**标签**: `#world models`, `#deep learning`, `#reinforcement learning`, `#video game AI`, `#multi-agent`

---

<a id="item-2"></a>
## [Januscape KVM 逃逸漏洞：影响 Intel 和 AMD 的 16 年旧漏洞](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

安全研究人员公开了 Januscape（CVE-2026-53359），这是首个同时影响 Intel 和 AMD 平台的 KVM/x86 虚拟机逃逸漏洞，并发布了概念验证利用代码。 该漏洞打破了客户机与宿主机内核之间的隔离边界，对多租户云环境及任何基于 KVM 的虚拟化部署构成严重威胁。 该漏洞是 shadow MMU 模拟中的释放后使用缺陷，允许客户机通过内部操作破坏宿主机内核的 shadow 页表，导致宿主机内核崩溃。

telegram · zaihuapd · 7月7日 10:14

**背景**: KVM（基于内核的虚拟机）是一个 Linux 内核模块，允许宿主机运行多个虚拟机。Shadow MMU 是在硬件支持不足时用于管理内存虚拟化的组件。该漏洞在 Linux 内核中从 2010 年存在至 2026 年 6 月，潜伏期长达 16 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://docs.kernel.org/virt/kvm/x86/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://security.googleblog.com/2024/06/virtual-escape-real-reward-introducing.html">Virtual Escape; Real Reward: Introducing Google’s kvmCTF</a></li>

</ul>
</details>

**标签**: `#security`, `#virtualization`, `#KVM`, `#vulnerability`, `#Linux kernel`

---

<a id="item-3"></a>
## [DeepSeek 自研 AI 推理芯片，减少对英伟达和华为依赖](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 9.0/10

DeepSeek 自研 AI 推理芯片已进行约一年，旨在减少对美国出口管制下对英伟达和华为芯片的依赖。该芯片专注于推理而非训练，公司已开始招聘芯片设计工程师并接洽代工厂。 此举标志着 AI 硬件供应链的战略转变，一家中国领先 AI 公司寻求摆脱对西方及受制裁芯片供应商的依赖。若成功，可能削弱美国出口管制对中国 AI 产业的影响。 该芯片处于早期阶段，专为推理任务设计。DeepSeek 此前依赖英伟达 H800 和华为昇腾芯片，创始人梁文锋在 2024 年一次罕见采访中承认芯片限制是公司面临的挑战。

telegram · zaihuapd · 7月7日 11:08

**背景**: DeepSeek 是一家以大型语言模型闻名的中国 AI 公司。美国出口管制限制英伟达 H100 等先进 AI 芯片对华销售，迫使企业寻找替代方案。华为也生产昇腾 AI 芯片，但性能不及英伟达顶级产品。近期华为路线图显示昇腾 950PR 推理芯片性能达 1.56 PFLOPs，挑战英伟达 H20。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>
<li><a href="https://www.huaweicentral.com/huawei-reveals-3-year-ascend-ai-chip-roadmap-950-coming-in-2026/">Huawei reveals 3-year Ascend AI chip roadmap, 950 coming in 2026</a></li>
<li><a href="https://laweconcenter.org/resources/us-export-controls-on-ai-and-semiconductors/">US Export Controls on AI and Semiconductors - International ...</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#DeepSeek`, `#chip design`, `#export controls`

---

<a id="item-4"></a>
## [腾达固件隐藏后门可获取管理员权限](https://kb.cert.org/vuls/id/213560) ⭐️ 8.0/10

多个版本的腾达固件中存在一个未记录的身份验证后门（CVE-2026-11405），使用硬编码密码'rzadmin'，允许攻击者获得设备 Web 管理面板的完全管理权限。 该漏洞影响多种腾达网络设备，包括路由器和交换机，可能危及家庭和企业网络。它突显了具有硬编码凭据的 IoT 设备中持续存在的安全风险。 后门位于/bin/httpd web 服务器二进制文件的 login()函数中。已确认五个特定固件版本易受攻击，包括 AC10、AC15 和 BE12Pro 型号的版本。

hackernews · miniBill · 7月8日 00:08 · [社区讨论](https://news.ycombinator.com/item?id=48825749)

**背景**: 硬编码密码是嵌入在源代码中的明文密码，可绕过正常身份验证。在 IoT 设备中，此类后门无需用户交互即可远程利用。该漏洞最初在 2022 年的一篇文章中被详细描述，现在已被分配 CVE-2026-11405。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hidden-backdoor-in-tenda-router-firmware-grants-admin-access/">Hidden backdoor in Tenda router firmware grants admin access</a></li>
<li><a href="https://thehackernews.com/2026/07/certcc-warns-of-hidden-admin-backdoor.html">CERT/CC Warns of Hidden Admin Backdoor in Tenda Router Firmware</a></li>
<li><a href="https://kb.cert.org/vuls/id/213560">VU#213560 - Tenda firmware (multiple versions) contains ...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，硬编码密码'rzadmin'在 2022 年的一篇博客文章中就已披露，且最近的固件已加密，增加了分析难度。一些人认为这是技术能力不足而非恶意行为，但建议避免使用腾达产品。

**标签**: `#security`, `#backdoor`, `#Tenda`, `#IoT`, `#hardcoded credentials`

---

<a id="item-5"></a>
## [欧盟聊天控制提案威胁端到端加密](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

欧盟提出了“聊天控制”法规（1.0 版和 2.0 版），要求平台扫描所有私人消息，包括端到端加密消息，以查找儿童性虐待材料。批评者认为这实际上破坏了加密，并建立了大规模监控基础设施。 如果实施，聊天控制将从根本上削弱端到端加密，影响数亿欧盟公民的隐私和安全。这为政府强制监控私人通信树立了危险的全球先例。 聊天控制 1.0 已于 2026 年 4 月到期，但聊天控制 2.0 的谈判仍在继续，计划进行三方会谈。该提案依赖客户端扫描（client-side scanning），即在用户设备上加密之前分析内容，引发了关于后门和安全性降低的技术与法律担忧。

hackernews · gasull · 7月7日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 聊天控制指欧盟为打击在线儿童性虐待材料（CSAM）而制定的一系列法规。这些提案要求数字平台检测并报告 CSAM，可能通过扫描所有消息来实现。客户端扫描是一种有争议的方法，它在数据被加密和发送之前在设备上检查数据，可能被用于更广泛的监控，并削弱对加密的信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://fightchatcontrol.eu/chat-control-overview">Chat Control 1.0 vs 2.0 - Fight Chat Control</a></li>
<li><a href="https://www.internetsociety.org/resources/doc/2020/fact-sheet-client-side-scanning/">Fact Sheet: Client-Side Scanning - Internet Society</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈反对这些提案，用户称其为“夺取独裁权力”和“令人毛骨悚然的监控国家”。技术问题被提出，关于如何扫描加密消息，参考了政府后门或类似苹果 CSAM 扫描器的设备端扫描，并担心误报会影响无辜用户。

**标签**: `#privacy`, `#encryption`, `#EU legislation`, `#surveillance`, `#technology policy`

---

<a id="item-6"></a>
## [欧盟强制所有新车安装驾驶员监控摄像头](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

根据欧盟最新法规，所有在欧盟销售的新车必须配备驾驶员监控摄像头系统，以检测疲劳和分心驾驶。 这项强制规定深刻影响了欧洲的车辆安全与隐私规范，波及数百万驾驶员和制造商，并引发了关于安全技术与个人隐私之间平衡的讨论。 该法规具体要求驾驶员疲劳与注意力警告（DDAW）系统，使用红外摄像头和人工智能监控眼球运动、头部位置等线索，作为欧盟一般安全法规（EU）2019/2144 的一部分。

hackernews · nickslaughter02 · 7月7日 20:50 · [社区讨论](https://news.ycombinator.com/item?id=48823557)

**背景**: 驾驶员监控系统（DMS）使用车内摄像头和传感器追踪驾驶员行为，例如视线方向和头部姿势，以检测分心或疲劳。此类系统已在部分豪华车型中使用，目前欧盟和美国监管机构正强制要求安装以提高道路安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=PI_COM:C(2023)4523">Advanced Drivers Distraction Warning (ADDW) - EUR-Lex</a></li>
<li><a href="https://spyro-soft.com/blog/automotive/driver-monitoring-systems-to-become-mandatory-under-new-eu-and-us-road-safety-regulations">Driver Monitoring Systems to become mandatory under new EU and US road safety regulations</a></li>

</ul>
</details>

**社区讨论**: 社区评论呈现了复杂情绪：许多用户报告了误报带来的困扰，例如不必要的刹车或蜂鸣声，而另一些人则认为这些系统准确且可能挽救生命，与飞机警报过载的对比突显了对设计和用户体验的担忧。

**标签**: `#regulation`, `#privacy`, `#automotive`, `#driver monitoring`, `#EU`

---

<a id="item-7"></a>
## [sqlite-utils 4.0 发布，支持数据库模式迁移](https://simonwillison.net/2026/Jul/7/sqlite-utils/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 sqlite-utils 4.0，这是一个重大版本更新，增加了对数据库模式迁移的内置支持，使开发者能够对 SQLite 数据库模式进行版本控制和应用增量更改。 模式迁移是管理生产环境中数据库演化的关键功能；此版本使 sqlite-utils 成为基于 SQLite 的项目更完整的工具，尤其对于依赖 Python 和 CLI 工作流的开发者。 该版本支持应用和回滚迁移，并同时提供 Python 库和命令行工具。两周前，发布了候选版本 4.0rc1，引入了迁移和嵌套事务功能。

rss · Simon Willison · 7月7日 15:42

**背景**: sqlite-utils 是 Simon Willison 创建的 Python 库和命令行工具，用于操作 SQLite 数据库。它在 Python 的 sqlite3 模块之上提供了更高级的操作。数据库模式迁移是一种管理数据库模式版本控制、增量更改的方法，常用于 DevOps 和软件开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>

</ul>
</details>

**标签**: `#sqlite-utils`, `#SQLite`, `#Python`, `#database`, `#migrations`

---

<a id="item-8"></a>
## [可微分光线追踪用于无线电传播建模的博士论文](https://www.reddit.com/r/MachineLearning/comments/1upvkp5/phd_thesis_on_differentiable_ray_tracing_for/) ⭐️ 8.0/10

一篇博士论文提出了用于无线电传播建模的可微分光线追踪框架，利用 JAX 自动微分计算通过物理环境的精确梯度，以求解逆问题和训练机器学习模型。 这项工作连接了无线通信与可微分仿真，为信道建模、定位和材料校准提供了基于梯度的优化方法。其开源发布（DiffeRT）使得这些技术可被用于下一代无线设计。 论文分为三部分：物理基础、GPU 加速路径追踪与不连续性平滑技术、实际应用。同时开源了基于 JAX 的 2D 可微分光线追踪工具箱 DiffeRT2d。

reddit · r/MachineLearning · /u/jeertmans · 7月7日 13:45

**背景**: 光线追踪通过模拟光线在环境中的传播路径来模拟波动传播。可微分光线追踪扩展了这一点，允许相对于场景参数计算梯度，从而实现优化。无线电传播模型预测无线电波的传播方式，对无线网络规划至关重要。该论文融合了这些领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Radio_propagation">Radio propagation - Wikipedia</a></li>
<li><a href="https://github.com/jeertmans/DiffeRT2d">GitHub - jeertmans/DiffeRT2d: 2D Toolbox for Differentiable ...</a></li>
<li><a href="https://people.csail.mit.edu/tzumao/diffrt/">Differentiable Monte Carlo Ray Tracing through Edge Sampling</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞论文的可读性和开源代码，认为其对无线通信和可微分编程具有潜在影响。

**标签**: `#differentiable ray tracing`, `#radio propagation`, `#automatic differentiation`, `#machine learning`, `#wireless communications`

---

<a id="item-9"></a>
## [可信 LoRA 适配器子空间阻止恶意微调更新](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

一篇新论文提出将微调限制在从可信 LoRA 适配器学习的子空间中，从而防止模型学习恶意更新。该方法在 196 个公开 LoRA 适配器上测试，并针对自适应攻击进行了评估，结果显示攻击成功率大幅下降，而有用适配能力基本保留。 这提供了一种新颖的微调投毒防御方法，无需检测投毒数据，有望提升在设备端适配或用户生成数据微调等场景下的 AI 安全性。它通过限制可学习行为的空间，将焦点从检测转向预防。 该方法依赖一个可信 LoRA 适配器池来定义子空间，保留有用适配的同时使恶意方向在几何上不可达。评估中包含了专门设计用于绕过该防御的自适应攻击，论文提供了公开代码和实验以供复现。

reddit · r/MachineLearning · /u/Bright_Warning_8406 · 7月7日 20:00

**背景**: LoRA（低秩适配）是一种高效微调大型模型的技术，通过在冻结基础模型的同时添加小型可训练适配器模块来实现。微调投毒指在训练集中注入恶意数据以诱导后门等隐藏行为。传统防御侧重于检测或过滤投毒数据，而本工作则采取不同方法，将模型的学习能力限制在可信行为的子空间内。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://www.paloaltonetworks.com/cyberpedia/what-is-data-poisoning">What Is Data Poisoning? [Examples & Prevention] - Palo Alto Networks</a></li>
<li><a href="https://www.ibm.com/think/topics/lora">What is LoRA (Low-Rank Adaption)? | IBM</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#AI safety`, `#fine-tuning`, `#LoRA`, `#adversarial robustness`

---

<a id="item-10"></a>
## [美国生产英伟达 Blackwell 晶圆，但封装仍需台湾](https://www.tomshardware.com/tech-industry/nvidia-and-intel-tout-chips-built-in-america-but-every-arizona-made-blackwell-die-is-still-packaged-in-taiwan) ⭐️ 8.0/10

英伟达 Blackwell 晶圆已在台积电亚利桑那州 Fab 21 采用定制 4NP 制程量产，但这些晶圆仍需运往台湾进行 CoWoS-L 先进封装和 HBM 集成。 这表明美国已能生产尖端逻辑芯片，但在先进封装上仍依赖台湾，这是 AI 芯片供应链中的关键瓶颈，具有地缘政治影响。 先进封装需要 CoWoS-L 技术和 HBM 内存堆叠，美国目前尚无量产这些的设施；Amkor、台积电和 SK 海力士正在建设相关产能，预计最早 2028-2029 年建成。

telegram · zaihuapd · 7月7日 09:47

**背景**: 英伟达 Blackwell 架构采用台积电定制 4NP 制程，拥有 2080 亿个晶体管。CoWoS-L 是台积电的一种先进封装技术，通过硅中介层将逻辑芯片与 HBM 堆叠集成。英特尔也在亚利桑那州投产了 18A 制程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm">CoWoS® - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.intel.com/content/www/us/en/foundry/process/18a.html">Intel 18A | See Our Biggest Process Innovation</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#NVIDIA`, `#supply chain`, `#manufacturing`, `#Blackwell`

---

<a id="item-11"></a>
## [中国考虑对顶级 AI 模型实施出口管制](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 8.0/10

中国商务部已与阿里巴巴、字节跳动及智谱 AI 等企业开会，讨论限制国产最先进人工智能模型向海外提供访问，包括尚未发布的模型。 这一政策可能通过限制中国领先模型的海外可用性来重塑全球 AI 格局，可能影响开源发布并加剧中美技术脱钩。 限制可能仅适用于未来发布的新模型，最终范围仍在讨论中。官员们还考虑将 AI 核心技术泄露或窃取定为国家安全罪行，并限制境外资本投资国内 AI 初创企业。

telegram · zaihuapd · 7月7日 11:42

**背景**: 中国已建立了强大的国内 AI 生态系统，如智谱 AI（国际品牌名为 Z.ai）推出 GLM 系列等开放权重模型。智谱 AI 于 2025 年 1 月被列入美国实体清单。拟议的出口管制将影响闭源和开源模型，可能波及全球依赖这些模型的开发者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qz.com/beijing-china-ai-model-export-restrictions-070726">China weighs restrictions on overseas access to its most ...</a></li>
<li><a href="https://worldview.ranenetwork.com/content/situational-report/2026-07-07/china-beijing-explores-potential-export-restrictions-on-advanced-ai-models">China: Beijing Explores Potential Export Restrictions on ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zhipu_AI">Zhipu AI</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#China`, `#technology policy`, `#export controls`, `#national security`

---

<a id="item-12"></a>
## [我国人形机器人年产量 2026 年有望突破 10 万台](https://www.news.cn/tech/20260707/1e0c79e82bb94a97a1488ebe3984834d/c.html) ⭐️ 8.0/10

工信部宣布，2026 年我国人形机器人整机产量有望突破 10 万台，规模以上工业企业人工智能应用普及率已超过 30%。 这一里程碑反映了中国在制造业中融合人工智能与机器人的快速进展，可能巩固其在工业自动化领域的全球领先地位，并加速经济转型。 国内已研制近 200 项人工智能关键标准，AtomGit 开源社区注册用户超过 1100 万。2026 年上海世界人工智能大会将有 1100 余家企业展示 3000 余项展品，其中超过 300 款产品为全球首发。

telegram · zaihuapd · 7月8日 02:25

**背景**: 人形机器人旨在模仿人类形态和运动，通常由大型 AI 模型和智能体驱动。“规模以上”指年收入超过一定门槛的企业。AtomGit 是一个中国开源平台，支持代码托管和社区协作，类似于 GitHub。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gitcode.com/">AtomGit - 全球开发者的开源社区,开源代码托管平台</a></li>
<li><a href="https://github.com/atomgit-atomcode/atomcode">GitHub - atomgit-atomcode/atomcode: An open-source ...</a></li>

</ul>
</details>

**标签**: `#humanoid robots`, `#AI adoption`, `#industrial AI`, `#China`, `#robotics`

---

<a id="item-13"></a>
## [Claude Cowork 上线：AI 可后台自动完成复杂任务](https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork) ⭐️ 8.0/10

Anthropic 面向 Pro、Max、Team 及 Enterprise 付费用户推出了 Claude Cowork，使 AI 能够在桌面端、网页和移动端后台自主完成多步骤复杂任务。 这标志着 AI 助手能力的重大进步，例如整理文件、生成表格和报告等任务现在可以独立运行，无需用户持续关注，从而大幅提升跨平台的生产力。 任务在 Anthropic 服务器上远程运行，即使关闭电脑也会继续；桌面端支持直接读写本地文件和浏览器操作，可设置定时自动任务并按项目管理。

telegram · zaihuapd · 7月8日 03:50

**背景**: Claude 是 Anthropic 开发的一系列大语言模型，于 2023 年 3 月首次发布，采用 constitutional AI 技术进行安全训练。Claude Cowork 是一个面向非技术办公任务的 AI 代理，能够访问 macOS 上的用户文件夹以读取、编辑、创建文件并执行异步工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://grokipedia.com/page/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#automation`, `#productivity`, `#Claude`

---

<a id="item-14"></a>
## [阿里下令员工 7 月 10 日前卸载 Claude](https://t.me/zaihuapd/42424) ⭐️ 8.0/10

阿里巴巴内部宣布反向禁用 Claude 及 Anthropic 其他产品，要求所有员工在 2025 年 7 月 10 日前卸载。此前，Anthropic 指控阿里在 2025 年 4 月 22 日至 6 月 5 日期间使用约 2.5 万个虚假账户与 Claude 交互超过 2800 万次。 这标志着中国大型科技公司重大政策转变，可能影响中国企业使用外国 AI 工具的方式，并加剧 AI 行业的竞争。同时，这也凸显了 Anthropic 等美国 AI 公司与中国企业之间因账户滥用和安全问题而日益紧张的关系。 禁令涉及 Anthropic 产品，包括 Sonnet、Opus、Fable 等模型，以及 Claude Code 等 Agent 产品。此前，阿里曾报销员工使用 Claude、GPT、Gemini 等外部模型的费用。

telegram · zaihuapd · 7月8日 06:09

**背景**: Claude 是美国公司 Anthropic 开发的一系列大型语言模型，于 2023 年 3 月首次作为 AI 聊天机器人发布。它采用宪法 AI 技术确保伦理合规，模型包括 Haiku、Sonnet、Opus 和 Fable。Claude Code 是一款 AI 辅助软件开发工具。阿里巴巴是一家专注于电子商务、云计算和 AI 的中国跨国企业集团。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model: Haiku, Sonnet, Opus, or Fable</a></li>

</ul>
</details>

**标签**: `#AI`, `#Alibaba`, `#Claude`, `#Anthropic`, `#corporate policy`

---