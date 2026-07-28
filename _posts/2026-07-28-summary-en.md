---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 29 items, 7 important content pieces were selected

---

1. [Critical RCE in Fastjson 1.x Without Gadget, Affects JDK 8/17/21](#item-1) ⭐️ 9.0/10
2. [Anthropic CEO Opposes Open-Weights Models, Supports China Chip Bans](#item-2) ⭐️ 8.0/10
3. [A missing underscore sent innocent man to prison for 18 months](#item-3) ⭐️ 8.0/10
4. [Moonshot AI Releases 2.8 Trillion Parameter Kimi-K3 Weights](#item-4) ⭐️ 8.0/10
5. [DP-FedSOFIM: Second-Order DP Federated Learning Without Extra Cost](#item-5) ⭐️ 8.0/10
6. [Solo Evaluation of 6 Frontier LLMs Reveals Left-Leaning Bias](#item-6) ⭐️ 8.0/10
7. [SMIC Tests China's First Domestic DUV Lithography Machine](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Critical RCE in Fastjson 1.x Without Gadget, Affects JDK 8/17/21](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a high-risk remote code execution (RCE) vulnerability in Fastjson versions 1.2.68 through 1.2.83, which requires no gadget chain and no autoType support, affecting JDK 8, 17, and 21. No official patch is available as Fastjson 1.x reached end of life in October 2024. This vulnerability is critical because it allows unauthenticated remote code execution without requiring common bypass conditions like autoType or classpath gadgets, making it easier to exploit. Given Fastjson's widespread use in Java applications, especially in Alibaba ecosystems and other enterprise environments, this poses a severe security risk with no official mitigation. The vulnerability works against Fastjson 1.2.68–1.2.83 and exploits the default SafeMode disabled state; a confirmed attack vector requires a Spring Boot executable fat-JAR and a network-reachable path sending attacker-controlled JSON. The only effective remediation is upgrading to Fastjson 2 or enabling SafeMode and restricting deserialization sources.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular JSON serialization/deserialization library for Java, developed by Alibaba. The autoType feature allows type information to be embedded in JSON to enable polymorphic deserialization, but historically, it has been a frequent attack surface. A 'gadget chain' is a sequence of existing classes on the classpath that, when deserialized, executes arbitrary code; many previous Fastjson vulnerabilities required such gadgets. This new vulnerability bypasses both autoType and gadget requirements, making it exceptionally dangerous. SafeMode, introduced in 1.2.68, disables autoType completely; however, it is not enabled by default.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html">Fastjson 1.x RCE Vulnerability Targeted in Attacks With No Patched...</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson_safemode_en · alibaba/fastjson Wiki</a></li>
<li><a href="https://github.com/frohoff/ysoserial">GitHub - frohoff/ysoserial: A proof-of-concept tool for ... Java Deserialization Attacks: From Gadget Chains to RCE Java deserialization tricks - Synacktiv Lab: Developing a custom gadget chain for Java deserialization Rev Gadget: A Java Deserialization Gadget Chains Discover ... GrrrDog/Java-Deserialization-Cheat-Sheet - GitHub</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#Fastjson`, `#RCE`, `#Java`

---

<a id="item-2"></a>
## [Anthropic CEO Opposes Open-Weights Models, Supports China Chip Bans](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic CEO Dario Amodei published a blog post stating the company opposes open-weights AI models due to safety risks, and supports U.S. chip export bans to China. This stance from a leading AI company intensifies the debate over open vs. closed AI development, potentially influencing policy and industry norms. Amodei specifically advocates for banning chip sales to China and cracking down on smuggling, while acknowledging that bans alone are not a silver bullet.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights models make trained neural network parameters publicly available, allowing modification and redistribution. Unlike fully open-source models, they often lack the training data and code needed to fully reproduce the model. This distinction is central to debates about safety, accessibility, and competition in AI.

<details><summary>References</summary>
<ul>
<li><a href="https://infercom.ai/glossary/open-weights-model/">What is an Open - Weight Model ? Definition | Infercom</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>

</ul>
</details>

**Discussion**: Commenters largely criticized Amodei's position as self-serving and inconsistent, with some accusing him of virtue signaling. Others questioned the logic of supporting bans while claiming they are ineffective.

**Tags**: `#AI safety`, `#open-source models`, `#Anthropic`, `#AI policy`, `#China`

---

<a id="item-3"></a>
## [A missing underscore sent innocent man to prison for 18 months](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

Due to a missing underscore in a police subpoena, Kik's system returned the wrong user's data, leading to an innocent Canadian man being wrongfully convicted and imprisoned for 18 months on child exploitation charges. This case underscores how a minor technical oversight in legal procedures can have devastating human consequences, highlighting the urgent need for better technical literacy in law enforcement and more robust verification methods when handling digital evidence. The subpoena requested information for Kik user 'fus_ro_dah' (with one underscore), but due to SQL wildcard interpretation, it matched a different user 'fus_ro_dah' (with two underscores) — the underscore character acts as a single-character wildcard in SQL LIKE queries, so 'fus_ro_dah' matched any string starting with 'fus' followed by any character and then 'ro_dah'.

hackernews · quantified · Jul 27, 22:10 · [Discussion](https://news.ycombinator.com/item?id=49076116)

**Background**: In SQL databases, the underscore (_) is a wildcard that matches any single character when used with the LIKE operator. If a search pattern contains an underscore without proper escaping, the database interprets it as a wildcard rather than a literal underscore. This technical nuance was overlooked in the police subpoena to Kik, causing the wrong account to be identified. The victim was in the US, the defendant in Canada, and cross-border investigation added complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.w3resource.com/sql/wildcards-like-operator/wildcards-underscore.php">SQL wildcards underscore ( _ ) - w3resource</a></li>
<li><a href="https://learn.microsoft.com/en-us/sql/t-sql/language-elements/wildcard-match-one-character-transact-sql?view=sql-server-ver17">_ (Wildcard - Match One Character) (Transact-SQL) - SQL Server | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage at the wrongful conviction, questioning why the defense lawyer failed to challenge the flawed digital evidence. Many highlighted the need for compensation beyond vacating the conviction, noting lifelong reputational damage. Some also pointed out the jurisdictional issues between US and Canada that may have hampered a fair trial.

**Tags**: `#wrongful conviction`, `#legal tech`, `#data accuracy`, `#criminal justice`, `#technology failure`

---

<a id="item-4"></a>
## [Moonshot AI Releases 2.8 Trillion Parameter Kimi-K3 Weights](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI released the weights for their 2.8 trillion parameter Kimi-K3 model on Hugging Face, under a custom license that requires large commercial entities to enter a separate agreement for Model as a Service (MaaS) businesses. This release continues the trend of extremely large open-weight models, but its non-standard license—requiring attribution for high-revenue companies and a separate deal for MaaS providers—sparks debate on the boundaries of open source and open weight in AI. The Kimi-K3 model weights are 1.56 TB in size, and the license no longer calls itself modified MIT, explicitly requiring a separate agreement for MaaS providers with over $20 million in aggregate revenue over any consecutive 12 months.

rss · Simon Willison · Jul 27, 23:39

**Background**: Moonshot AI previously released Kimi-K2 under a modified MIT license that added attribution requirements for commercial entities with over 100 million MAU or $20 million monthly revenue. The K3 license goes further by targeting MaaS businesses and no longer labeling itself as modified MIT. Open-weight models grant access to model parameters but often impose restrictions beyond traditional open-source definitions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-K3/blob/main/LICENSE">Kimi-K3/LICENSE at main · MoonshotAI/Kimi-K3 · GitHub</a></li>
<li><a href="https://kingy.ai/ai/ai-guides/kimi-k3-license-commercial-use-open-source/">Kimi K3 License: Commercial Use Is Allowed—with Conditions</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Large Language Models`, `#Open Source`, `#Moonshot`, `#Kimi-K3`

---

<a id="item-5"></a>
## [DP-FedSOFIM: Second-Order DP Federated Learning Without Extra Cost](https://www.reddit.com/r/MachineLearning/comments/1v8pkb7/dpfedsofim_secondorder_federated_optimization/) ⭐️ 8.0/10

DP-FedSOFIM introduces a second-order federated optimization method that achieves differential privacy with no additional privacy cost or O(d²) communication overhead by moving curvature estimation entirely to the server. This work addresses a key limitation in differentially private federated learning—prior second-order methods required heavy client-side computation and communication of full matrices, limiting scalability. DP-FedSOFIM shows that useful curvature information can be extracted from already-privatized aggregates, enabling faster convergence under tight privacy budgets. The server maintains an exponential moving average (EMA) of privatized gradient aggregates and uses its regularized rank-one outer product as a Fisher proxy, applying the Sherman-Morrison formula for efficient preconditioning without forming the matrix. Experiments show round-10 accuracy gains of up to +20.3 points over DP-FedGD on CIFAR-10/ResNet at epsilon=5, with under 2% wall-clock overhead per round.

reddit · r/MachineLearning · /u/worthybog0 · Jul 28, 06:04

**Background**: Federated learning (FL) trains a shared model across decentralized data without centralizing it, but model updates can leak private information. Differential privacy (DP) mitigates this by clipping and adding noise to client updates, but noise injection degrades convergence, especially under tight privacy budgets. Standard DP-FL methods use first-order optimization, while second-order methods can improve convergence but typically require clients to compute and transmit full covariance matrices (O(d²) cost), introducing new privacy sensitivity and communication bottlenecks.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2601.09166v1">DP-FedSOFIM: Differentially Private Federated Stochastic ...</a></li>
<li><a href="https://arxiv.org/html/2505.23588v1">Accelerated Training of Federated Learning via Second-Order ...</a></li>

</ul>
</details>

**Tags**: `#Federated Learning`, `#Differential Privacy`, `#Second-Order Optimization`, `#Privacy-Preserving Machine Learning`

---

<a id="item-6"></a>
## [Solo Evaluation of 6 Frontier LLMs Reveals Left-Leaning Bias](https://www.reddit.com/r/MachineLearning/comments/1v8fnzw/evaluated_6_frontier_llms_gpt54_claude_sonnet_46/) ⭐️ 8.0/10

A solo evaluation of six frontier LLMs (GPT-5.4, Claude Sonnet 4.6, Claude Opus 4.7, Gemini Pro, Gemini Flash, and Grok 4.3) across 8 bias benchmarks with ~20,600 examples found that all models, including Grok, exhibited left-leaning political bias despite Grok's self-reported right-leaning stance. Additionally, refusal rates on race-related questions varied significantly, with GPT-5.4 refusing 20.3% of the time. This study provides empirical evidence that even models designed to avoid bias or with stated political leanings can exhibit systemic left-leaning behavior, which has implications for fairness in AI applications. It highlights the need for ongoing bias auditing and transparency in model behavior. The evaluation used eight established datasets: WinoBias, BBQ Race/Ethnicity, SeeGULL, OpinionsQA, cajcodes Political Bias, Hyperpartisan News, and Political Compass. A notable limitation is that this is a solo, non-peer-reviewed project with single prompt templates and no multi-run averaging.

reddit · r/MachineLearning · /u/marggggggggg · Jul 27, 22:37

**Background**: Bias benchmarks like WinoBias and BBQ evaluate LLMs for stereotypical associations in coreference and question answering tasks. WinoBias uses Winograd-schema sentences to measure occupational gender bias, while BBQ (Bias Benchmark for QA) assesses bias across social categories including race and gender. These benchmarks are widely used to detect unintended model biases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winobias">WinoBias : Gender Bias in Coreference Benchmark</a></li>
<li><a href="https://deepeval.com/docs/benchmarks-bbq">BBQ | DeepEval - The LLM Evaluation Framework</a></li>
<li><a href="https://github.com/google-research-datasets/seegull">GitHub - google-research-datasets/seegull: SeeGULL is a broad-coverage stereotype dataset in English containing stereotypes about identity groups spanning 178 countries across 8 different geo-political regions across 6 continents, as well as state-level identities within the US and India. · GitHub</a></li>

</ul>
</details>

**Tags**: `#AI bias`, `#LLM evaluation`, `#political bias`, `#model behavior`, `#fairness benchmarks`

---

<a id="item-7"></a>
## [SMIC Tests China's First Domestic DUV Lithography Machine](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

SMIC is currently trialing China's first domestically developed deep ultraviolet (DUV) lithography machine, built by Shanghai startup Yuliangsheng. The system is being used to produce 28nm chips and may eventually be used for 7nm and even 5nm through multi-patterning techniques. This development represents a critical step in China's effort to achieve semiconductor self-sufficiency and reduce reliance on ASML, especially given US export restrictions on advanced equipment. If successful, it could reshape global chip manufacturing supply chains. Most components of the DUV machine are domestically produced, though some parts still rely on imports. Industry insiders estimate that mass production with stable yields is at least one to two years away, with potential volume production by 2027.

telegram · zaihuapd · Jul 27, 14:10

**Background**: DUV lithography uses 193nm wavelength light, while EUV uses 13.5nm, offering higher resolution for advanced nodes. China currently uses ASML's DUV tools for its most advanced chips, but EUV sales to China are banned. Multi-patterning techniques like SADP allow DUV to produce features smaller than its optical limit, enabling 7nm and 5nm nodes, albeit with lower yield and higher cost.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1960307062815855033">半导体先进工艺：多重图形化技术（LELE、SADP、SAQP）</a></li>
<li><a href="https://docs.pingcode.com/ask/61823.html">DUV和EUV光刻机的区别在哪 – PingCode</a></li>
<li><a href="https://www.sohu.com/a/811893835_121811690">EUV和DUV光刻机有什么区别？_技术_制造_芯片</a></li>

</ul>
</details>

**Tags**: `#lithography`, `#semiconductor`, `#China`, `#SMIC`, `#DUV`

---