---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 41 条内容中筛选出 12 条重要资讯。

---

1. [Shai-Hulud 供应链攻击入侵 Keyv 及相关 npm 包](#item-1) ⭐️ 9.0/10
2. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](#item-2) ⭐️ 9.0/10
3. [Mistral 发布 3B 开放权重审核模型 Shieldstral](#item-3) ⭐️ 8.0/10
4. [生成多元肤色的简单算法与色彩空间](#item-4) ⭐️ 8.0/10
5. [Waymo 在达拉斯向公众开放无人驾驶出租车服务](#item-5) ⭐️ 8.0/10
6. [联邦快递的钓鱼式邮件削弱用户信任](#item-6) ⭐️ 8.0/10
7. [优化智能体 Harness 以支持自改进](#item-7) ⭐️ 8.0/10
8. [MiniMax-H3 全模态模型通过 MLX 在 Apple Silicon 上本地运行](#item-8) ⭐️ 8.0/10
9. [白宫闭门敲定 AI 评估框架，细节不公开](#item-9) ⭐️ 8.0/10
10. [华为提出‘韬定律’：以时间缩微替代几何缩微](#item-10) ⭐️ 8.0/10
11. [Cloudflare 弃用第三方安全工具，用 58 美元/月 AI 处理漏洞赏金](#item-11) ⭐️ 8.0/10
12. [我国首部 L3/L4 自动驾驶强制性国标报批，2027 年实施](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Shai-Hulud 供应链攻击入侵 Keyv 及相关 npm 包](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

攻击者入侵了 keyv 维护者的 GitHub 账户，keyv 是一款周下载量超 1.27 亿次的 npm 键值存储库，并利用该访问权限在维护者的整个包组合中推送窃取凭据的恶意软件。这一 Shai-Hulud 蠕虫感染了 79 个包名下的 353 个版本，在仓库钩子仍然存在的情况下窃取了开发者和 CI 凭证。 由于 keyv 的周下载量达 1.27 亿，是广泛使用的依赖项，此次供应链攻击十分严重，恶意代码可能蔓延至整个 npm 生态系统。该攻击紧随另外两起重大 npm 供应链事件，凸显了依赖系统长期存在的脆弱性。 此次攻击与 Shai-Hulud 蠕虫相关，该蠕虫利用包生态系统的自动化机制进行传播。被入侵的包包含安装前钩子或仓库钩子，清理后仍然存在，使攻击者能够窃取开发者和 CI 流水线的凭据。

hackernews · cimi_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: Keyv 是 Node.js 生态中一个简单的键值存储库，常配合各种后端适配器用于数据缓存。Shai-Hulud 这类供应链攻击瞄准开发者与开源包之间的信任关系，通过入侵维护者账号向广泛使用的项目中注入恶意代码。此次事件是 npm 生态攻击更广泛趋势的一部分，此前已发生 s1ngularity 攻击以及 Josh Junon(Qix)被入侵事件，后者是 18 个 npm 包的维护者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/keyv-npm-package-compromised/">Keyv npm Package with 127M Weekly Downloads Compromised in Shai-Hulud ...</a></li>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code ...</a></li>
<li><a href="https://www.securityweek.com/shai-hulud-supply-chain-attack-worm-used-to-steal-secrets-180-npm-packages-hit/">Shai - Hulud Supply Chain Attack : Worm Used to... - SecurityWeek</a></li>

</ul>
</details>

**社区讨论**: 社区对依赖系统的脆弱性表达了深切担忧，有评论者呼吁暂停使用安装前和安装后钩子。其他人则提出了实际缓解措施，例如在 npmrc 中设置'min-release-age=5'以避免采用刚发布的可疑包，还有人分享了关于 npm 供应链攻击技术的最新文档。

**标签**: `#supply chain`, `#npm`, `#security`, `#open source`, `#dependency management`

---

<a id="item-2"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 9.0/10

《金融时报》报道，谷歌已悄然搭建了史上最大规模的基础设施融资架构之一，支持向 Anthropic 交付超过 1500 亿美元的 AI 芯片。相关合同总额约 2000 亿美元；今年 6 月，名为 Compute SPV 的特殊目的载体完成首批交易，购入约 350 亿美元硬件。 这标志着 AI 资本开支的融资方式发生范式转变——通过华尔街的风险分担，将数十亿美元的芯片和数据中心成本移出企业资产负债表。此举也加深了谷歌对 Anthropic 算力供应链的控制，并可能为整个 AI 行业开创一种可复制的融资模板。 由于 Anthropic 没有信用评级，各方分担风险：谷歌为数据中心提供担保，博通购买并协助融资芯片，阿波罗与黑石购买硬件后回租给 Anthropic。6 月 Compute SPV 首批交易约合 1 吉瓦算力、100 万颗 TPU；该模式借鉴了波音、GE 推销飞机和发动机的厂商融资玩法。

telegram · zaihuapd · 8月4日 10:52

**背景**: TPU（张量处理单元）是谷歌为 AI 计算设计的专用加速芯片，负责训练和推理等场景。SPV（特殊目的载体）是为隔离金融风险而设立的法律实体，常见于资产证券化和项目融资中。厂商融资则是一种由来已久的做法——由制造商支持客户购买其设备，此次被用来为庞大的 AI 算力基础设施提供资金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://money.udn.com/money/story/5628/9173216?from=edn_related_storybottom">谷 歌 TPU 橫空出世 多平台浪潮崛起 | 社論 | 專欄 | 經濟日報</a></li>
<li><a href="https://baike.baidu.com/item/SPV/5115244">SPV（词汇简称）_百度百科 SPV架构全解析：跨境投资中的风险隔离、税务优化与资金流动设计指南 什么是SPV公司隔离？附真实的SPV隔离案例详解！ - 今日头条 什么是SPV，WFOE，BVI？大白话讲你知 - 今日头条 境外投资必读：什么是SPV（特殊目的公司）？设立流程、政策依据与实务... 特殊目的实体_百度百科</a></li>

</ul>
</details>

**标签**: `#AI Infrastructure`, `#Google`, `#Anthropic`, `#Financing`, `#Chips`

---

<a id="item-3"></a>
## [Mistral 发布 3B 开放权重审核模型 Shieldstral](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral 发布了 Shieldstral，这是一个 3B 参数的开放权重多模态安全分类器，能够在推理时根据用自然语言编写的审核策略判断文本和图像。它的表现优于最高达其规模 7 倍的模型，并在多模态安全分类方面达到了新的最先进水平。 这使得大规模内容审核变得经济高效且易于部署，对较小平台尤其有帮助。它顺应了专注于小型专用模型的趋势，为大型审核 API 提供了一种实用的替代方案。 该模型将内容审核表述为二元问答任务，并具有策略自适应性，即可以在推理时调整策略而无需重新训练。该开放权重模型可在 Hugging Face 上获得，名称为 mistralai/Shieldstral-1.0-3B。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**背景**: 开放权重模型是指训练参数公开可下载的 AI 模型，用户可以在自己的设备上运行、研究甚至修改它们。内容审核通常依赖大型专有分类器或昂贵的人工审核；一个小的、策略自适应的分类器提供了一种灵活的中间选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://arxiv.org/html/2607.25857v1">Shieldstral - arXiv.org</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 评论者对该模型能否处理任意规则集、还是仅沿用现有固定审核风格感到好奇，其中一人提到无需重新训练即可调整策略的潜力。另一位用户开玩笑说应该叫“Safestral”，并称赞 Mistral 专注于小型微调模型的策略，还有用户询问它与 OpenAI 的审核 API 相比如何。有评论者表示，它似乎是图像分享平台一个现实且经济高效的解决方案。

**标签**: `#AI`, `#content-moderation`, `#open-weights`, `#Mistral`, `#LLM`

---

<a id="item-4"></a>
## [生成多元肤色的简单算法与色彩空间](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 8.0/10

作者介绍了一种自定义色彩空间和简单方程，用于生成多样且可信的肤色，并附带一个基于 JavaScript 的颜色选择器和程序化生成算法（含 Python 示例），以及交互式演示。 这为数字艺术家和游戏开发者提供了一个实用且包容的肤色选取工具，解决了常见的痛点。它也为创意工具中关于包容性和色彩建模的持续讨论做出了贡献。 该色彩空间通过 PCA 将三维肤色数据降为二维，然后手动拟合椭圆和函数来构建平滑方程。页面中包含“未来工作”部分，指出了局限性和改进空间。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 色彩空间是一种用数值表示颜色的系统，而肤色在标准 RGB 或 Lab 空间中构成一个复杂且非均匀的区域。程序化生成是一种通过算法创建内容的方法，广泛用于游戏和数字艺术中。现有的肤色调色板往往无法涵盖人类肤色的全部多样性，因此推动了专用色彩空间的研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>
<li><a href="https://en.wikipedia.org/wiki/Procedural_generation">Procedural generation - Wikipedia</a></li>
<li><a href="https://news.ycombinator.com/item?id=49170165">Show HN: Simple algorithm and color space to generate diverse skin tones | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这项工作，有人认为从 PCA 降到 2D 再到手动拟合函数的手法很巧妙，还有人将其结果与 Oklab 和 Pudding 的粉底色号数据联系起来。建设性批评包括没有引用 Pantone 肤色系统，以及部分生成颜色出现绿色、蓝色或紫色色相的问题。

**标签**: `#color-space`, `#skin-tone`, `#procedural-generation`, `#digital-art`, `#algorithm`

---

<a id="item-5"></a>
## [Waymo 在达拉斯向公众开放无人驾驶出租车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 宣布其无人驾驶出租车服务现已向达拉斯所有公众开放，覆盖达拉斯-沃斯堡都会区。 此次扩张将全无人驾驶出行带到一个以汽车为主的大都会区，为居民提供了新的交通选择，并表明自动驾驶技术正从最初的试点城市向外规模化推广。同时，正如社区讨论所示，它也引发了关于基础设施、安全和城市政策的重要讨论。 Waymo 在达拉斯的服务区域覆盖达拉斯-沃斯堡都会区，其车辆使用配备摄像头、LiDAR 和雷达传感器套件的 Waymo Driver 系统。该服务为完全无人驾驶，车内无安全驾驶员。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 始于 2009 年谷歌的自动驾驶汽车项目，2016 年作为 Alphabet 旗下独立公司分拆。2020 年 10 月，它成为首家在没有安全驾驶员的情况下提供公开机器人出租车服务的公司。机器人出租车是提供按需出行的自动驾驶车辆，它们通过摄像头、LiDAR 和雷达等传感器套件，并结合软件来安全地导航道路。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Robotaxi">Robotaxi - Wikipedia</a></li>
<li><a href="https://waymo.com/waymo-driver/">Self-Driving Car Technology for a Reliable Ride - Waymo Driver</a></li>

</ul>
</details>

**社区讨论**: 评论者的情绪总体积极但克制，强调 Waymo 车辆可预测且事故少于人类驾驶员，尤其是与洛杉矶攻击性驾驶员相比。一位用户指出，尽管 DFW 密度低且汽车文化重，但服务很受欢迎；另一位则认为无人驾驶出租车可作为一种有效的经济适用房政策，减少对停车和公共交通投资的需求。也有人提到偶尔出现车辆卡住等问题，但总体热情较高。

**标签**: `#autonomous-vehicles`, `#waymo`, `#robotaxi`, `#transportation`, `#policy`

---

<a id="item-6"></a>
## [联邦快递的钓鱼式邮件削弱用户信任](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

在 2024 年的一篇博文中，安全研究员 Troy Hunt 记录了联邦快递的合法通知邮件如何具备钓鱼攻击的特征，比如意外的请求和看似可疑的链接。他认为，这些令人困惑但真实的邮件训练用户忽略危险信号，使真正的钓鱼攻击更难被识别。 这很重要，因为大品牌自身的邮件做法会削弱安全意识，让用户更容易受到真实钓鱼和社会工程攻击。它揭示了一个系统性问题：即使是善意的公司，也在侵蚀人们区分合法通信与恶意通信的关键线索。 博文引用了评论者提供的真实案例，包括由联邦快递员工个人发送的带有 PDF 附件的海关通知，以及使用 c.gle 短链接的 Google 存储空间提醒。这些案例表明，即使是安全意识较强的用户，也很难验证看似可疑但实际合法的通信。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**背景**: 电子邮件欺骗和钓鱼攻击利用了早期电子邮件协议缺乏内置身份验证的缺陷，攻击者可以伪造发件人地址并冒充可信品牌。社会工程攻击依靠心理操纵，常利用紧迫感、恐惧或熟悉感来诱导受害者点击恶意链接或泄露凭据。当合法公司发送设计糟糕、与攻击模式相似的邮件时，会在无意中让用户对警示信号变得麻木。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Email_spoofing">Email spoofing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Social_engineering_(security)">Social engineering (security) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了亲身体验，印证了 Hunt 所述困惑：有人描述一封来自联邦快递员工个人的海关邮件最终被证实是真的，还有人质疑 Google 的 c.gle 链接是否合法。其他评论指出，新顶级域名的激增，以及诈骗者和合法机构共用语音助手等做法，让非专业人士更难判断真实性。

**标签**: `#phishing`, `#email security`, `#security awareness`, `#social engineering`

---

<a id="item-7"></a>
## [优化智能体 Harness 以支持自改进](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

Lilian Weng 发表了一篇关于 Harness 工程的文章，认为优化 LLM 智能体的外部脚手架（工具、提示词和上下文）可以显著提升性能、质量和成本效率。文章提出智能体应该自我改进其 Harness，而不是只依赖模型权重。 Harness 工程正成为与模型权重并列的独立性能杠杆；同一模型在不同 Harness 下性能可相差达 6 倍。自动化 Harness 优化能减少手工工程投入，提高生产级智能体的可靠性和成本效益，对构建 LLM 系统的研究人员和工程师都有重要影响。 近期如 Meta-Harness 的研究将 Harness 视为端到端可优化空间，用完整执行轨迹而非压缩摘要来优化，取得了显著更好的效果（中位数分数 50.0 对 34.9）。社区实验显示，自动研究可以把加载上下文的过程从 20k token、15 次工具调用压缩到 800 token、1 次工具调用。

hackernews · tosh · 8月4日 06:17 · [社区讨论](https://news.ycombinator.com/item?id=49164896)

**背景**: 在 LLM 智能体系统中，Harness 指围绕模型的外部执行支持结构，也就是决定模型存储、检索和接收哪些信息的代码，包括提示词、工具接口、规划产物、验证循环、记忆系统和沙箱等。长期以来 Harness 主要靠人工设计，但近期研究将其视为一个独立的、可优化的性能杠杆，与基础模型能力互补。Lilian Weng 的这篇文章正是这一日益受关注的 Harness 工程方向的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.28052">Meta-Harness: End-to-End Optimization of Model Harnesses (PDF) Advanced Optimization Techniques For Large Language ... Meta-Harness: End-to-End Optimization of Model Harnesses Agentic Harness: Code-Driven LLM Optimization LLM Model Optimization Techniques and Frameworks Meta-Harness — automatically optimizing the code around the LLM GitHub - ai-boost/awesome-harness-engineering: Awesome list ...</a></li>
<li><a href="https://www.preprints.org/manuscript/202606.2203">Harness Engineering for LLM Agents : A Survey of... | Preprints.org</a></li>
<li><a href="https://zendevy.com/en/ai/harness-engineering-prompt-context-evolution/">Harness Engineering : From Prompts to Runtime Control — ZenDevy</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体积极且带有前瞻性。参与者提出了一些实践路径，例如为代码库构建通用适应度函数、利用自动研究分析执行轨迹来发现问题并修复；还有人猜测 Harness 是否会生成自己的 RLHF/DPO 训练集。也有评论者分享个人项目或开玩笑，比如‘Torment Nexus 的探索’。

**标签**: `#AI agents`, `#LLMs`, `#harness engineering`, `#optimization`

---

<a id="item-8"></a>
## [MiniMax-H3 全模态模型通过 MLX 在 Apple Silicon 上本地运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

MiniMax 发布了 MiniMax-H3，这是一个可处理文本、图像、音频和视频的全模态生成模型。Simon Willison 演示了新的 MLX 移植版（PipeNetwork/minimax-h3-mlx），使其能在 Apple Silicon 上运行，并在他的 M5 Max MacBook Pro 上根据文本提示生成了 15 秒的视频片段。 这一进展意义重大，因为它将最先进的全模态模型——支持文本、图像、音频和视频的输入/输出——带到了消费级 Apple 硬件上，而不仅仅是云端 API。它降低了本地多模态实验的门槛，也凸显了 MLX 在 AI 生态系统中日益重要的作用。 运行该模型需要下载约 115 GB 的模型文件；在 Willison 的测试中，生成一个视频耗时近 45 分钟。在没有提示词指导的情况下，音频输出被形容为“奇怪的、类似语音的乱码”，MiniMax 提供了提示词编写指南来改善效果。

rss · Simon Willison · 8月4日 19:10

**背景**: 全模态模型（omni-modal model）是能在统一架构中跨多种数据模态（如文本、图像、音频和视频）进行感知与生成的 AI 模型，通常在共享潜在空间内操作，而不是像一些系统那样把独立训练的模型拼接起来。MLX 是 Apple 开源的数组与机器学习框架，专为 Apple Silicon 设计，提供熟悉的 Python API 并支持高效的本地推理。这个移植版将 MiniMax-H3 的权重转换为 MLX 格式，使开发者能够在 Mac 上运行大型多模态生成模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/omni-model/">What’s an Omni-Model? Definition, Uses, and Benefits | NVIDIA Glossary</a></li>

</ul>
</details>

**标签**: `#MLX`, `#MiniMax`, `#omni-modal`, `#video generation`, `#Apple Silicon`

---

<a id="item-9"></a>
## [白宫闭门敲定 AI 评估框架，细节不公开](https://www.axios.com/2026/08/03/white-house-finalizes-ai-framework-behind-closed-doors) ⭐️ 8.0/10

该框架可能成为前沿 AI 模型发布前的事实审查机制，影响 OpenAI、谷歌、Anthropic 等主要开发者。细节保密引发透明度担忧，但也表明 AI 监管正通过行政渠道推进。 该框架明确了保密、网络安全、知识产权保护和保密协议等要求，并列出可提前访问模型的“可信伙伴”名单。行政令将模型能力基准测试及适用门槛列为机密信息。

telegram · zaihuapd · 8月4日 02:31

**背景**: 自愿 AI 评估框架是用于在模型部署前衡量其能力和风险的标准测试套件。白宫 6 月 2 日的行政令要求制定这一框架，政府除 Anthropic、OpenAI 和谷歌外，还在与众多业界伙伴商讨后续步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/ainewswire_google-stax-aims-to-make-ai-model-evaluation-activity-7378790904440074240-WwQs">Google launches Stax, a customizable AI evaluation framework for...</a></li>
<li><a href="https://epoch.ai/benchmarks">Data on AI Capabilities and Benchmarking | Epoch AI</a></li>
<li><a href="https://www.codesota.com/tasks">Every AI Capability — Benchmark Evidence and Trust | CodeSOTA</a></li>

</ul>
</details>

**标签**: `#AI政策`, `#模型评估`, `#白宫`, `#监管`, `#AI安全`

---

<a id="item-10"></a>
## [华为提出‘韬定律’：以时间缩微替代几何缩微](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

在 2026 年国际电路与系统研讨会上，华为提出‘韬定律’（τ缩放定律），主张以时间缩微取代几何缩微作为半导体演进的新原则。华为称过去六年已按该定律设计并量产 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟手机芯片。 若经验证，韬定律可在不依赖最先进光刻机的情况下延续半导体进步，突破摩尔定律的物理极限，影响整个芯片产业。对华为乃至中国而言，这尤其重要，为在出口管制下达到先进芯片密度和系统性能提供了替代路径。 韬定律通过华为‘逻辑折叠’多层级协同优化，在器件、电路、芯片和系统各层面系统性地降低特征时间常数τ。华为预计，到 2031 年基于该定律的高端芯片晶体管密度可达 1.4 纳米制程同等水平，并表示未来将以开放合作推动产业发展。

telegram · zaihuapd · 8月4日 08:04

**背景**: 摩尔定律是半导体行业长期遵循的经验法则，即晶体管密度大约每两年翻一番；但随着单纯靠缩小尺寸带来的收益递减，该定律正逼近物理极限。几何缩微指不断缩小芯片上的特征尺寸，而时间缩微则通过降低决定器件开关速度的时间常数，从器件、电路、芯片到系统多个层面进行协同优化，以提升密度、能效和性能。韬定律于 2026 年 IEEE ISCAS 会议上发布，相关理论论文已在中国预印本平台 ChinaXiv 上公开。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.globaltimes.cn/page/202605/1361841.shtml">Huawei unveils new semiconductor law, charting fresh path for industry development - Global Times</a></li>
<li><a href="https://chinarxiv.org/items/chinaxiv-202605.00224">A Time Scaling Theory for Multi-Layer Electronic Systems</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#Huawei`, `#Moore's Law`, `#chip design`, `#hardware innovation`

---

<a id="item-11"></a>
## [Cloudflare 弃用第三方安全工具，用 58 美元/月 AI 处理漏洞赏金](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare 首席安全官 Grant Bourzikas 在悉尼的一次活动上透露，该公司现在使用 Anthropic 的 Claude Sonnet 自动化处理漏洞赏金报告，每月仅花费 58 美元，而使用安全专用模型则需约 20 万美元/月。公司还构建了 200 多个自主安全代理，并基本弃用第三方安全工具，改用自研应用。 这件事之所以重要，是因为它展示了一家大型科技公司以极低的成本将 AI 代理和前沿模型应用于核心安全工作流程，可能重塑安全运营的人员配置与工具选型方式。它也标志着行业正更广泛地向 AI 驱动自动化转型，对安全厂商和安全团队的角色都将产生影响。 Bourzikas 明确提醒其他企业不要效仿 Cloudflare 的做法，称并非每家银行都该自己开发所有软件。此外，首席战略官 Stephanie Cohen 将公司此前裁员 1100 人归因于 AI 带来的自动化变革，并透露 Cloudflare 计划通过微支付充当 AI 公司与出版商之间的中介。

telegram · zaihuapd · 8月4日 09:24

**背景**: Claude Sonnet 是 Anthropic 推出的中端大语言模型，属于包含 Haiku（最小）和 Opus（最大）的模型家族。2026 年，Anthropic 还发布了 Claude Mythos，这是一款专门的自主网络安全模型，能够发现并利用漏洞，最初仅向部分组织提供。Cloudflare 使用更便宜的通用型 Sonnet 进行漏洞赏金分类，说明许多安全任务并不需要最昂贵的专用模型。该公司的做法反映了企业自建 AI 代理流程、而非简单购买现成安全产品的新趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Sonnet">Claude Sonnet</a></li>
<li><a href="https://www.contrastsecurity.com/glossary/mythos-ai">What Is Mythos AI? Autonomous Exploits and AppSec Defense | Contrast Security</a></li>
<li><a href="https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities">Our evaluation of Claude Mythos Preview’s cyber capabilities | AISI Work</a></li>

</ul>
</details>

**标签**: `#AI`, `#Security`, `#Cloudflare`, `#Automation`, `#Bug Bounty`

---

<a id="item-12"></a>
## [我国首部 L3/L4 自动驾驶强制性国标报批，2027 年实施](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

我国工业和信息化部已完成《智能网联汽车自动驾驶系统安全要求》强制性国家标准报批稿，并于 6 月 17 日起公示。该标准建议 2027 年 7 月 1 日实施，是我国首部针对 L3 和 L4 级自动驾驶的强制性国标，并引入了 Safety Case 安全档案机制。 这标志着自动驾驶监管从宽松的营销化宣传转向可执行的安全硬约束。车企必须通过结构化论证系统性地证明安全性，这将重塑中国自动驾驶行业的研发、测试与合规流程。 该标准要求企业采用'声明—论据—证据'的结构建立 Safety Case 安全档案，在全生命周期内论证安全性。同时对 L3 级系统提出人机交接和驾驶人接管能力监测要求，对 L4 级系统提出自主风险处置能力要求。

telegram · zaihuapd · 8月4日 13:06

**背景**: L3 和 L4 是 SAE 定义的高级驾驶自动化等级：L3 在特定条件下可由系统驾驶，但需人类在请求时接管；L4 则可在限定场景内无需人工干预完成全部驾驶任务。Safety Case 是一套由证据支持的结构化安全论证体系，源于高风险行业，用于证明系统在特定环境下运行是可接受安全的，使监管逻辑从'满足条款'转向'自证安全'。中国工程院院士李骏指出，2026 年是全球自动驾驶安全监管的拐点，行业将全面进入 Safety Case 时代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/966/272.htm">我国首部 L3/L4 自动驾驶强制性国标公示：2027 年 7 月起正式实施，车...</a></li>
<li><a href="https://baike.baidu.com/item/Safety+Case/67871945">Safety Case - 百度百科</a></li>
<li><a href="https://www.sohu.com/a/1040778204_100084983">中国工程院院士李骏：自动驾驶安全进入Safety Case时代</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#China`, `#L3/L4`

---