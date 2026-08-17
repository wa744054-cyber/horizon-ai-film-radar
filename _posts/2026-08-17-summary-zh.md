---
layout: default
title: "Horizon Summary: 2026-08-17 (ZH)"
date: 2026-08-17
lang: zh
---

> 从 36 条内容中筛选出 13 条重要资讯。

---

1. [DuckDB v2.0 预览：推出 Quack 协议和扩展仓库](#item-1) ⭐️ 9.0/10
2. [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越远大规模模型](#item-2) ⭐️ 9.0/10
3. [AI 生成的 Copilot Autofix 引入命令注入，Snowflake Jira 遭攻破](#item-3) ⭐️ 8.0/10
4. [GitHub 重大故障引发可靠性、定价与替代方案讨论](#item-4) ⭐️ 8.0/10
5. [Anthropic CEO Dario Amodei：AI 监管是信任危机](#item-5) ⭐️ 8.0/10
6. [AirTag 追踪揭示珍本书被送往亚马逊 AI 训练设施](#item-6) ⭐️ 8.0/10
7. [SemiAnalysis 警告：PJM 的 120 亿美元建模错误可能重演](#item-7) ⭐️ 8.0/10
8. [研究者揭露让稀疏注意力看似有效的常见套路](#item-8) ⭐️ 8.0/10
9. [OpenAI 预览 Ultrafast 模式，GPT-5.6 Sol 提速 14 倍](#item-9) ⭐️ 8.0/10
10. [Stripe 洽购 OpenRouter，估值或达 100 亿美元](#item-10) ⭐️ 8.0/10
11. [ChatGPT 上线 Computer History，记录点击与按键但不截屏](#item-11) ⭐️ 8.0/10
12. [宇树预告“超人”人形机器人：跳高 2 米、时速 12.66 米，超越人类纪录](#item-12) ⭐️ 8.0/10
13. [意大利对苹果开出 1.15 亿美元罚单，指其滥用 App Store 主导权](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DuckDB v2.0 预览：推出 Quack 协议和扩展仓库](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

DuckDB v2.0 预览版引入了 Quack，这是一种远程协议，可让 DuckDB 实例通过 HTTP 互为客户端和服务器，并正式确定了带有签名机制的扩展仓库。预览还突出展示了不到六个月内近 10,000 次提交的快速发展。 DuckDB 是一款广泛使用的进程内 OLAP 数据库；v2.0 的重大进化，尤其是 Quack 使其能够以服务器模式运行，拓宽了其超越嵌入式分析的用例。扩展仓库通过签名机制提升了安全性和社区贡献的便利性，可能加速整个生态系统的发展。 Quack 支持在网络上传输完整的 DuckDB 功能集，并允许多个并发写入者。扩展仓库由名称、URL 前缀和用于签名扩展的 RSA 公钥定义，核心仓库由 DuckDB 团队维护，社区仓库则用于第三方扩展。

hackernews · ibotty · 8月17日 13:46 · [社区讨论](https://news.ycombinator.com/item?id=49330781)

**背景**: DuckDB 是一个开源、列式存储的嵌入式 SQL 数据库，专为大规模数据集上的分析查询而设计。它以其高性能和与 Python、R 等语言的集成而著称。扩展机制允许添加新文件格式和特定领域功能等特性，新的仓库系统通过签名发布确保信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://duckdb.org/quack/">Quack Remote Protocol – DuckDB</a></li>
<li><a href="https://duckdb.org/docs/current/extensions/installing_extensions">Installing Extensions – DuckDB</a></li>
<li><a href="https://en.wikipedia.org/wiki/DuckDB">DuckDB - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者反应热烈，称赞 Quack 和 DuckDB 在降低资源需求方面的影响。一位用户开玩笑询问能否用 minisign 代替 RSA 进行扩展签名，另一位用户则对高提交速度和潜在的 AI 参与表示担忧。还有评论者鼓励大家资助数据库研究。

**标签**: `#DuckDB`, `#database`, `#release`, `#analytics`, `#community`

---

<a id="item-2"></a>
## [Qwen3.8 27B 在 Artificial Analysis 获 52 分，超越远大规模模型](https://artificialanalysis.ai/models/qwen3-8-27b) ⭐️ 9.0/10

阿里巴巴 Qwen 系列的小型开源模型 Qwen3.8 27B 在 Artificial Analysis 基准测试中取得 52 分。这一成绩超过了 Opus 4.6 等规模大得多的模型，并与 DeepSeek V4 Flash 持平。 这一结果意义重大，因为一个可在消费级游戏 PC 上运行的 27B 参数模型，如今能与动用海量算力和数据中心级资源的顶尖模型匹敌甚至胜出。它挑战了“必须靠规模才能实现顶尖能力”的假设，也证明了高效、可在本地运行的开源 AI 的价值。 根据社区对比，Qwen3.6 27B 此前得分为 38，而 Qwen3.8 27B 的 52 分与 DeepSeek V4 Flash 0731 持平，后者在大型模型类别（超过 1500 亿参数）中排名第五。它在 Artificial Analysis 上还据称超越了所有中等规模（400 亿至 1500 亿参数）模型。

hackernews · anana_ · 8月17日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=49334544)

**背景**: Artificial Analysis 是一个独立的 AI 模型与 API 服务商评测平台，从质量、价格、输出速度和延迟等维度对模型进行比较。Qwen 系列由阿里云达摩院开发，是一族采用 Apache 2.0 许可的开源权重语言模型，覆盖从小型稠密模型到大型混合专家模型的多种规模。Artificial Analysis 上的 52 分是该平台综合评估模型智能与能力的量化结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://huggingface.co/Qwen">Org profile for Qwen on Hugging Face, the AI community building the...</a></li>
<li><a href="https://qwen.moe/">Qwen — Open Foundation Models</a></li>

</ul>
</details>

**社区讨论**: 社区反应既兴奋又难以置信：有评论者指出，一个 27B 模型击败 Opus 4.6“既好笑又有点可怕”，而且它在游戏硬件上就能顺畅运行。多位用户分享了实际体验，称该模型智能、古怪且具有很强的智能体特性，会执着地以不寻常方式解决问题；也有用户表示将进行大量测试，以在真实编程工作流中验证这一基准成绩。

**标签**: `#Qwen`, `#AI benchmarks`, `#small language models`, `#open-source AI`, `#model efficiency`

---

<a id="item-3"></a>
## [AI 生成的 Copilot Autofix 引入命令注入，Snowflake Jira 遭攻破](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

GitHub Copilot Autofix 的一条建议在 Snowflake 的 GitHub Actions 工作流中引入了命令注入漏洞，该漏洞被利用以攻破 Snowflake 的 Jira 实例。这一事件展示了 AI 生成的代码修复在安全关键场景中的真实失败案例。 该事件凸显了 AI 辅助编程的安全风险，自动化修复可能无意中引入新漏洞。它强调了在 CI/CD 流水线等通常处理敏感基础设施的场景中，对 AI 生成代码进行严格审查和静态分析的必要性。 该漏洞是 GitHub Actions 工作流（jira_issue.yml）中的模板注入，允许通过未转义的 title 和 body 变量执行任意命令。zizmor 静态分析扫描标记了该问题，错误为“template-injection: code injection via template expansion”，位于工作流第 24 行。

hackernews · galnagli · 8月17日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=49331423)

**背景**: GitHub Copilot Autofix 是一项自动为代码扫描警报建议修复的功能，旨在加快漏洞修复速度。命令注入发生在不安全用户输入被传递给 shell 时，允许攻击者执行任意命令。在 GitHub Actions 工作流中，模板表达式如 ${{ }} 会在运行器中被求值，如果在 run 命令中使用而未经正确转义，可能导致代码注入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/code-security/responsible-use/responsible-use-autofix-code-scanning">Responsible use of Copilot Autofix for code scanning - GitHub Docs</a></li>
<li><a href="https://portswigger.net/web-security/os-command-injection">What is OS command injection, and how to prevent it? | Web Security Academy</a></li>

</ul>
</details>

**社区讨论**: 评论者认为，在没有静态分析的情况下编写 GitHub Actions 是疏忽的，并建议在 CI 中使用 zizmor 来捕获模板注入问题。有用户观察到，AI 降低了生成变更的成本，但没有降低审查成本，瓶颈正在向验证转移。另一位用户质疑有漏洞的变更是否真的是 Copilot 生成的，指出链接的 PR 中 Copilot 提交与漏洞无关。

**标签**: `#AI code generation`, `#security`, `#GitHub Actions`, `#supply chain`, `#Copilot`

---

<a id="item-4"></a>
## [GitHub 重大故障引发可靠性、定价与替代方案讨论](https://www.githubstatus.com/incidents/zkxwbgr0cnmx) ⭐️ 8.0/10

GitHub 发生重大服务故障（事件编号 zkxwbgr0cnmx），用户在 githubstatus.com 上看到“当前没有服务器可处理您的请求”的错误，网页 diff 等核心功能无法使用。故障持续数小时，状态更新显示 API 请求、Actions、Git 操作、Issues、Pages、Pull Requests 和 Webhooks 均出现性能下降。 GitHub 是开源和企业软件开发的关键平台，因此这次故障打乱了无数开发者的工作流以及 CI/CD 流水线。大量社区讨论也反映出人们对 GitHub 的可靠性、定价和对微软的依赖越来越担忧，部分用户正在认真考虑替代方案。 该事件最初由用户报告，之后官方状态页才更新；故障发生近三小时后，页面仍显示“我们仍在努力确定根本原因”。部分服务曾短暂恢复，但 Git 操作随后再次出现性能下降，说明恢复过程并不顺利。

hackernews · SpyCoder77 · 8月17日 13:35 · [社区讨论](https://news.ycombinator.com/item?id=49330597)

**背景**: 状态页是一个公开的仪表板，用于实时显示服务的各个组件（如 API、数据库和 Web 界面）的运行状态，帮助组织向用户传达故障和维护信息。服务事件是指导致或可能导致服务降级或中断的异常情况，需要人工干预才能恢复正常运行。GitHub 的官方状态页 githubstatus.com 是向用户报告此类事件的正式渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://statusbot.flaredesk.com/status-page/">Status Page – StatusBot by Flaredesk</a></li>
<li><a href="https://okchecker.com/blog/what-is-status-page">What Is a Status Page and Why You Need One | OKchecker</a></li>
<li><a href="https://handbook.gitlab.com/handbook/engineering/infrastructure-platforms/incident-management/">Incident Management | The GitLab Handbook</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了强烈不满，有人称这次故障是一个“转折点”，还有人表示要转向更便宜、更容易迁移的托管方案。围绕 GitHub 是否应对非付费用户限流或对 LLM 生成流量消耗的资源收费展开了争论，也有不少人批评微软对平台的经营管理。

**标签**: `#github`, `#incident`, `#outage`, `#reliability`, `#devops`

---

<a id="item-5"></a>
## [Anthropic CEO Dario Amodei：AI 监管是信任危机](https://twitter.com/DarioAmodei/status/2088758816376807762) ⭐️ 8.0/10

Anthropic CEO Dario Amodei 发表声明，认为 AI 监管本质上是一场信任危机，并称普通人不信任企业、政府和科技行业。他拒绝了带有正面包装的华丽营销活动，转而承诺 Anthropic 在生物学和医学领域的真实成果将在实现后以尽可能大的声音公之于众。 这塑造了一家领先 AI 实验室如何构建 AI 监管公共政策辩论的框架，凸显了前沿 AI 公司与公众之间日益扩大的信誉差距。社区反应不一——从真诚信任到指责其居高临下的修辞——表明公众认知如何影响 AI 治理讨论。 Amodei 特别指出，带有正面包装的营销活动无法赢回信任，并称“AI 将治愈癌症”已成为一种陈词滥调，多数人认为它具有欺骗性。他声称 Anthropic 正在迅速加大在生物学和医学领域的投入，预计未来几个月会出现“早期曙光”，未来几年会取得“惊人成果”。

hackernews · jacquesm · 8月17日 01:59 · [社区讨论](https://news.ycombinator.com/item?id=49325789)

**背景**: 随着 Anthropic、OpenAI 和 Google 等前沿模型快速发展，AI 监管成为一个重大政策议题。信任在这场辩论中至关重要，因为公众和监管机构担心权力集中、安全性，以及 AI 公司是否真正为公共利益而非自身利益行事。Amodei 的评论是对更广泛批评的回应，即 Anthropic 的安全言辞与其行为并不总是一致，包括关于开放权重和封闭开发的争论。

**社区讨论**: 社区反应出现分歧：一些评论者（如 mhaberl）对 Amodei 的意图表示真诚信任，而另一些人（如 mindwok）则认为 Anthropic 存在严重的公关问题，使用居高临下的“奥威尔式”修辞，让公众感到不被信任。另一位评论者 pu_pe 补充说，由于扩展定律（scaling laws），AI 在结构上倾向于集中权力，开放权重只能部分解决这一问题，只是将权力集中转移到掌控算力和芯片的实体手中。

**标签**: `#AI regulation`, `#Anthropic`, `#trust`, `#AI policy`, `#community discussion`

---

<a id="item-6"></a>
## [AirTag 追踪揭示珍本书被送往亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

调查媒体 404 Media 在订单中一本珍本书里藏入苹果 AirTag。追踪发现包裹被送到拉斯维加斯亚马逊 LAS8 设施的 VGT3 区域，证实亚马逊正在为 AI 训练大规模破坏性扫描书籍。 这是首例直接追踪证据，将大宗珍本购买与亚马逊 AI 训练业务联系起来，加剧了人们对 AI 公司未经授权获取训练数据的担忧。该发现使 AI 训练数据来源的版权与合理使用争议更加尖锐。 该订单通过 Biblio 图书市场下单，AirTag 最终到达 VGT3，亚马逊员工在论坛讨论中称该地点用于破坏性书籍扫描。设施入口还贴有恐龙抱书的标志，疑似在暗示这项扫描业务。

rss · Simon Willison · 8月17日 15:21

**背景**: AI 公司一直被怀疑从二手图书市场大量购买实体书，扫描后制成训练语料库，再将实体书丢弃或销毁。2025 年针对 Anthropic 的诉讼揭示了其秘密项目“Project Panama”，涉及扫描数百万本书，法官 Alsup 关于破坏性扫描的合理使用裁定正在影响行业做法。Biblio 是稀有书和古旧书的主要交易平台，正是这类批量且对价格不敏感的订单经常出现的地方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-training-facility/">We Tracked a Shipment of Rare Books . It Ended at an Amazon AI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Biblio.com">Biblio.com - Wikipedia</a></li>
<li><a href="https://www.ibtimes.co.uk/anthropic-secret-book-scanning-operation-1811155">Inside Project Panama, Anthropic's Secret Effort To Scan ... | IBTimes UK</a></li>

</ul>
</details>

**标签**: `#AI training`, `#data sourcing`, `#copyright`, `#Amazon`, `#investigation`

---

<a id="item-7"></a>
## [SemiAnalysis 警告：PJM 的 120 亿美元建模错误可能重演](https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted) ⭐️ 8.0/10

SemiAnalysis 发布分析报告，指出 PJM 电网规划中的建模错误浪费了美国电力用户 120 亿美元，并警告 PJM 的结构性反增长容量市场与治理体系可能导致同样昂贵的错误重演。 这一发现凸显了美国电力市场中电网建模假设所涉及的巨大财务风险。PJM 的容量市场设计直接影响可靠性投资与数十亿美元的消费者开支，若重蹈覆辙，将进一步加重电力用户的负担。 该分析批评 PJM 的模型在结构上反增长，其容量市场设计在全球独一无二但存在缺陷，治理体系也过于庞大而难以有效运作。报告还通过实时重建相关备用容量计算来揭示该错误。

rss · Semianalysis · 8月16日 22:27

**背景**: PJM 互联运营着覆盖美国东部大片地区的批发电力和容量市场，容量市场会提前数年向发电商付费，以确保未来用电需求得到满足。容量拍卖结果（例如 2024 年 7 月拍卖在 PJM 大部分地区以 269.92 美元/兆瓦-日成交）直接影响用户电费。当规划模型错误预测备用裕度或需求时，市场可能购买超出需要的容量，造成电力用户资金浪费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted">Full of Cold Air - PJM's $12B modeling mistake</a></li>
<li><a href="https://www.congress.gov/crs-product/R48553">PJM’s Electric Capacity Market: Background and Current Issues | Congress.gov | Library of Congress</a></li>
<li><a href="https://www.pjm.com/markets-and-operations/rpm.aspx">PJM - Capacity Market (RPM)</a></li>

</ul>
</details>

**标签**: `#grid modeling`, `#energy policy`, `#PJM`, `#infrastructure`, `#cost analysis`

---

<a id="item-8"></a>
## [研究者揭露让稀疏注意力看似有效的常见套路](https://www.reddit.com/r/MachineLearning/comments/1vqqqcs/how_to_make_any_sparse_attention_kv_compression/) ⭐️ 8.0/10

一位专注于 KV 缓存压缩的研究者在 Twitter 上发帖（并被分享到 r/MachineLearning），详细列举了让稀疏注意力和 KV 压缩方法看起来效果出众的常见套路与基准设置。帖子特别批评了使用误导性的单跳检索任务、挑选有利的基线方法、以及用汇总指标掩盖失败等做法。 该批评之所以重要，是因为评测方式直接影响哪些方法被视为最先进并被采用。通过揭露常见陷阱，它促使机器学习社区在稀疏注意力和 KV 压缩研究中要求更公平的基准和更严谨的对比。 帖子列出了四个主要套路：选择没有干扰物的单跳检索任务；从不单独隔离方法本身的贡献（例如使用与基线不同的窗口或块大小）；仅依赖汇总指标来掩盖弱点（以 RULER 的 13 个任务为例）；以及挑选所有模型得分都相近的饱和基准。作者承认自己也犯过其中一些做法，并正在努力改进。

reddit · r/MachineLearning · /u/korec1234 · 8月17日 12:18

**背景**: KV 缓存是 Transformer 模型中的一种机制，用于存储先前计算出的键和值向量以加速自回归推理，但它会随序列长度增长，造成内存和带宽瓶颈。稀疏注意力方法通过限制每个 token 关注哪些键值对来降低这些成本，但其效果高度依赖评测设计。'大海捞针'（NIAH）测试是一种常见的长期上下文检索基准，将一条相关信息放置在无关上下文中，但如果上下文中没有干扰或不相关信息，就容易被人为操纵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/docs/transformers/kv_cache">Cache strategies · Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/sparse-attention">Sparse Attention Mechanisms - emergentmind.com</a></li>
<li><a href="https://arxiv.org/abs/2407.01437">[2407.01437] Needle in the Haystack for Memory Based Large Language Models</a></li>

</ul>
</details>

**标签**: `#KV Cache`, `#Sparse Attention`, `#Model Evaluation`, `#Efficient Transformers`, `#Research Critique`

---

<a id="item-9"></a>
## [OpenAI 预览 Ultrafast 模式，GPT-5.6 Sol 提速 14 倍](https://t.me/zaihuapd/43228) ⭐️ 8.0/10

OpenAI 预览了 Ultrafast 这一新的 API 服务层级，其运行 GPT-5.6 Sol 的速度最高可达标准处理的 14 倍。该服务由 Cerebras 驱动，每秒最多生成 750 个 token，目前仅向少数客户限量开放。 这一进展意义重大，因为亚秒级响应有望让 OpenAI 最强大的模型在故障响应、金融研究、客服和电商等对时间敏感的场景中变得切实可用。这也表明 OpenAI 愿意借助专用硬件合作伙伴来提升推理性能。 Ultrafast 运行在 Cerebras 的晶圆级引擎硬件上，OpenAI 与 Cerebras 均表示该模式在不降低模型质量的前提下实现提速。此预览受算力限制，OpenAI 表示将随着算力扩充逐步扩大访问范围。

telegram · zaihuapd · 8月17日 00:47

**背景**: Cerebras Systems 设计晶圆级处理器并提供 AI 推理/训练云服务，它将整片硅晶圆用作单个芯片，相比 GPU 集群可降低延迟。GPT-5.6 是 OpenAI 于 2026 年 7 月发布的大语言模型系列，包含 Luna、Terra 和 Sol 三个变体，其中 Sol 能力最强。Ultrafast 通过 OpenAI API 将 Cerebras 的低延迟推理栈应用于 Sol。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>
<li><a href="https://techcrunch.com/2026/08/13/openai-introduces-ultrafast-a-new-mode-that-makes-gpt-5-6-sol-work-at-14x-the-speed/">OpenAI introduces 'Ultrafast,' a new mode that makes GPT-5.6 Sol work at 14x the speed | TechCrunch</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#performance`, `#API`, `#Cerebras`

---

<a id="item-10"></a>
## [Stripe 洽购 OpenRouter，估值或达 100 亿美元](https://t.me/zaihuapd/43229) ⭐️ 8.0/10

《华尔街日报》24 日援引知情人士称，Stripe 正就收购 AI 模型路由初创公司 OpenRouter 进行谈判，交易估值约 100 亿美元。双方可能达成协议，但交易尚未最终确认。 这笔约 100 亿美元的潜在收购表明，AI 基础设施正成为核心金融科技公司的战略布局重点。若交易完成，Stripe 可能将模型路由和 AI 接入能力嵌入其支付与商业生态，影响众多使用 AI 功能的开发者和企业。 谈判仍在进行中，尚未确认最终协议，估值和条款可能有变。OpenRouter 提供统一 API，让开发者能通过一次接入使用数百个 AI 模型（有指南称超过 500 个），这正是 Stripe 看重的核心资产。

telegram · zaihuapd · 8月17日 01:19

**背景**: AI 模型路由是一种技术，能将每个传入请求分发给最合适的 AI 模型，而不是为所有任务固定使用同一个模型。OpenRouter 是一个聚合众多大语言模型的网关，通过统一 API 简化开发者的接入流程。Stripe 是重要的在线支付公司，近年来一直在加强 AI 和开发者工具方面的布局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://inworld.ai/resources/what-is-an-ai-router">What Is an AI Router? LLM Model Routing Explained (2026)</a></li>
<li><a href="https://evolink.ai/blog/what-is-ai-model-routing-guide-for-developers">What Is AI Model Routing? A Practical Guide for Developers | EvoLink</a></li>
<li><a href="https://openrouter.ai/docs/quickstart">OpenRouter Quickstart Guide</a></li>

</ul>
</details>

**标签**: `#Stripe`, `#OpenRouter`, `#AI`, `#acquisition`, `#fintech`

---

<a id="item-11"></a>
## [ChatGPT 上线 Computer History，记录点击与按键但不截屏](https://www.theverge.com/ai-artificial-intelligence/980742/chatgpts-computer-history-tracks-your-clicks-and-keystrokes) ⭐️ 8.0/10

OpenAI 在 ChatGPT macOS 桌面应用中推出了 Computer History 功能，这是一项可选功能，会记录点击和按键，以构建用于训练和自动化的活动时间线。该功能取代了此前的 Chronicle 研究预览版，目前正在向部分账户类型推送。 这标志着 AI 助手向观察并自动化真实电脑操作又迈进了一步，但同时也引发了显著的隐私担忧。该功能与 Windows Recall 类似，但避免了截屏，可能为桌面 AI 代理如何处理敏感用户数据树立新的先例。 Computer History 默认需要手动开启，允许用户排除特定应用和网站、删除记录，并会忽略无痕或隐私浏览标签页。OpenAI 表示它不截取图像、视频或音频，只记录点击和按键等“事件”。

telegram · zaihuapd · 8月17日 04:16

**背景**: ChatGPT macOS 应用是 OpenAI 模型的聊天客户端，如今还与 AI 编程代理 Codex 集成。Computer History 会创建应用和网站活动的可搜索时间线，供 ChatGPT 和 Codex 学习工作方式、建议自动化。该功能让人联想到 Windows 11 的 Windows Recall，后者通过截屏记录用户活动，并因隐私问题遭到大量争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.chatgpt.com/docs/customization/computer-history">Computer History | ChatGPT Learn</a></li>
<li><a href="https://www.zdnet.com/article/chatgpt-computer-history/">ChatGPT's new Computer History tracks your Mac activity to create a timeline - but should you let it? | ZDNET</a></li>
<li><a href="https://en.wikipedia.org/wiki/Windows_Recall">Windows Recall</a></li>

</ul>
</details>

**标签**: `#ChatGPT`, `#OpenAI`, `#privacy`, `#AI assistant`, `#macOS`

---

<a id="item-12"></a>
## [宇树预告“超人”人形机器人：跳高 2 米、时速 12.66 米，超越人类纪录](https://m.weibo.cn/detail/5332901463070926) ⭐️ 8.0/10

宇树科技周一发布了全新人形机器人“超人”的预告，宣称其原地跳高可达 2 米，极限速度达每秒 12.66 米。官方表示，全新整机仅用 3 个多月研发完成，未来几个月还有较大完善空间。 这一消息意义重大，因为“超人”据称在原地跳高和奔跑速度两方面都超越了人类纪录，成为人形机器人领域的一个里程碑。发布几天后，宇树将成为中国大陆首家上市的通用人形机器人公司，凸显了该行业的商业化势头。 该机器人腿长 0.85 米，极限速度达 12.66 米/秒，超过了尤塞恩·博尔特曾跑出的最快速度。由于目前只是预告，公开的技术细节有限，宇树表示未来几个月仍有较大完善空间。

telegram · zaihuapd · 8月17日 07:12

**背景**: 宇树科技 2016 年成立于杭州，最初专注于消费级四足机器人，后来扩展到人形机器人领域。人形机器人要实现高速双足奔跑和跳跃，需要先进的运动控制、高速传感器和基于 AI 的规划，这些领域近年来进展迅速。宇树即将在中国大陆上市，反映出投资者对机器人和 AI 领域日益浓厚的兴趣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/unitree-robot-hits-12-66-094529616.html">Unitree’s New Robot Hits 12.66 m/s — Faster Than Usain Bolt Ever Ran</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/chinese-humanoid-robot-maker-unitree-123559978.html">China's Unitree unveils 'Superman' robot as fervour builds ahead of Shanghai debut</a></li>

</ul>
</details>

**标签**: `#robotics`, `#humanoid`, `#Unitree`, `#AI`, `#engineering`

---

<a id="item-13"></a>
## [意大利对苹果开出 1.15 亿美元罚单，指其滥用 App Store 主导权](https://t.me/zaihuapd/43243) ⭐️ 8.0/10

意大利反垄断机构 AGCM 对苹果处以 1.15 亿美元罚款，理由是通过应用跟踪透明度（ATT）政策滥用其在 App Store 的主导地位。监管机构认定苹果单方面对第三方开发者施加 ATT 要求，却让自家应用免于显示同样的权限弹窗。 这项裁决可能为 ATT 这类以隐私为核心的政策如何受到竞争公平性审查开创先例。它可能促使苹果统一其针对第三方和自家应用的数据跟踪规则，从而影响欧盟及其他地区开发者的广告收入和用户数据访问。 AGCM 表示，ATT 的条款是单方面强加的，与苹果宣称的隐私目标不成比例，损害了开发者的商业利益。罚款总额约为 1 亿欧元，苹果回应称强烈反对该决定，认为监管机构忽视了 ATT 为用户带来的隐私保护益处。

telegram · zaihuapd · 8月17日 12:50

**背景**: 应用跟踪透明度（ATT）是 iOS 14.5 中引入的一项隐私功能，要求应用在跨其他公司的应用和网站追踪用户活动前，必须获得用户许可。苹果要求所有通过 App Store 分发的第三方应用遵守此规则，但其自身应用却无需显示相同的弹窗。这种不对称做法遭到开发者和监管机构的批评，认为苹果利用其 App Store 主导地位施加不公平条件。意大利此次行动是全球范围内对苹果 App Store 行为进行更广泛审查的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/apptrackingtransparency">App Tracking Transparency | Apple Developer Documentation</a></li>
<li><a href="https://support.apple.com/en-us/102420">If an app asks to track your activity - Apple Support</a></li>
<li><a href="https://medium.com/design-bootcamp/prompt-apples-app-tracking-transparency-policy-att-31a8a482b5b1">App Tracking Transparency (ATT): Apple’s Privacy ... - Medium</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Apple`, `#App Store`, `#privacy`, `#regulation`

---