---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 39 条内容中筛选出 15 条重要资讯。

---

1. [华为昇腾 950 超节点首秀，宣称算力达英伟达 6.7 倍](#item-1) ⭐️ 9.0/10
2. [月之暗面发布开源 2.8 万亿参数模型 Kimi K3](#item-2) ⭐️ 9.0/10
3. [美国拟设类似 FINRA 的独立机构监管顶级 AI 模型](#item-3) ⭐️ 9.0/10
4. [JWST 确认类地行星 LHS 1140b 首次发现大气层](#item-4) ⭐️ 8.0/10
5. [Kimi K3 与鹈鹕基准测试：训练数据争议](#item-5) ⭐️ 8.0/10
6. [开源 AI 模型市场份额激增](#item-6) ⭐️ 8.0/10
7. [FAA 恢复波音 737 MAX 和 787 自认证资格](#item-7) ⭐️ 8.0/10
8. [解决问题的三种非解决式应对方式分析](#item-8) ⭐️ 8.0/10
9. [实时 SSH 蜜罐可视化展示机器人攻击](#item-9) ⭐️ 8.0/10
10. [Prism 漏洞泄露研究者论文](#item-10) ⭐️ 8.0/10
11. [美议员呼吁禁止中国存储芯片进入盟友供应链](#item-11) ⭐️ 8.0/10
12. [OpenAI CFO 提出‘每美元有用智能’衡量 AI 投资回报](#item-12) ⭐️ 8.0/10
13. [Meta 与 Anthropic 洽谈百亿美元 AI 算力租赁](#item-13) ⭐️ 8.0/10
14. [SpaceX 与五角大楼谈判 AI 算力交易](#item-14) ⭐️ 8.0/10
15. [台积电宣布 A14 制程将于 2028 年投产](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [华为昇腾 950 超节点首秀，宣称算力达英伟达 6.7 倍](https://www.ithome.com/0/978/019.htm) ⭐️ 9.0/10

华为在 2026 世界人工智能大会上首次公开展示昇腾 950 超节点（Atlas 950 SuperPoD），声称其通过 1024 卡集群提供 1 EFLOPS FP8 和 2 EFLOPS FP4 算力，拥有 256 TB 全局统一内存，据中银证券报告，总算力达到英伟达 144 卡 NVL144 系统的 6.7 倍。 这标志着中美 AI 芯片竞争的重大里程碑，可能重塑大规模 AI 训练基础设施格局，降低中国企业对于英伟达硬件的依赖。 昇腾 950 采用华为自研灵衢（UnifiedBus）互联协议和超节点架构，支持最多 1024 卡无收敛互联。此外，昇腾 384 超节点已商用落地 750 多套，广泛应用于互联网、运营商、金融等行业。

telegram · zaihuapd · 7月17日 10:27

**背景**: 超节点是一种通过高速互联技术将多台服务器紧密连接，使其像一台巨型计算机一样协同工作的 AI 计算系统，对于训练万亿参数大语言模型至关重要。华为的灵衢协议是一个五层协议栈，替代 PCIe、NVLink 和 RDMA，可实现多达 8192 卡的无损扩展。昇腾 950 代表了华为在 AI 加速器领域挑战英伟达主导地位的最新举措。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/cn/news/2026/7/atlas-950-superpod">昇腾950超节点真机亮相2026世界人工智能大会</a></li>

</ul>
</details>

**标签**: `#华为`, `#昇腾950`, `#AI芯片`, `#算力`, `#数据中心`

---

<a id="item-2"></a>
## [月之暗面发布开源 2.8 万亿参数模型 Kimi K3](https://t.me/zaihuapd/42637) ⭐️ 9.0/10

月之暗面发布了全球首个开源 2.8 万亿参数模型 Kimi K3，在 Frontend Code Arena 基准测试中以 1679 分排名第一，超越了 Claude Fable 5。 此次发布表明，大规模开源模型在专业编程任务上可以与闭源领导者竞争，可能加速前端开发等领域对大型开源模型的采用。 Kimi K3 基于 Kimi Delta Attention 和 Attention Residuals 架构，具备原生视觉能力和 100 万 token 上下文窗口。其前代 Kimi k2.6 排名第 18，而 K3 跃升至第一，在 Frontend Code Arena 的 7 个评测领域中 6 项领先。

telegram · zaihuapd · 7月18日 02:29

**背景**: 大型语言模型消耗大量计算资源，高效的注意力机制至关重要。Kimi Delta Attention 是一种线性注意力变体，它扩展了 Gated DeltaNet，引入通道级衰减，在保持质量的同时降低内存使用。Attention Residuals 用学习到的注意力替代标准残差连接，提升深度效率。Frontend Code Arena 评估 AI 生成的网页应用代码，涵盖品牌、响应性和交互性等类别。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/moonshot-releases-2-8-trillion-parameter-kimi-k3">China's 2.8-trillion-parameter Kimi K3 beats Claude Fable 5 in Frontend Code Arena benchmark— Moonshot AI delivers largest open-weight AI model ever, as China works around U.S. compute limits | Tom's Hardware</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear [2505.11254] Delta Attention: Fast and Accurate Sparse ... Attention Mechanisms | NVlabs/GatedDeltaNet | DeepWiki hwilner/kimi-delta-attention - GitHub Delta Attention Residuals — cere-bro DeltaNet Explained (Part I) | Songlin Yang</a></li>
<li><a href="https://arxiv.org/pdf/2603.15031">Attention Residuals</a></li>

</ul>
</details>

**标签**: `#大语言模型`, `#开源`, `#月之暗面`, `#2.8T参数`, `#前端编程`

---

<a id="item-3"></a>
## [美国拟设类似 FINRA 的独立机构监管顶级 AI 模型](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 9.0/10

特朗普政府正考虑设立一个类似金融业监管局（FINRA）的独立 AI 监管机构，负责审查顶尖 AI 模型的安全性。该提案由财政部长斯科特·贝森特牵头，目前正由白宫幕僚长苏茜·威尔斯审阅。 这一政策举措可能重塑美国 AI 监管格局，回应华尔街对网络安全的担忧以及硅谷对政府临时管控措施的不满。如果实施，它将让两大行业在制定高级 AI 模型安全标准方面拥有更大发言权。 该提案与 Google DeepMind 首席执行官德米斯·哈萨比斯提出的设立行业资助独立监管机构的建议方向一致。然而，总统特朗普尚未审阅该方案，相关框架仍在讨论中，内容可能有所调整。

telegram · zaihuapd · 7月18日 05:45

**背景**: FINRA 是一家美国私人公司，作为经纪交易商和交易所市场的自律组织。拟议中的 AI 监管机构将类似地由行业资助并独立运作，向证券交易委员会报告。这一方法旨在借鉴金融行业的监管模式，平衡创新与安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Financial_Industry_Regulatory_Authority">Financial Industry Regulatory Authority - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#government policy`, `#Trump administration`, `#AI safety`, `#FINRA`

---

<a id="item-4"></a>
## [JWST 确认类地行星 LHS 1140b 首次发现大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

天文学家利用詹姆斯·韦伯空间望远镜（JWST）的发射光谱，在红矮星宜居带内的岩石行星 LHS 1140b 上探测到了大气层，排除了它是迷你海王星的可能性。 这是在宜居带内岩石类地系外行星上首次确认存在大气层，标志着系外行星特征描述和潜在生物标志物搜寻的一个重要里程碑。 LHS 1140b 约为地球大小的 1.7 倍，距离地球 48 光年；JWST 在行星经过恒星背后时进行的二次食光谱分析显示，其光谱特征与厚氢氦大气层不符。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 比地球大但比海王星小的系外行星常被分类为超级地球或迷你海王星。迷你海王星拥有厚实的氢氦大气层。JWST 通过凌星光谱法，在行星凌星或掩星期间分析穿过其大气的星光，从而确定其成分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2301.04191">[2301.04191] A JWST transmission spectrum of a nearby Earth-sized exoplanet</a></li>

</ul>
</details>

**社区讨论**: 评论中对红矮星行星能保留大气层表示惊讶，但指出 JWST 数据排除了迷你海王星的可能性。其他人讨论了太阳透镜望远镜、星际推进技术以及费米悖论中通信时间窗口的影响。

**标签**: `#exoplanet`, `#astronomy`, `#atmosphere`, `#habitable zone`, `#JWST`

---

<a id="item-5"></a>
## [Kimi K3 与鹈鹕基准测试：训练数据争议](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

Simon Willison 使用他非正式的“骑自行车的鹈鹕”基准测试评估了新的 Kimi K3 模型，引发了关于训练数据污染和分词奇特现象的讨论。社区还提出了该基准测试的对抗性扩展方案。 这一讨论凸显了 LLM 评估的挑战，尤其是那些能揭示训练数据污染的创造性基准测试。分析还揭示了隐藏的系统提示和跨模型的分词不一致性，这些因素影响着成本和性能的比较。 Simon 指出，Kimi K3 生成了一只不错的鹈鹕 SVG，但也证实了他的怀疑：该提示很可能出现在训练数据中。一位评论者发现，向 Kimi K3 输入“hi”消耗了 86 个 token，暗示存在一个与推理努力相关的 85 个 token 的隐藏系统提示。

hackernews · droidjj · 7月17日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: “骑自行车的鹈鹕”基准测试是 Simon Willison 创建的一个非正式测试，要求 LLM 生成一只骑自行车的鹈鹕的 SVG 图像。该测试用于评估创造性编码和视觉推理能力。Kimi K3 是中国初创公司 Moonshot AI 推出的 2.8 万亿参数模型，拥有 100 万 token 的上下文窗口并开源了权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为训练数据污染很可能是事实，有人指出他们自己博客的内容在 6 个月内就出现在 LLM 中。其他人提出了对抗性变体，例如在 SWE-bench 中插入需要生成 SVG 的中断，以更好地测试模型的鲁棒性。

**标签**: `#LLM evaluation`, `#Kimi K3`, `#benchmark`, `#AI safety`, `#community discussion`

---

<a id="item-6"></a>
## [开源 AI 模型市场份额激增](https://stateofopensource.ai/) ⭐️ 8.0/10

开源 AI 模型在 OpenRouter 上的 token 处理量已超过闭源模型，四个月内增长了近 5 倍。 这一转变挑战了 OpenAI 和 Anthropic 等公司的闭源模型的主导地位，可能降低开发者和企业的成本并提高可及性。 根据 OpenRouter 数据，3 月 19 日开源模型处理了 8880 亿个 token；到 7 月，这一数字达到 4.19 万亿个 token。市场份额从闭源模型占 60%转向开源模型占 63%。

hackernews · rellem · 7月17日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源 AI 模型可公开使用和修改，通常无需许可费用；而闭源模型是专有的，需要付费访问。这一增长凸显了 AI 技术民主化的更广泛趋势。

**社区讨论**: 评论者对开源模型超越闭源模型表示乐观，一位用户指出 token 处理量大幅增长。也有人批评原始演示文稿由 LLM 生成，缺乏真正的分析。

**标签**: `#open-source AI`, `#AI models`, `#market trends`, `#LLMs`

---

<a id="item-7"></a>
## [FAA 恢复波音 737 MAX 和 787 自认证资格](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html) ⭐️ 8.0/10

美国联邦航空管理局（FAA）恢复了波音公司为 737 MAX 和 787 梦想飞机自行颁发适航证书的权力，该权力在 2018 年和 2019 年致命坠机事件后被撤销。 这标志着波音在监管恢复方面迈出了重要一步，可能会加快飞机交付并减少 FAA 的监督，但也引发了批评者对于恢复松懈自我监管的安全担忧。 根据组织委派授权（ODA）计划，波音现在可以在没有 FAA 直接检查的情况下颁发适航证书，但 FAA 保留对设计型号证书和整体安全合规的监督。

hackernews · hmm37 · 7月17日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=48952439)

**背景**: 适航证书确认单架飞机符合其经批准的设计型号并可以安全运行，与验证整体设计的型号证书不同。FAA 的 ODA 计划允许像波音这样的授权公司代表 FAA 执行认证任务。在 737 MAX 坠机事件后，FAA 撤销了波音颁发适航证书的 ODA 权力，要求 FAA 直接参与。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.faa.gov/newsroom/faa-statement-boeing-airworthiness-certificates">FAA Statement - Boeing Airworthiness Certificates | Federal Aviation Administration</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX_certification">Boeing 737 MAX certification - Wikipedia</a></li>
<li><a href="https://skybrary.aero/articles/organisation-designation-authorisation-oda">Organisation Designation Authorisation ( ODA )</a></li>

</ul>
</details>

**社区讨论**: 评论者对适航证书和型号证书的区别感到困惑，有人指出多次重新认证使 737 系列得以延续。其他人表达了恐惧和质疑，认为恢复授权背后存在政治或经济动机。

**标签**: `#aviation`, `#regulation`, `#Boeing`, `#FAA`, `#safety`

---

<a id="item-8"></a>
## [解决问题的三种非解决式应对方式分析](https://improvesomething.today/responses-to-problems/) ⭐️ 8.0/10

一篇题为《Three ways people respond to a problem (other than solving it)》的文章指出了三种常见的非解决式应对方式：推卸、维持原状以及忽视或淡化。 这很重要，因为它揭示了组织和软件工程中适得其反的行为，帮助团队识别并避免此类陷阱，从而提高问题解决的效率。 该文章发布于 improvesomething.today，社区参与度高，获得 219 个点赞和 120 条评论，表明其与软件工程和组织行为高度相关。

hackernews · surprisetalk · 7月17日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=48947490)

**背景**: 解决问题是一项核心技能，但人们常常因为激励、权力动态或目标不明确而回避直接解决问题。这三种应对方式为诊断这些行为和理解潜在动机提供了一个框架。

**社区讨论**: 评论者指出，忽视问题有时是策略性的，维持问题可能让当权者受益，推卸问题可能是关于任务委派。他们还提出了第四种反应：改变问题以适应个人目标。

**标签**: `#problem-solving`, `#organizational behavior`, `#decision-making`, `#software engineering`

---

<a id="item-9"></a>
## [实时 SSH 蜜罐可视化展示机器人攻击](https://honeypotlive.cc/) ⭐️ 8.0/10

新网站 honeypotlive.cc 提供了 SSH 蜜罐交互的实时可视化，展示机器人实时尝试登录并执行命令的过程。 该项目将看不见的自动化攻击变得可见，帮助网络安全社区了解攻击模式以及蜜罐在威胁情报中的重要性。 该可视化很可能使用 Cowrie SSH 蜜罐作为数据源，它记录了攻击者的命令，并可通过 pip 安装。站点还实时显示命令输出，包括垃圾信息和恶意活动。

hackernews · tusksm · 7月17日 14:05 · [社区讨论](https://news.ycombinator.com/item?id=48947548)

**背景**: SSH 蜜罐是一种模拟真实 SSH 服务的诱饵服务器，用于引诱攻击者。它会记录所有活动以供分析，帮助研究人员研究自动化机器人攻击和凭证填充。Cowrie 是一个知名的开源蜜罐，支持 SSH 和 Telnet，并具有先进的 shell 解析功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Honeypot_(computing)">Honeypot (computing) - Wikipedia</a></li>
<li><a href="https://github.com/jaksi/sshesame">An easy to set up and use SSH honeypot, a fake SSH server ...</a></li>

</ul>
</details>

**社区讨论**: Cowrie 的作者确认该站点展示了典型的互联网背景噪音，并强调了 Cowrie 近期改进。其他评论者提到了一个相关的 LLM 驱动蜜罐项目（honeyprompt），并指出用户正在滥用 Web 界面发送大量文本，降低了观察真实机器人模式的能力。

**标签**: `#cybersecurity`, `#honeypot`, `#SSH`, `#real-time monitoring`

---

<a id="item-10"></a>
## [Prism 漏洞泄露研究者论文](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 8.0/10

OpenAI 的 Prism LaTeX 编译器中的一个 bug 意外地将其他用户的论文返回给一名研究者，导致未发表的工作被泄露。该问题在 Discord 和 Twitter 上被指出，Prism 团队在 10 分钟内关闭了网站。 这一事件凸显了 AI 辅助科学工具中的严重隐私和安全风险，可能暴露敏感的未发表研究。它削弱了依赖此类平台进行协作工作的研究人员的信任。 该 bug 出现在编译过程中，导致跨用户论文泄露。受影响的用户担心自己的论文也可能已经被暴露。

reddit · r/MachineLearning · /u/Few-Monitor5103 · 7月17日 17:59

**背景**: Prism 是 OpenAI 提供的一款免费 LaTeX 编辑器及 AI 原生工作空间，集成了 GPT-5.2 以辅助研究人员写作和协作。它旨在简化科学文档创建，但像任何基于云的工具一样，引发了数据隐私和安全方面的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/prism/">Prism | A free, LaTeX Editor and AI-native workspace for ...</a></li>
<li><a href="https://openai.com/index/introducing-prism/">Introducing Prism - OpenAI</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#security`, `#paper leak`, `#Prism`, `#privacy`

---

<a id="item-11"></a>
## [美议员呼吁禁止中国存储芯片进入盟友供应链](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 8.0/10

美国众议院中国委员会主席 John Moolenaar 和民主党议员 George Whitesides 致信商务部长 Howard Lutnick，要求将长鑫存储（CXMT）列入实体清单，并对长江存储（YMTC）施加额外限制，理由是对美国国家、经济及供应链安全构成不可接受的风险。 此举可能重塑全球存储芯片供应链，迫使美国及盟友公司排除中国 DRAM 和 NAND Flash，可能导致战略依赖并扰乱苹果等科技巨头的采购。 议员们还敦促与日本、韩国和欧盟协调，防止中国制造商在供应短缺时扎根于盟友供应链，尤其在 AI 基础设施关键组件方面。长鑫存储和长江存储近期被移出美国国防部 CMC 清单，但合规风险依然存在。

telegram · zaihuapd · 7月17日 14:00

**背景**: 长鑫存储是中国领先的 DRAM 制造商，长江存储专注于 NAND Flash。美国实体清单限制外国实体未经许可购买美国技术。这些中国存储企业因涉嫌与军方关联而屡遭美国制裁，尽管近期被移出一个黑名单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/長江存儲">长江存储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/實體清單">实体清单 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#supply chain`, `#China`, `#memory chips`, `#regulation`

---

<a id="item-12"></a>
## [OpenAI CFO 提出‘每美元有用智能’衡量 AI 投资回报](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 8.0/10

OpenAI 首席财务官 Sarah Friar 提出了一个以‘每美元有用智能’为核心的四维框架来衡量 AI 投资回报，倡导基于成果的评估而非传统的 token 成本指标。该公告还强调了 GPT-5.6 Sol 模型，该模型在编码任务上达到最先进水平，输出 token 比竞品减少 54%。 该框架将企业 AI 评估从简单的采用率指标转向基于价值的生产力衡量标准，使组织能够做出更明智的投资决策。同时，它也强调了模型效率和可靠性的重要性，这直接影响生产中的总拥有成本。 四个维度分别是：完成的有用工作量、每个成功任务的全成本、AI 输出的可靠性，以及随使用增长每美元投入是否产生更多价值。OpenAI 展示了其最强编码模型 GPT-5.6 Sol，它在使用不到一半输出 token 且每任务成本降低约三分之一的情况下，性能超越了竞品模型。

telegram · zaihuapd · 7月17日 15:00

**背景**: 传统的 AI 成本衡量侧重于 token 价格——即每处理单位文本的成本。然而，更便宜的模型可能需要多次尝试或更长的输出才能完成任务，导致总成本更高。‘每美元有用智能’指标捕捉了 AI 实际交付的价值，考虑了完成的工作量、可靠性和规模化效率。这类似于衡量人类劳动的生产力而非仅仅关注小时工资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://andresseo.expert/ai/openais-new-ai-scorecard-the-metric-that-finally-measures-roi-beyond-token-costs/">OpenAI's AI Scorecard: Measuring Useful Intelligence per Dollar</a></li>
<li><a href="https://tomtunguz.com/tokens-per-result">Intelligence Per Dollar | Tomasz Tunguz</a></li>

</ul>
</details>

**标签**: `#AI ROI`, `#OpenAI`, `#productivity metrics`, `#GPT-5.6`, `#AI economics`

---

<a id="item-13"></a>
## [Meta 与 Anthropic 洽谈百亿美元 AI 算力租赁](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta 正在与人工智能初创公司 Anthropic 进行早期谈判，拟将 AI 算力租借给对方，潜在交易规模高达 1000 亿美元，为期两年；该方案由 Anthropic 于 2026 年 6 月提出。 该交易凸显了 AI 算力的极度稀缺性，同时可能为 Meta 开辟新的收入来源，并向投资者证明其巨额基础设施支出的合理性。 Anthropic 将按月付款，双方均可提前退出。Meta 正在评估该提案，谈判尚处早期阶段，因此交易未必能达成。

telegram · zaihuapd · 7月18日 01:14

**背景**: AI 算力（compute）是训练和运行大型语言模型（如 Anthropic 开发的模型）的关键资源。Meta 一直在大力投资数据中心，仅 2026 年就计划投入高达 1450 亿美元，部分用于支持其自身的 AI 研发。将闲置算力租给其他公司，有助于 Meta 将其投资变现，并缓解投资者对资本支出的担忧。

**标签**: `#AI compute`, `#Meta`, `#Anthropic`, `#datacenter`, `#business deal`

---

<a id="item-14"></a>
## [SpaceX 与五角大楼谈判 AI 算力交易](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX 正与美国国防部谈判，拟提供用于运行 AI 模型的数据中心算力，潜在交易金额高达数十亿美元。 该交易将标志着 SpaceX 从火箭发射和卫星互联网服务大幅扩展至国防 AI 云计算领域，可能重塑 AI 基础设施供应商的竞争格局。 谈判仍在进行中，仍有可能破裂。SpaceX 近期还与 Anthropic 和谷歌签署了类似的算力供应协议，并计划大幅扩展其云计算业务。

telegram · zaihuapd · 7月18日 01:44

**背景**: SpaceX 以其提供全球宽带互联网的 Starlink 卫星星座和可重复使用火箭而闻名。五角大楼正在加速获取云计算能力，以支持国家安全和日常行动中的 AI 应用，其中包括一项名为“AI 兵工厂”的新专项计划，寻求 300 亿美元预算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbeta.com.tw/articles/science/1569346.htm">SpaceX洽谈为 五 角 大 楼 AI 计划提供算力支持 - SpaceX - cnBeta.COM</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starlink">SpaceX Starlink</a></li>

</ul>
</details>

**标签**: `#AI`, `#云计算`, `#国防`, `#SpaceX`, `#五角大楼`

---

<a id="item-15"></a>
## [台积电宣布 A14 制程将于 2028 年投产](https://t.me/zaihuapd/42643) ⭐️ 8.0/10

台积电宣布其下一代 A14 制程技术计划于 2028 年投产，与即将量产的 N2 制程相比，相同功耗下速度提升高达 15%，或相同速度下功耗降低达 30%。 这一宣布重申了台积电在先进半导体制造领域保持领先地位的路线图，对需要更高性能和效率的 AI 及高性能计算芯片至关重要。 与 N2 相比，A14 的逻辑密度提升超过 20%。台积电还计划在 2026 年末推出中间的 A16 制程，该制程将集成 Super Power Rail 背面供电技术。

telegram · zaihuapd · 7月18日 05:00

**背景**: 台积电的 N2 是其首个采用环绕栅极（GAA）纳米片晶体管的制程节点，将于 2025 年量产。A16 是一个 1.6 纳米级别的节点，结合了 GAAFET 与背面供电技术。A14 可能是一个 1.4 纳米级别的节点，代表了 A16 之后的下一步。这些节点是台积电持续缩小晶体管、提升每瓦性能以制造领先芯片战略的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tsmc.com/english/dedicatedFoundry/technology/logic/l_A16">A16 Technology - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/tsmc-begins-quietly-volume-production-of-2nm-class-chips-first-gaa-transistor-for-tsmc-claims-up-to-15-percent-improvement-at-iso-power">TSMC begins quietly volume production of 2nm-class chips — first GAA transistor for TSMC claims up to 15% improvement at ISO power | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductor`, `#chip manufacturing`, `#A14`, `#process technology`

---