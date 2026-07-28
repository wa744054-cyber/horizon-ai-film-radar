---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 29 条内容中筛选出 7 条重要资讯。

---

1. [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞，影响 JDK 8/17/21](#item-1) ⭐️ 9.0/10
2. [Anthropic CEO 反对开源权重模型，支持对华芯片禁令](#item-2) ⭐️ 8.0/10
3. [缺少下划线导致无辜者入狱 18 个月](#item-3) ⭐️ 8.0/10
4. [Moonshot AI 发布 2.8 万亿参数 Kimi-K3 权重](#item-4) ⭐️ 8.0/10
5. [DP-FedSOFIM：无需额外代价的二阶差分隐私联邦学习](#item-5) ⭐️ 8.0/10
6. [对 6 个前沿 LLM 的独立评测显示左倾偏差](#item-6) ⭐️ 8.0/10
7. [中芯国际测试国产首台 DUV 光刻机](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞，影响 JDK 8/17/21](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

安全研究人员 Kirill Firsov 披露，Fastjson 1.2.68 至 1.2.83 版本存在高危远程代码执行漏洞，无需 gadget 链也无需开启 autoType，影响 JDK 8、17 和 21。由于 Fastjson 1.x 已于 2024 年 10 月停止维护，官方不会发布补丁。 该漏洞极其严重，因为无需启用 autoType 或依赖 classpath gadget 等常见条件即可实现未认证远程代码执行，利用门槛极低。考虑到 Fastjson 在 Java 应用（尤其是阿里巴巴生态及企业环境）中广泛使用，此漏洞带来严峻安全风险，且官方无补丁可用。 该漏洞影响 Fastjson 1.2.68–1.2.83，利用了默认 SafeMode 未开启的状态；已确认的攻击向量需要 Spring Boot 可执行 fat-JAR 以及可被攻击者控制的 JSON 输入路径。唯一有效的补救措施是升级到 Fastjson 2，或开启 SafeMode 并限制反序列化来源。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson 是阿里巴巴开发的 Java 流行 JSON 序列化/反序列化库。autoType 功能允许在 JSON 中嵌入类型信息以实现多态反序列化，但历史上一直是常见攻击面。Gadget 链是一系列存在于 classpath 中的类，反序列化时能执行任意代码；以往许多 Fastjson 漏洞需要依赖此类 gadget。此新漏洞绕过了 autoType 和 gadget 要求，因而极其危险。SafeMode 自 1.2.68 引入，可完全禁用 autoType，但默认未开启。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched...</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson_safemode_en · alibaba/fastjson Wiki</a></li>
<li><a href="https://github.com/frohoff/ysoserial">GitHub - frohoff/ysoserial: A proof-of-concept tool for ... Java Deserialization Attacks: From Gadget Chains to RCE Java deserialization tricks - Synacktiv Lab: Developing a custom gadget chain for Java deserialization Rev Gadget: A Java Deserialization Gadget Chains Discover ... GrrrDog/Java-Deserialization-Cheat-Sheet - GitHub</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Fastjson`, `#RCE`, `#Java`

---

<a id="item-2"></a>
## [Anthropic CEO 反对开源权重模型，支持对华芯片禁令](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic CEO Dario Amodei 发表博文，声明公司因安全风险反对开源权重 AI 模型，并支持美国对中国实施芯片出口禁令。 一家领先 AI 公司的这一立场加剧了关于开源与封闭 AI 开发的辩论，可能影响政策和行业规范。 Amodei 特别主张禁止向中国销售芯片并打击走私，同时承认禁令本身并非万能药。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开源权重模型公开训练好的神经网络参数，允许修改和再分发。与完全开源模型不同，它们通常缺乏完全复现模型所需的训练数据和代码。这一区别是 AI 领域关于安全性、可访问性和竞争辩论的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://infercom.ai/glossary/open-weights-model/">What is an Open - Weight Model ? Definition | Infercom</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>

</ul>
</details>

**社区讨论**: 评论者大多批评 Amodei 的立场是自私且自相矛盾的，有人指责他在进行道德表演。其他人质疑他支持禁令却又声称其无效的逻辑。

**标签**: `#AI safety`, `#open-source models`, `#Anthropic`, `#AI policy`, `#China`

---

<a id="item-3"></a>
## [缺少下划线导致无辜者入狱 18 个月](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

因警方传票中缺少一个下划线，Kik 的系统返回了错误用户的数据，导致一名无辜的加拿大男子被错误定罪并监禁 18 个月，罪名涉及儿童剥削。 此案表明，法律程序中的微小技术疏忽可能造成毁灭性的人道后果，凸显了执法部门亟需提高技术素养，并在处理数字证据时采用更严格的验证方法。 传票要求提供 Kik 用户“fus_ro_dah”（一个下划线）的信息，但由于 SQL 通配符解释，它匹配了另一个用户“fus__ro_dah”（两个下划线）——在 SQL LIKE 查询中，下划线字符充当单字符通配符，因此“fus_ro_dah”匹配了任何以“fus”开头、后跟任意一个字符然后“ro_dah”的字符串。

hackernews · quantified · 7月27日 22:10 · [社区讨论](https://news.ycombinator.com/item?id=49076116)

**背景**: 在 SQL 数据库中，下划线（_）是与 LIKE 运算符一起使用时匹配任意单个字符的通配符。如果搜索模式中包含下划线而未正确转义，数据库会将其解释为通配符而非字面下划线。警方发给 Kik 的传票忽视了这一技术细节，导致识别了错误的账户。受害者在美国，被告在加拿大，跨国调查增加了复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.w3resource.com/sql/wildcards-like-operator/wildcards-underscore.php">SQL wildcards underscore ( _ ) - w3resource</a></li>
<li><a href="https://learn.microsoft.com/en-us/sql/t-sql/language-elements/wildcard-match-one-character-transact-sql?view=sql-server-ver17">_ (Wildcard - Match One Character) (Transact-SQL) - SQL Server | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 评论者对错误定罪表示愤慨，质疑辩护律师为何未能质疑存在缺陷的数字证据。许多人指出，仅撤销定罪是不够的，还需赔偿，因为声誉损害是终身的。一些人还指出了美加之间的司法管辖权问题，这可能妨碍了公正审判。

**标签**: `#wrongful conviction`, `#legal tech`, `#data accuracy`, `#criminal justice`, `#technology failure`

---

<a id="item-4"></a>
## [Moonshot AI 发布 2.8 万亿参数 Kimi-K3 权重](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI 在 Hugging Face 上发布了其 2.8 万亿参数的 Kimi-K3 模型权重，采用自定义许可证，要求大型商业实体在提供模型即服务（MaaS）时需另行签订协议。 此次发布延续了超大规模开放权重模型的趋势，但其非标准许可证——要求高收入公司进行署名，并为 MaaS 提供商设置单独协议——引发了关于 AI 中开源与开放权重界限的讨论。 Kimi-K3 模型权重大小为 1.56 TB，其许可证不再自称修改版 MIT，明确要求连续 12 个月内总收入超过 2000 万美元的 MaaS 提供商必须签订单独协议。

rss · Simon Willison · 7月27日 23:39

**背景**: Moonshot AI 此前发布 Kimi-K2 时采用修改版 MIT 许可证，增加了对月活超 1 亿或月收入超 2000 万美元的商业实体的署名要求。K3 许可证更进一步，针对 MaaS 业务，并且不再自称修改版 MIT。开放权重模型允许访问模型参数，但往往施加超越传统开源定义的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-K3/blob/main/LICENSE">Kimi-K3/LICENSE at main · MoonshotAI/Kimi-K3 · GitHub</a></li>
<li><a href="https://kingy.ai/ai/ai-guides/kimi-k3-license-commercial-use-open-source/">Kimi K3 License: Commercial Use Is Allowed—with Conditions</a></li>

</ul>
</details>

**标签**: `#AI`, `#Large Language Models`, `#Open Source`, `#Moonshot`, `#Kimi-K3`

---

<a id="item-5"></a>
## [DP-FedSOFIM：无需额外代价的二阶差分隐私联邦学习](https://www.reddit.com/r/MachineLearning/comments/1v8pkb7/dpfedsofim_secondorder_federated_optimization/) ⭐️ 8.0/10

DP-FedSOFIM 提出了一种二阶联邦优化方法，通过将曲率估计完全移至服务器端，在不增加隐私成本或 O(d²) 通信开销的情况下实现差分隐私。 这项工作解决了差分隐私联邦学习中的一个关键限制——之前的二阶方法需要在客户端计算和传输完整矩阵，开销大且难以扩展。DP-FedSOFIM 表明，可以从已私有化的聚合中提取有用的曲率信息，从而在严格的隐私预算下实现更快的收敛。 服务器维护私有化梯度聚合的指数移动平均（EMA），并将其正则化的秩一外积作为 Fisher 代理，利用 Sherman-Morrison 公式高效预条件而不显式构建矩阵。实验表明，在 CIFAR-10/ResNet 上 epsilon=5 时，第 10 轮的准确率比 DP-FedGD 高出最多 20.3 个百分点，且每轮时间开销不到 2%。

reddit · r/MachineLearning · /u/worthybog0 · 7月28日 06:04

**背景**: 联邦学习（FL）通过分散数据训练共享模型而不集中数据，但模型更新可能泄露隐私。差分隐私（DP）通过裁剪和添加噪声来缓解此问题，但噪声注入会降低收敛速度，尤其在严格的隐私预算下。标准的 DP-FL 方法使用一阶优化，而二阶方法可以改善收敛，但通常需要客户端计算并传输完整的协方差矩阵（O(d²) 成本），从而引入新的隐私敏感度和通信瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2601.09166v1">DP-FedSOFIM: Differentially Private Federated Stochastic ...</a></li>
<li><a href="https://arxiv.org/html/2505.23588v1">Accelerated Training of Federated Learning via Second-Order ...</a></li>

</ul>
</details>

**标签**: `#Federated Learning`, `#Differential Privacy`, `#Second-Order Optimization`, `#Privacy-Preserving Machine Learning`

---

<a id="item-6"></a>
## [对 6 个前沿 LLM 的独立评测显示左倾偏差](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

一项对六个前沿大语言模型（GPT-5.4、Claude Sonnet 4.6、Claude Opus 4.7、Gemini Pro、Gemini Flash 和 Grok 4.3）的独立评测，使用约 20,600 个样本覆盖 8 个偏见基准，发现所有模型（包括自称为右倾的 Grok）均表现出左倾政治偏见。此外，涉及种族问题的拒答率差异显著，GPT-5.4 的拒答率高达 20.3%。 该研究提供了经验证据，表明即使是为了避免偏见或具有明确政治倾向的模型，也可能表现出系统性的左倾行为，这对 AI 应用的公平性具有重要影响。它凸显了持续进行偏见审计和模型行为透明度的必要性。 评测使用了八个既定数据集：WinoBias、BBQ Race/Ethnicity、SeeGULL、OpinionsQA、cajcodes Political Bias、Hyperpartisan News 和 Political Compass。一个明显的局限是，这是一个个人完成的非同行评审项目，采用了单一提示模板且未进行多次运行平均。

reddit · r/MachineLearning · /u/marggggggggg · 7月27日 22:37

**背景**: WinoBias 和 BBQ 等偏见基准用于评估大语言模型在指代消解和问答任务中的刻板关联。WinoBias 使用维诺格拉德模式句子衡量职业性别偏见，而 BBQ（QA 偏见基准）评估包括种族和性别在内的社会类别偏见。这些基准被广泛用于检测模型的意外偏见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winobias">WinoBias : Gender Bias in Coreference Benchmark</a></li>
<li><a href="https://deepeval.com/docs/benchmarks-bbq">BBQ | DeepEval - The LLM Evaluation Framework</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>

</ul>
</details>

**标签**: `#AI bias`, `#LLM evaluation`, `#political bias`, `#model behavior`, `#fairness benchmarks`

---

<a id="item-7"></a>
## [中芯国际测试国产首台 DUV 光刻机](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

中芯国际正在试运行中国首台由上海初创公司宇量昇自主研发的深紫外（DUV）光刻机，用于生产 28 纳米芯片，并可能通过多重图形化工艺实现 7 纳米甚至 5 纳米制程。 这一进展是中国实现半导体自给自足、减少对 ASML 依赖的关键一步，尤其是在美国对先进设备实施出口限制的背景下。若成功，可能重塑全球芯片制造供应链。 该 DUV 光刻机大部分零部件已实现国产化，但仍有部分依赖进口。业内人士估计，实现量产和稳定良率至少需要一至两年，最快可能于 2027 年进入量产。

telegram · zaihuapd · 7月27日 14:10

**背景**: DUV 光刻使用 193 纳米波长的光，而 EUV 使用 13.5 纳米，分辨率更高。中国目前最先进的芯片依赖 ASML 的 DUV 设备，但 EUV 对华销售被禁。多重图形化技术（如 SADP）使得 DUV 能够制造出比其光学极限更小的特征，从而实现 7 纳米和 5 纳米节点，但良率较低且成本更高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1960307062815855033">半导体先进工艺：多重图形化技术（LELE、SADP、SAQP）</a></li>
<li><a href="https://docs.pingcode.com/ask/61823.html">DUV和EUV光刻机的区别在哪 – PingCode</a></li>
<li><a href="https://www.sohu.com/a/811893835_121811690">EUV和DUV光刻机有什么区别？_技术_制造_芯片</a></li>

</ul>
</details>

**标签**: `#lithography`, `#semiconductor`, `#China`, `#SMIC`, `#DUV`

---