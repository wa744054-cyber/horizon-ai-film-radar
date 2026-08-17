---
layout: default
title: "Horizon Summary: 2026-08-17 (EN)"
date: 2026-08-17
lang: en
---

> From 36 items, 13 important content pieces were selected

---

1. [DuckDB 2.0 Preview Unveils Quack Protocol and Extension Repositories](#item-1) ⭐️ 9.0/10
2. [Qwen3.8 27B Scores 52 on Artificial Analysis, Beating Far Larger Models](#item-2) ⭐️ 9.0/10
3. [AI-Generated Copilot Autofix Introduces Command Injection in Snowflake's Jira](#item-3) ⭐️ 8.0/10
4. [GitHub Outage Sparks Debate on Reliability, Pricing, and Alternatives](#item-4) ⭐️ 8.0/10
5. [Anthropic CEO Dario Amodei: AI Regulation Is a Trust Crisis](#item-5) ⭐️ 8.0/10
6. [AirTag Tracking Links Rare Book Shipment to Amazon AI Facility](#item-6) ⭐️ 8.0/10
7. [SemiAnalysis Warns PJM's $12B Modeling Mistake Could Repeat](#item-7) ⭐️ 8.0/10
8. [Researcher Exposes Common Tricks That Make Sparse Attention Look Good](#item-8) ⭐️ 8.0/10
9. [OpenAI Previews Ultrafast Mode for GPT-5.6 Sol, Up to 14x Faster via Cerebras](#item-9) ⭐️ 8.0/10
10. [Stripe in Talks to Acquire OpenRouter at $10B Valuation](#item-10) ⭐️ 8.0/10
11. [ChatGPT macOS App Adds Opt-In Computer History That Tracks Clicks and Keystrokes](#item-11) ⭐️ 8.0/10
12. [Unitree's 'Superman' robot jumps 2m, runs 12.66 m/s, beating human records](#item-12) ⭐️ 8.0/10
13. [Italy Fines Apple $115 Million for Abusing App Store Dominance](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DuckDB 2.0 Preview Unveils Quack Protocol and Extension Repositories](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

The DuckDB v2.0 preview introduces Quack, a remote protocol that allows DuckDB instances to act as clients and servers over HTTP, and formalizes extension repositories with signed extensions. It also highlights rapid development with nearly 10,000 commits in under six months. DuckDB is a widely used in-process OLAP database; v2.0 shows significant evolution, especially Quack enabling server-like usage, which expands its use cases beyond embedded analytics. Extension repositories improve security and community contributions, potentially accelerating the ecosystem. Quack supports the full DuckDB feature set over the wire and allows multiple concurrent writers. Extension repositories are defined by a name, URL prefix, and RSA public keys for signing, with a core repository managed by the DuckDB team and community repositories for third-party extensions.

hackernews · ibotty · Aug 17, 13:46 · [Discussion](https://news.ycombinator.com/item?id=49330781)

**Background**: DuckDB is an open-source, column-oriented embedded SQL database designed for analytical queries on large datasets. It is known for high performance and integration with languages like Python and R. Extensions allow adding features such as new file formats and domain-specific functionality, and the new repository system ensures trust through signed releases.

<details><summary>References</summary>
<ul>
<li><a href="https://duckdb.org/quack/">Quack Remote Protocol – DuckDB</a></li>
<li><a href="https://duckdb.org/docs/current/extensions/installing_extensions">Installing Extensions – DuckDB</a></li>
<li><a href="https://en.wikipedia.org/wiki/DuckDB">DuckDB - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are enthusiastic, praising Quack and DuckDB's impact on reducing resource requirements. One user humorously asks about using minisign instead of RSA for extension signing, while another raises concern about the high commit velocity and potential AI involvement. A commenter also encourages funding database research.

**Tags**: `#DuckDB`, `#database`, `#release`, `#analytics`, `#community`

---

<a id="item-2"></a>
## [Qwen3.8 27B Scores 52 on Artificial Analysis, Beating Far Larger Models](https://artificialanalysis.ai/models/qwen3-8-27b) ⭐️ 9.0/10

Qwen3.8 27B, a small open-source model from Alibaba's Qwen family, achieved a score of 52 on the Artificial Analysis benchmark. This result outperforms much larger models such as Opus 4.6 and matches DeepSeek V4 Flash. This is significant because a 27B-parameter model that can run on a consumer gaming PC now rivals or beats frontier models built with enormous compute and data-center-scale resources. It challenges the assumption that raw scale is required for state-of-the-art capability and strengthens the case for efficient, locally runnable open-source AI. According to community comparisons, Qwen3.6 27B previously scored 38, while Qwen3.8 27B's 52 matches DeepSeek V4 Flash 0731, which ranks #5 in the large-model category (over 150B parameters). It also reportedly beats all medium models in the 40B–150B range on Artificial Analysis.

hackernews · anana_ · Aug 17, 17:25 · [Discussion](https://news.ycombinator.com/item?id=49334544)

**Background**: Artificial Analysis is an independent platform that benchmarks AI models and API providers across quality, price, output speed, and latency. The Qwen family, developed by Alibaba Cloud's DAMO Academy, is a series of open-weight language models released under the Apache 2.0 license, ranging from small dense models to large mixture-of-experts models. A score of 52 on Artificial Analysis represents a composite measure of intelligence and capability based on the platform's evaluations.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://huggingface.co/Qwen">Org profile for Qwen on Hugging Face, the AI community building the...</a></li>
<li><a href="https://qwen.moe/">Qwen — Open Foundation Models</a></li>

</ul>
</details>

**Discussion**: The community reaction is a mix of excitement and disbelief: commenters note that a 27B model beating Opus 4.6 is 'funny and a bit terrifying,' and that it runs decently on gaming hardware. Several users report hands-on testing, describing the model as intelligent, strange, and highly agentic — obsessively solving problems in unusual ways — while others plan extensive testing to verify the benchmark results in real-world coding workflows.

**Tags**: `#Qwen`, `#AI benchmarks`, `#small language models`, `#open-source AI`, `#model efficiency`

---

<a id="item-3"></a>
## [AI-Generated Copilot Autofix Introduces Command Injection in Snowflake's Jira](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

A GitHub Copilot Autofix recommendation introduced a command injection vulnerability in a Snowflake GitHub Actions workflow, which was exploited to compromise Snowflake's Jira instance. The incident demonstrates a real-world failure of AI-generated code fixes in a security-critical context. This incident highlights the security risks of AI-assisted coding, where automated fixes can inadvertently introduce new vulnerabilities. It underscores the need for rigorous review and static analysis of AI-generated code, especially in CI/CD pipelines that often handle sensitive infrastructure. The vulnerability was a template injection in a GitHub Actions workflow (jira_issue.yml) that allowed arbitrary command execution via unescaped title and body variables. A zizmor static analysis scan flagged the issue with the error 'template-injection: code injection via template expansion' at line 24 of the workflow.

hackernews · galnagli · Aug 17, 14:18 · [Discussion](https://news.ycombinator.com/item?id=49331423)

**Background**: GitHub Copilot Autofix is a feature that automatically suggests fixes for code scanning alerts, aiming to speed up vulnerability remediation. Command injection occurs when unsafe user input is passed to a shell, allowing attackers to execute arbitrary commands. In GitHub Actions workflows, template expressions like ${{ }} are evaluated by the runner, and using them inside run commands without proper escaping can lead to code injection.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/code-security/responsible-use/responsible-use-autofix-code-scanning">Responsible use of Copilot Autofix for code scanning - GitHub Docs</a></li>
<li><a href="https://portswigger.net/web-security/os-command-injection">What is OS command injection, and how to prevent it? | Web Security Academy</a></li>

</ul>
</details>

**Discussion**: Commenters argued that writing GitHub Actions without static analysis is negligent and recommended using zizmor in CI to catch template injection issues. One user observed that AI lowers the cost of generating changes but not the cost of reviewing them, shifting the bottleneck to verification. Another questioned whether the vulnerable change was truly Copilot-generated, noting the linked PR's Copilot commit was unrelated to the vulnerability.

**Tags**: `#AI code generation`, `#security`, `#GitHub Actions`, `#supply chain`, `#Copilot`

---

<a id="item-4"></a>
## [GitHub Outage Sparks Debate on Reliability, Pricing, and Alternatives](https://www.githubstatus.com/incidents/zkxwbgr0cnmx) ⭐️ 8.0/10

GitHub suffered a major service incident (zkxwbgr0cnmx) on githubstatus.com, with users receiving "No server is currently available" errors on core features like web diffs. The incident lasted for hours, with status updates reporting degraded performance across API Requests, Actions, Git Operations, Issues, Pages, Pull Requests, and Webhooks. GitHub is a critical platform for open source and enterprise development, so this outage disrupted countless developer workflows and CI/CD pipelines. The large community discussion also highlights growing concerns about GitHub's reliability, pricing, and dependence on Microsoft, with some users actively considering alternatives. The incident was first reported by a user before the official status page was updated, and "We are still working to identify the root cause" remained for nearly three hours. Some services were briefly mitigated before Git Operations degraded again, showing that recovery was not immediate.

hackernews · SpyCoder77 · Aug 17, 13:35 · [Discussion](https://news.ycombinator.com/item?id=49330597)

**Background**: A status page is a public dashboard that shows the real-time operational status of a service's components, such as APIs, databases, and web interfaces, helping organizations communicate incidents and maintenance. A service incident is an anomalous event that causes or may lead to service degradation or an outage, requiring human intervention to restore normal operations. GitHub's status page at githubstatus.com is the official channel for reporting such incidents to users.

<details><summary>References</summary>
<ul>
<li><a href="https://statusbot.flaredesk.com/status-page/">Status Page – StatusBot by Flaredesk</a></li>
<li><a href="https://okchecker.com/blog/what-is-status-page">What Is a Status Page and Why You Need One | OKchecker</a></li>
<li><a href="https://handbook.gitlab.com/handbook/engineering/infrastructure-platforms/incident-management/">Incident Management | The GitLab Handbook</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong frustration, with some saying this outage was a "tipping point" and others vowing to leave GitHub for cheaper, more portable hosting options. There was debate about whether GitHub should rate-limit non-paying users or charge for resources consumed by LLM-generated traffic, and criticism of Microsoft's stewardship of the platform.

**Tags**: `#github`, `#incident`, `#outage`, `#reliability`, `#devops`

---

<a id="item-5"></a>
## [Anthropic CEO Dario Amodei: AI Regulation Is a Trust Crisis](https://twitter.com/DarioAmodei/status/2088758816376807762) ⭐️ 8.0/10

Dario Amodei, CEO of Anthropic, published a statement arguing that AI regulation is fundamentally a crisis of trust, saying ordinary people distrust companies, governments, and the tech industry. He rejected the idea of a glitzy marketing campaign with a positive spin, instead promising that Anthropic's real achievements—especially in biology and medicine—will be announced as loudly as possible once accomplished. This shapes how a leading AI lab frames the public policy debate on AI regulation, highlighting a growing credibility gap between frontier AI companies and the public. The mixed community reaction—ranging from genuine trust to accusations of condescending rhetoric—shows how perception can influence AI governance discussions. Amodei specifically noted that a positive-spin marketing campaign would not win back trust, saying 'AI will cure cancer' has become a cliché that most people find deceptive. He claimed Anthropic is rapidly ramping up its biology and medicine efforts, expecting 'early glimmers' in the coming months and 'incredible results' in the coming years.

hackernews · jacquesm · Aug 17, 01:59 · [Discussion](https://news.ycombinator.com/item?id=49325789)

**Background**: AI regulation is a major policy topic as frontier models from Anthropic, OpenAI, and Google advance rapidly. Trust is central to this debate because the public and regulators worry about power concentration, safety, and whether AI companies serve the public interest rather than their own. Amodei's comments respond to broader criticism that Anthropic's safety rhetoric does not always match its behavior, including debates about open weights and closed development.

**Discussion**: Community responses were divided: some commenters, like mhaberl, expressed genuine trust in Amodei's intentions, while others, like mindwok, argued Anthropic has a major PR problem and uses condescending 'Orwellian' rhetoric that makes the public feel distrusted. Another commenter, pu_pe, added that AI structurally concentrates power due to scaling laws, and open-weights only partially address this by shifting concentration to those who control compute and chips.

**Tags**: `#AI regulation`, `#Anthropic`, `#trust`, `#AI policy`, `#community discussion`

---

<a id="item-6"></a>
## [AirTag Tracking Links Rare Book Shipment to Amazon AI Facility](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

Investigative outlet 404 Media embedded an Apple AirTag inside a rare book from a 1,000-volume order. The package was delivered to the VGT3 corner of Amazon's LAS8 facility in Las Vegas, confirming that the books are being destructively scanned for AI training data. This is the first direct tracking evidence tying bulk rare-book purchases to an Amazon AI training operation, lending weight to suspicions that AI companies are sourcing training data without authorization. It sharpens the ongoing copyright and fair-use debate over mass book scanning for AI. The order was placed on the Biblio marketplace, and the AirTag arrived at VGT3, which Amazon workers' online discussions said is used for destructive book scanning. The facility entrance even displayed a dinosaur-with-book logo, an apparent nod to the scanning operation.

rss · Simon Willison · Aug 17, 15:21

**Background**: AI companies have been suspected of buying large quantities of physical books from used-book marketplaces, scanning them to create training corpora, and then discarding or destroying the physical copies. A 2025 lawsuit against Anthropic revealed 'Project Panama,' a secret effort to scan millions of books, and Judge Alsup's fair-use ruling on destructive scanning is now shaping industry practice. Biblio is a major marketplace for rare and antiquarian books, where such bulk, price-insensitive orders have been reported.

<details><summary>References</summary>
<ul>
<li><a href="https://www.404media.co/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-training-facility/">We Tracked a Shipment of Rare Books . It Ended at an Amazon AI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Biblio.com">Biblio.com - Wikipedia</a></li>
<li><a href="https://www.ibtimes.co.uk/anthropic-secret-book-scanning-operation-1811155">Inside Project Panama, Anthropic's Secret Effort To Scan ... | IBTimes UK</a></li>

</ul>
</details>

**Tags**: `#AI training`, `#data sourcing`, `#copyright`, `#Amazon`, `#investigation`

---

<a id="item-7"></a>
## [SemiAnalysis Warns PJM's $12B Modeling Mistake Could Repeat](https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted) ⭐️ 8.0/10

SemiAnalysis published an analysis claiming that a modeling mistake in PJM's grid planning wasted $12 billion of US ratepayer money. The article warns that PJM's structurally anti-growth capacity market and governance system could lead to the same costly error again. The finding highlights the enormous financial stakes in grid modeling assumptions for US electricity markets. It matters because PJM's capacity market design affects reliability investments and billions in consumer costs, and repeating the mistake would further burden ratepayers. The analysis faults PJM's model as structurally anti-growth, with a poorly designed capacity market that is globally unique and a governance system too big to function effectively. It includes a live rebuild of the relevant reserve calculation to expose the error.

rss · Semianalysis · Aug 16, 22:27

**Background**: PJM Interconnection operates the wholesale electricity market for a large portion of the US East Coast, including a capacity market that pays generators years in advance to be available for future demand. Capacity auction results, like the July 2024 auction clearing at $269.92/MW-day in most of PJM, directly affect consumer bills. When planning models misforecast the reserve margin or demand, the market can procure more capacity than needed, wasting ratepayer money.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted">Full of Cold Air - PJM's $12B modeling mistake</a></li>
<li><a href="https://www.congress.gov/crs-product/R48553">PJM’s Electric Capacity Market: Background and Current Issues | Congress.gov | Library of Congress</a></li>
<li><a href="https://www.pjm.com/markets-and-operations/rpm.aspx">PJM - Capacity Market (RPM)</a></li>

</ul>
</details>

**Tags**: `#grid modeling`, `#energy policy`, `#PJM`, `#infrastructure`, `#cost analysis`

---

<a id="item-8"></a>
## [Researcher Exposes Common Tricks That Make Sparse Attention Look Good](https://www.reddit.com/r/MachineLearning/comments/1vqqqcs/how_to_make_any_sparse_attention_kv_compression/) ⭐️ 8.0/10

A researcher specializing in KV cache compression published a Twitter thread (shared on r/MachineLearning) detailing common tricks and benchmark settings used to make sparse attention and KV compression methods appear artificially effective. The post specifically calls out practices such as using misleading single-hop retrieval tasks, cherry-picking baselines, and hiding failures behind aggregate metrics. This critique matters because evaluation practices directly influence which methods are perceived as state-of-the-art and get adopted. By exposing common pitfalls, it encourages the ML community to demand fairer benchmarks and more rigorous comparisons in sparse attention and KV compression research. The post lists four main tricks: choosing single-hop retrieval tasks without distractors, never isolating a method's contribution (e.g., using different window/block sizes than baselines), relying only on aggregate metrics to hide weak areas (citing RULER's 13 tasks as an example), and selecting saturated benchmarks where all models score similarly. The author admits to being guilty of some practices and says they are trying to improve.

reddit · r/MachineLearning · /u/korec1234 · Aug 17, 12:18

**Background**: KV cache is a mechanism in transformer models that stores previously computed key and value vectors to speed up autoregressive inference, but it grows with sequence length, creating memory and bandwidth bottlenecks. Sparse attention methods aim to reduce these costs by restricting which key-value pairs each token attends to, but their effectiveness is highly sensitive to evaluation design. The needle-in-a-haystack (NIAH) test is a common long-context retrieval benchmark where a single relevant piece of information is placed among irrelevant context, and it can be gamed if the context contains no distracting or competing information.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/docs/transformers/kv_cache">Cache strategies · Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/sparse-attention">Sparse Attention Mechanisms - emergentmind.com</a></li>
<li><a href="https://arxiv.org/abs/2407.01437">[2407.01437] Needle in the Haystack for Memory Based Large Language Models</a></li>

</ul>
</details>

**Tags**: `#KV Cache`, `#Sparse Attention`, `#Model Evaluation`, `#Efficient Transformers`, `#Research Critique`

---

<a id="item-9"></a>
## [OpenAI Previews Ultrafast Mode for GPT-5.6 Sol, Up to 14x Faster via Cerebras](https://t.me/zaihuapd/43228) ⭐️ 8.0/10

OpenAI unveiled a preview of Ultrafast, a new OpenAI API service tier that runs GPT-5.6 Sol up to 14 times faster than Standard processing. Powered by Cerebras, it generates up to 750 output tokens per second, and is currently limited to a small group of customers. This matters because sub-second responses could make OpenAI's most capable model practical for time-sensitive use cases such as incident response, financial research, customer support, and e-commerce. It also signals OpenAI's willingness to lean on specialized hardware partners to improve inference performance. Ultrafast runs on Cerebras wafer-scale engine hardware and, according to OpenAI and Cerebras, delivers the speedup without compromising model quality. The preview is capacity-constrained, and OpenAI says it will expand access as compute capacity grows.

telegram · zaihuapd · Aug 17, 00:47

**Background**: Cerebras Systems designs wafer-scale processors and an AI inference/training cloud, using an entire silicon wafer as a single chip to reduce latency compared with GPU clusters. GPT-5.6 is OpenAI's large language model family released in July 2026, with variants Luna, Terra, and Sol; Sol is the most capable variant. Ultrafast applies Cerebras' low-latency inference stack to Sol via the OpenAI API.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>
<li><a href="https://techcrunch.com/2026/08/13/openai-introduces-ultrafast-a-new-mode-that-makes-gpt-5-6-sol-work-at-14x-the-speed/">OpenAI introduces 'Ultrafast,' a new mode that makes GPT-5.6 Sol work at 14x the speed | TechCrunch</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#performance`, `#API`, `#Cerebras`

---

<a id="item-10"></a>
## [Stripe in Talks to Acquire OpenRouter at $10B Valuation](https://t.me/zaihuapd/43229) ⭐️ 8.0/10

The Wall Street Journal reported on the 24th that Stripe is in negotiations to acquire OpenRouter, an AI model routing startup, at a valuation of about $10 billion. A deal could be reached, according to people familiar with the matter. A $10 billion acquisition would signal that AI infrastructure is becoming a strategic layer for core financial technology firms. If completed, Stripe could embed model routing and AI access into its payments and commerce ecosystem, affecting developers and businesses building AI-powered features. The talks are still in flux and no final agreement has been confirmed, so the valuation and deal terms could change. OpenRouter offers a unified API that lets developers access hundreds of AI models through a single integration, which is the core asset Stripe would gain.

telegram · zaihuapd · Aug 17, 01:19

**Background**: AI model routing is a technique that sends each incoming request to the most appropriate AI model rather than hardcoding a single model for all tasks. OpenRouter is a gateway that aggregates many large language models behind one API, simplifying access for developers. Stripe is a major online payments company that has been deepening its AI and developer tooling offerings.

<details><summary>References</summary>
<ul>
<li><a href="https://inworld.ai/resources/what-is-an-ai-router">What Is an AI Router? LLM Model Routing Explained (2026)</a></li>
<li><a href="https://evolink.ai/blog/what-is-ai-model-routing-guide-for-developers">What Is AI Model Routing? A Practical Guide for Developers | EvoLink</a></li>
<li><a href="https://openrouter.ai/docs/quickstart">OpenRouter Quickstart Guide</a></li>

</ul>
</details>

**Tags**: `#Stripe`, `#OpenRouter`, `#AI`, `#acquisition`, `#fintech`

---

<a id="item-11"></a>
## [ChatGPT macOS App Adds Opt-In Computer History That Tracks Clicks and Keystrokes](https://www.theverge.com/ai-artificial-intelligence/980742/chatgpts-computer-history-tracks-your-clicks-and-keystrokes) ⭐️ 8.0/10

OpenAI has introduced Computer History in the ChatGPT macOS desktop app, an opt-in feature that records clicks and keystrokes to build an activity timeline for training and automation. The feature replaces the earlier Chronicle research preview and is currently rolling out to certain account types. This marks another step toward AI assistants that can observe and automate real computer activity, but it also raises significant privacy concerns. The feature is similar to Windows Recall but avoids screenshots, potentially setting a new precedent for how desktop AI agents handle sensitive user data. Computer History is opt-in by default, allows users to exclude specific apps and websites, can delete records, and ignores incognito or private browsing tabs. OpenAI states it does not capture images, video, or audio, only 'events' such as clicks and keystrokes.

telegram · zaihuapd · Aug 17, 04:16

**Background**: ChatGPT's macOS app is an AI assistant client that lets users chat with OpenAI's models and now integrates with Codex, an AI coding agent. Computer History creates a searchable timeline of app and website activity that ChatGPT and Codex can use to learn workflows and suggest automations. The feature is reminiscent of Windows Recall, a Windows 11 feature that captures screenshots, which faced significant backlash over privacy concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.chatgpt.com/docs/customization/computer-history">Computer History | ChatGPT Learn</a></li>
<li><a href="https://www.zdnet.com/article/chatgpt-computer-history/">ChatGPT's new Computer History tracks your Mac activity to create a timeline - but should you let it? | ZDNET</a></li>
<li><a href="https://en.wikipedia.org/wiki/Windows_Recall">Windows Recall</a></li>

</ul>
</details>

**Tags**: `#ChatGPT`, `#OpenAI`, `#privacy`, `#AI assistant`, `#macOS`

---

<a id="item-12"></a>
## [Unitree's 'Superman' robot jumps 2m, runs 12.66 m/s, beating human records](https://m.weibo.cn/detail/5332901463070926) ⭐️ 8.0/10

Unitree Robotics unveiled a preview of its new humanoid robot, 'Superman,' on Monday, claiming it can jump 2 meters from a standstill and reach a top speed of 12.66 meters per second. The company said the entire machine was developed in just over three months and will be further refined in the coming months. This announcement is significant because 'Superman' reportedly exceeds human records in both standing vertical jump and running speed, marking a milestone for humanoid robotics. The reveal comes days before Unitree is set to become the first general-purpose robotics company to list on mainland China's stock market, underscoring the commercial momentum of the sector. The robot has a leg length of 0.85 meters and a top speed of 12.66 m/s, which edges past the fastest speed ever recorded by Usain Bolt. Since this is only a preview, technical specifications are limited, and Unitree says significant room for improvement remains over the next few months.

telegram · zaihuapd · Aug 17, 07:12

**Background**: Unitree Robotics, founded in Hangzhou in 2016, is a Chinese company that initially specialized in quadruped robots for the consumer market and has since expanded into humanoid robots. High-speed bipedal running and jumping in humanoids require advanced locomotion control, high-speed sensors, and AI-based planning, areas that have seen rapid progress in recent years. The company's upcoming listing on mainland China's stock market reflects growing investor interest in robotics and AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/unitree-robot-hits-12-66-094529616.html">Unitree’s New Robot Hits 12.66 m/s — Faster Than Usain Bolt Ever Ran</a></li>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/chinese-humanoid-robot-maker-unitree-123559978.html">China's Unitree unveils 'Superman' robot as fervour builds ahead of Shanghai debut</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#humanoid`, `#Unitree`, `#AI`, `#engineering`

---

<a id="item-13"></a>
## [Italy Fines Apple $115 Million for Abusing App Store Dominance](https://t.me/zaihuapd/43243) ⭐️ 8.0/10

Italy's antitrust authority AGCM fined Apple $115 million for abusing its dominant position in the App Store through its App Tracking Transparency (ATT) policy. The regulator found that Apple unilaterally imposed ATT requirements on third-party developers while exempting its own apps from the same permission prompts. This ruling could set a precedent for how privacy-focused policies like ATT are scrutinized for competitive fairness. It may pressure Apple to harmonize its data-tracking rules for both third-party and first-party apps, affecting developers' ad revenue and user data access across the EU and beyond. AGCM said ATT's terms were imposed unilaterally and were disproportionate to Apple's stated privacy goals, harming developers' commercial interests. The fine amounts to roughly €100 million, and Apple responded that it strongly disagrees with the decision, arguing that regulators ignored the privacy benefits ATT provides to users.

telegram · zaihuapd · Aug 17, 12:50

**Background**: App Tracking Transparency (ATT) is a privacy feature introduced in iOS 14.5 that requires apps to obtain user permission before tracking their activity across other companies' apps and websites. Apple enforces this rule for all third-party apps distributed through the App Store, but its own apps are not required to display the same prompt. This asymmetry has drawn criticism from developers and regulators, who argue that Apple uses its App Store dominance to impose unfair conditions. The Italian action is part of broader global scrutiny of Apple's App Store practices.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/apptrackingtransparency">App Tracking Transparency | Apple Developer Documentation</a></li>
<li><a href="https://support.apple.com/en-us/102420">If an app asks to track your activity - Apple Support</a></li>
<li><a href="https://medium.com/design-bootcamp/prompt-apples-app-tracking-transparency-policy-att-31a8a482b5b1">App Tracking Transparency (ATT): Apple’s Privacy ... - Medium</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#Apple`, `#App Store`, `#privacy`, `#regulation`

---