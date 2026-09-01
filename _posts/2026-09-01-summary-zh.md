---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 37 条内容中筛选出 8 条重要资讯。

---

1. [谷歌从 Chrome 网上应用店下架 Manifest V2 扩展](#item-1) ⭐️ 8.0/10
2. [NAT：互联网中心化的原罪？](#item-2) ⭐️ 8.0/10
3. [滑窗注意力在长上下文推理上击败线性注意力](#item-3) ⭐️ 8.0/10
4. [新工具 Entropic Scree 可评估脏数据中的信号强度](#item-4) ⭐️ 8.0/10
5. [Claude 共享链接遭搜索引擎索引，敏感用户数据大量泄露](#item-5) ⭐️ 8.0/10
6. [OpenClaw 2.0 史上最大更新，汇集逾 1.6 万个拉取请求](#item-6) ⭐️ 8.0/10
7. [DeepSeek 上线实验性视觉语言模型 deepseek-v4-flash-vision-exp](#item-7) ⭐️ 8.0/10
8. [小米发布三款玄戒芯片，O3 SoC 将首搭小米 18 Fold](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌从 Chrome 网上应用店下架 Manifest V2 扩展](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

谷歌已开始从 Chrome 网上应用店移除 Manifest V2（MV2）扩展，实质上下架了 uBlock Origin 等热门工具。升级到 Chrome 139 及后续版本的用户将无法再使用这些扩展。 这标志着 Chrome 强制向 Manifest V3 过渡的一个重要里程碑，许多隐私倡导者认为 MV3 会削弱广告拦截能力。这影响数百万用户，加剧了人们对谷歌控制网络的担忧，并促使部分用户转向 Firefox 等替代浏览器。 Manifest V3 通过用 declarativeNetRequest 取代阻塞式 webRequest API 并将过滤规则限制在约 3 万条来限制扩展能力。uBlock Origin 开发者建议使用 Firefox，因为那里仍提供完整版；Chrome 用户只能使用 uBlock Origin Lite。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: Manifest V2 是 Chrome 多年来使用的扩展规范，允许 uBlock Origin 等强大扩展现拦截网络请求并在广告加载前将其屏蔽。谷歌在 2019 年宣布 MV3，称其更安全、更私密、性能更好，但 EFF 等批评者认为这会损害广告拦截和用户自主权。Chrome 139 会禁用所有剩余的 MV2 扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V 2 support timeline | Chrome for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2021/12/googles-manifest-v3-still-hurts-privacy-security-innovation">Google’s Manifest V 3 Still Hurts Privacy, Security, and Innovation</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍谴责谷歌的决定，认为广告拦截是安全必需，并怀疑谷歌是在保护其广告收入。许多人建议改用 Firefox，有人指出 uBlock Origin 在 Firefox 上一直表现更好。整体情绪强烈反感 Chrome，并支持浏览器多元化。

**标签**: `#Chrome`, `#MV2`, `#uBlock Origin`, `#ad-blocking`, `#privacy`

---

<a id="item-2"></a>
## [NAT：互联网中心化的原罪？](https://dreamstation.systems/personal/ntppost.html) ⭐️ 8.0/10

一篇反思性文章认为，NAT（网络地址转换）是互联网早期中心化的关键推手，而 Linux NAT 的原始实现者 Rusty Russell 在评论中承认并详细说明了当年所做的技术决策。 Rusty Russell 解释说，他当年选择不保留端口，以便将更多连接塞进一个 IP 地址，这导致来自其他地址的入站流量无法路由，实际上消除了公共端点。评论者区分了普通可控 NAT（他们认为可以接受）和运营商级 NAT（CGNAT）（他们称之为“真正的邪恶”，因为它限制了用户的自由）。

hackernews · robinpie · 8月31日 02:23 · [社区讨论](https://news.ycombinator.com/item?id=49504905)

**背景**: NAT 是作为 IPv4 地址枯竭的临时解决方案而发明的，它允许多个私有设备共享一个公网 IP 地址。它通过重新映射出站连接的端口来对返回流量进行区分，但同时也会阻止未经请求的入站连接，因此自托管服务需要依靠端口转发和 UPnP。IPv6 本意是要恢复端到端连接，但由于惯性、安全理由以及运营商部署 CGNAT 等原因，NAT 仍然被广泛使用。

**社区讨论**: 评论呈现赞同与反驳的混合态度：有人哀叹自托管变得困难以及客户端-服务器思维被正常化，另一些人则认为普通 NAT 没有问题，甚至保护了大量不安全设备。Rusty Russell 的坦白让人相信 NAT 的后果当初并未被充分预见，也引发了关于将现实世界规范错误套用到网络空间的更广泛担忧。

**标签**: `#NAT`, `#Internet`, `#Networking`, `#Centralization`, `#IPv6`

---

<a id="item-3"></a>
## [滑窗注意力在长上下文推理上击败线性注意力](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

一篇新的 arXiv 预印本声称，带有 sink 的滑窗注意力（SWA）在 BABILong 和 Needle-in-a-Haystack 等长上下文推理基准上，性能比线性注意力变体高出 2 到 10 倍，且无需后训练。 这项研究挑战了线性注意力这一重要研究方向，可能影响那些投入大量计算进行后训练以生成线性模型的研究团队。它表明该领域可能一直在用错误的基线进行基准测试，促使社区重新审视比较标准。 SWA 不需要后训练，运行速度快且内存占用低。作者强烈建议改用 SWA 而不是对线性模型进行后训练；线性注意力若要与 SWA 匹配，可能需要从头训练或进行大量后训练。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 8月31日 16:35

**背景**: 标准 Transformer 的自注意力计算量随序列长度呈二次增长，导致长序列处理成本高昂。线性注意力旨在将复杂度降为线性，但常需后训练才能表现良好；滑窗注意力通过只关注局部窗口来降低计算量，而 attention sink 保留早期 token 以稳定生成。BABILong 是一个用“大海捞针”方式测试模型在超长文档中推理能力的基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.28444v1">Sliding - window beats linear attention</a></li>
<li><a href="https://www.alphaxiv.org/abs/2608.28444">Sliding - window beats linear attention | alphaXiv</a></li>
<li><a href="https://arxiv.org/abs/2406.10149">[2406.10149] BABILong: Testing the Limits of LLMs with Long Context Reasoning-in-a-Haystack</a></li>

</ul>
</details>

**标签**: `#Attention`, `#Long-context`, `#LLM`, `#Efficiency`, `#Research`

---

<a id="item-4"></a>
## [新工具 Entropic Scree 可评估脏数据中的信号强度](https://www.reddit.com/r/MachineLearning/comments/1w3br9c/how_to_assess_if_there_is_a_strong_signal_in_your/) ⭐️ 8.0/10

一种名为 Entropic Scree（v1.0.0）的新诊断工具现已以 R 函数形式发布，并附有预印本；它使用变换后的互信息指标而非基于方差的 PCA，来估计高维真实世界数据的信噪比、内在秩和线性充分性。 这一点很重要，因为基于 PCA 的标准方法依赖线性方差假设，而这种假设在杂乱的高维数据上往往失效；Entropic Scree 的互信息方法让从业者在建模之前，能用一种更稳健的方式判断数据中是否存在可学习的信号。 该工具还提供解耦变量子网络的探索性图谱，并可作为“From Garbage to Gold”框架的实用诊断工具，该框架解释何时未整理的数据仍能支持准确预测。目前计划发布 Python 和 R 包，但现阶段仅提供 R 函数 Entropic.Scree.v1.0.0，且该方法尚未经过广泛的社区验证和大规模真实世界基准测试。

reddit · r/MachineLearning · /u/Chocolate_Milk_Son · 8月31日 12:02

**背景**: 主成分分析（PCA）及相关方法通过方差来概括数据，并假设变量之间存在线性关系，因此面对含有错误、缺失值和非线性依赖的“脏”数据时常常会产生误导。互信息衡量的是了解一个变量能在多大程度上告诉你另一个变量的信息，且不假设关系的具体形态；Entropic Scree 利用它估计数据集相对其特殊噪声所含的真实信号量。线性充分性（linear sufficiency）则关注一个线性投影是否能保留估计所需的全部信息，该工具会报告这一点，以说明标准 PCA 的假设是否适用。其预印本所引用的“From Garbage to Gold”框架认为，数据质量应从整体组合层面而非逐条记录层面评估，为直接从不整洁的企业数据中学习提供了理论依据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.12288">[2603.12288] From Garbage to Gold: A Data-Architectural Theory of Predictive Robustness</a></li>
<li><a href="https://arxiv.org/html/2603.12288">From Garbage to Gold: A Data-Architectural Theory of Predictive Robustness</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sufficient_statistic">Sufficient statistic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#data-analysis`, `#mutual-information`, `#dimensionality-reduction`, `#tabular-data`, `#diagnostic-tool`

---

<a id="item-5"></a>
## [Claude 共享链接遭搜索引擎索引，敏感用户数据大量泄露](https://t.me/zaihuapd/43511) ⭐️ 8.0/10

Anthropic 的 Claude 共享对话功能生成的公开链接未设置 noindex 标签，导致 Google 等搜索引擎将其索引。涉及 API 密钥、加密货币钱包、个人简历、律师咨询记录、公司内部项目资料及社会安全号码等敏感内容现可被公开搜索到。 这是一个严重的隐私漏洞，因为任何人都可以通过普通网络搜索发现私人对话，导致凭据与个人数据可能被滥用或出售。所有使用过共享功能的 Claude 用户都受影响，而 Anthropic 反应缓慢使得风险进一步加大，相比之下 ChatGPT 的同类问题当时很快就被修复。 泄露内容涵盖 API 密钥、加密货币钱包、个人简历、律师咨询记录、公司内部资料以及社会安全号码。Anthropic 尚未修复该漏洞，因此建议用户前往设置中的“共享对话”管理页面，手动删除涉及个人隐私或财务的聊天记录。

telegram · zaihuapd · 8月31日 03:22

**背景**: Claude 是 Anthropic 开发的一系列大语言模型和 AI 助手，于 2023 年 3 月以聊天机器人形式发布。noindex 是 HTML 中的一种 robots meta 标签，用于请求 Google 等搜索引擎机器人不要索引某个网页，而公开的共享链接通常需要设置该标签才能避免出现在搜索结果中。API 密钥是用于识别应用或用户、在计算机系统中完成身份验证的一串代码，一旦泄露可能导致未授权访问。大约一年前，ChatGPT 曾出现过类似的共享链接被索引问题，并很快得到修复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/API_key">API key - Wikipedia</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#Claude`, `#Anthropic`, `#vulnerability`

---

<a id="item-6"></a>
## [OpenClaw 2.0 史上最大更新，汇集逾 1.6 万个拉取请求](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

OpenClaw 于 8 月 30 日发布史上最大更新 2.0，汇集了来自 933 名贡献者（含 569 名首次参与者）的逾 1.6 万个拉取请求。此次更新全面改进了安装、消息、记忆、技能、模型、浏览器、插件与安全，并新增了多人协作的共享云端会话。 此次发布大幅扩展了 OpenClaw 的功能，并展现了强大的社区活力，巩固了其在开源 AI 智能体生态系统中的地位。贡献规模约占项目历史全部拉取请求的一半，这可能吸引更多开发者和用户关注并采用智能体式 AI 工具。 为了整合这次更新，团队近七周未发布新版本。新版本简化了安装流程，重建了浏览器端体验，并引入了共享云端会话，支持多人实时协作。

telegram · zaihuapd · 8月31日 04:38

**背景**: OpenClaw 是一款免费开源、运行在用户设备上，并以消息平台为主要界面的自主 AI 智能体。AI 智能体利用大语言模型来追求目标、使用工具并自主完成多步任务。拉取请求是 GitHub 上用于提出、审查和合并代码更改的协作功能，此次逾 1.6 万个贡献正是通过这一机制汇集的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openclaw.ai/">OpenClaw — Open -Source AI Assistant</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://docs.github.com/en/pull-requests/reference/pull-requests">Pull requests - GitHub Docs</a></li>

</ul>
</details>

**标签**: `#OpenClaw`, `#open-source`, `#release`, `#AI agents`, `#developer tools`

---

<a id="item-7"></a>
## [DeepSeek 上线实验性视觉语言模型 deepseek-v4-flash-vision-exp](https://t.me/zaihuapd/43518) ⭐️ 8.0/10

DeepSeek 已发布实验性视觉语言模型 deepseek-v4-flash-vision-exp，并已通过其 API 提供。同一天官方文档和定价也已完成更新。 这标志着 DeepSeek 拓展至多模态 AI 领域，使开发者能够构建同时理解图像和文本的应用。这也增强了 DeepSeek 与 OpenAI GPT-4V、Anthropic Claude 等具备视觉能力的商业模型竞争的地位。 该模型在 Chat Completions、Responses 以及兼容 Anthropic 的 Messages API 中均支持图文混合输入，可通过对图片的 URL、Base64 编码或文件形式提供图像。与 DeepSeek-V4-Flash-0731 相比，它的多模态智能体能力大幅提升，同时保持了相近的纯文本智能体性能。

telegram · zaihuapd · 8月31日 11:41

**背景**: 视觉语言模型（VLM）是一种能够同时解读和生成图像与文本信息的人工智能系统，将大语言模型的能力从纯文本任务扩展到多模态领域。OpenAI、Google、Anthropic 和 Microsoft 等主流厂商已为其旗舰模型加入视觉能力。DeepSeek 此次发布的实验性模型为开发者提供了多模态应用（如图像描述、截图文字识别和图表分析）的开放替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/vision/?ref=upstract.com">Vision | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/ DeepSeek - V 4 - Flash - Vision - Exp · Hugging Face</a></li>
<li><a href="https://chat-deep.ai/docs/deepseek-api-vision-input/">DeepSeek Vision API: Image Input via URL, Base64 & Files</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#API`, `#vision-language model`, `#AI release`, `#LLM`

---

<a id="item-8"></a>
## [小米发布三款玄戒芯片，O3 SoC 将首搭小米 18 Fold](https://t.me/zaihuapd/43524) ⭐️ 8.0/10

小米宣布了三款新的玄戒芯片：AI 旗舰 SoC 玄戒 O3、带宽达 1.22 TB/s 的 AI 加速芯片玄戒 O100，以及国内首款 3nm 智驾 AI 芯片玄戒 D100，三款芯片均完成回片（tape-out）验证。其中 O3 SoC 将首发搭载于小米 18 Fold。 这标志着小米在移动端、AI 加速和汽车三大领域全面发力自研芯片，降低对外部芯片供应商的依赖。O3 号称全球首款支持 LPDDR6 的移动处理器，加上出色的跑分成绩，可能会加剧智能手机 SoC 厂商之间的竞争。 玄戒 O3 采用十核全大核 CPU，据称多核跑分首次突破 15000 分。它还首发 16 核 G2-Ultra NX GPU，官方称相比上一代 O1 性能提升 85%、功耗降低 64%，并支持带宽更高的 LPDDR6 内存。

telegram · zaihuapd · 8月31日 15:15

**背景**: 回片（tape-out）验证指芯片设计已交付晶圆厂流片，并拿到首批物理样片进行测试，以确认设计是否正常。LPDDR6 是 JEDEC 制定的最新低功耗内存标准，旨在为手机等移动设备上的端侧 AI 任务提供更高带宽；小米的合作伙伴长鑫存储（CXMT）近期也宣布 LPDDR6 量产，小米手机有望首发商用 LPDDR6 芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR</a></li>
<li><a href="https://www.tomshardware.com/pc-components/dram/chinas-cxmt-beats-western-chipmakers-to-announcement-of-lpddr6-mass-production-xiaomi-smartphones-to-debut-industrys-first-lpddr6-chips">China's CXMT beats Western chipmakers to... | Tom's Hardware</a></li>
<li><a href="https://gadgets.beebom.com/guides/xiaomi-xring-o3-benchmark-specs">Xiaomi Xring O3: Benchmarks and Specs | Beebom Gadgets</a></li>

</ul>
</details>

**标签**: `#Xiaomi`, `#chip`, `#AI`, `#SoC`, `#hardware`

---