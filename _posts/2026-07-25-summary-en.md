---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 41 items, 15 important content pieces were selected

---

1. [Two Chinese Mathematicians Awarded 2026 Fields Medal](#item-1) ⭐️ 10.0/10
2. [Anthropic Releases Claude Opus 5, New Flagship Model](#item-2) ⭐️ 9.0/10
3. [Security camera ships GitHub admin token in login page](#item-3) ⭐️ 9.0/10
4. [Compiler Transforms Computation Graphs into Transformer Weights without Training](#item-4) ⭐️ 9.0/10
5. [Postgres LISTEN/NOTIFY scales to 60K notifications per second](#item-5) ⭐️ 8.0/10
6. [Software Quality Declines Despite Coding Advancements](#item-6) ⭐️ 8.0/10
7. [Tech Giants Warn Against Overregulating Open-Weight AI](#item-7) ⭐️ 8.0/10
8. [IRGC claims destruction of AWS Bahrain data center](#item-8) ⭐️ 8.0/10
9. [Buz: Fork of Bun Achieves Sub-Second Incremental Builds](#item-9) ⭐️ 8.0/10
10. [India orders GitHub to remove Bluetooth chat app Bitchat](#item-10) ⭐️ 8.0/10
11. [AMD Challenges NVIDIA's CUDA Dominance at Advancing AI 2026](#item-11) ⭐️ 8.0/10
12. [OpenAI Releases Enterprise AI Product Presence, Software Stocks Plunge](#item-12) ⭐️ 8.0/10
13. [Telegram Zero-Click Crash Vulnerability Silently Patched](#item-13) ⭐️ 8.0/10
14. [Ctrip unit fined $1.4M for illegal data exports](#item-14) ⭐️ 8.0/10
15. [Qualcomm announces across-the-board price hike starting September 1](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Two Chinese Mathematicians Awarded 2026 Fields Medal](https://t.me/zaihuapd/42748) ⭐️ 10.0/10

The International Mathematical Union has announced the 2026 Fields Medal winners, including two mathematicians of Chinese nationality: Deng Yu for contributions to partial differential equations and John Pardon for work in symplectic geometry. This marks the first time two Chinese mathematicians have won the Fields Medal in a single year, highlighting the growing prominence of Chinese research in pure mathematics and inspiring a new generation of mathematicians globally. Deng Yu was recognized for rigorously deriving the Boltzmann equation from hard-sphere dynamics and for probabilistic methods in nonlinear Schrödinger dynamics, while John Pardon was honored for developing new virtual fundamental cycle techniques and contributions to Fukaya categories.

telegram · zaihuapd · Jul 24, 12:51

**Background**: The Fields Medal is awarded every four years to mathematicians under 40 who have made outstanding contributions and show future promise. Deng Yu's work in partial differential equations addresses fundamental questions in kinetic theory and wave dynamics, while John Pardon's advances in symplectic geometry involve virtual fundamental cycles—a tool for counting geometric objects—and the Fukaya category, which organizes Lagrangian submanifolds and is central to mirror symmetry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Virtual_fundamental_class">Virtual fundamental class - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fukaya_category">Fukaya category</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#Fields Medal`, `#award`, `#Chinese mathematicians`, `#breakthrough`

---

<a id="item-2"></a>
## [Anthropic Releases Claude Opus 5, New Flagship Model](https://www.anthropic.com/news/claude-opus-5) ⭐️ 9.0/10

Anthropic has released Claude Opus 5, its latest flagship large language model, featuring enhanced performance and no data retention requirements for general access. This release is significant for enterprises and privacy-conscious users, as it offers cutting-edge AI capabilities without the data retention policies that competitors like Fable require, potentially accelerating adoption in sensitive sectors. Claude Opus 5 does not retain user prompts or outputs for general access, a key differentiator from some other high-performance models. Early benchmarks show it outperforming Fable in image-to-HTML conversion, and it maintains characteristic 'Claude-isms' in writing style.

hackernews · alvis · Jul 24, 16:57 · [Discussion](https://news.ycombinator.com/item?id=49038433)

**Background**: Claude Opus 5 is the latest in Anthropic's Opus line, which focuses on high-performance reasoning and safety. Data retention policies in AI models have become a major concern for enterprises handling sensitive data, as they may store prompts and outputs for training or safety monitoring. Anthropic's stance on zero data retention for Opus models positions it favorably in the enterprise market.

<details><summary>References</summary>
<ul>
<li><a href="https://www-cdn.anthropic.com/c5fbac3f0b1280a933ebd26d3cb8bb9f5bdeaf48/Claude+Opus+5+System+Card.pdf">Claude Opus 5 System Card</a></li>
<li><a href="https://benchlm.ai/models/claude-opus-5">Claude Opus 5 Benchmarks, Pricing & Speed (July 2026) | BenchLM.ai</a></li>
<li><a href="https://kie.ai/blog/what-is-claude-opus-5">What Is Claude Opus 5 ? Anthropic 's Honeycomb Flagship</a></li>

</ul>
</details>

**Discussion**: Community members praised the absence of data retention requirements, with one user calling it the most important feature. A developer testing image-to-HTML reported Opus 5 outperforming Fable in accuracy. Others noted that Opus 5 retains distinct writing quirks from its predecessor, and highlighted the growing need for model routing as AI options proliferate.

**Tags**: `#AI`, `#Large Language Models`, `#Anthropic`, `#Claude`, `#Machine Learning`

---

<a id="item-3"></a>
## [Security camera ships GitHub admin token in login page](https://hhh.hn/hanwha-github-token/) ⭐️ 9.0/10

A Hanwha security camera was discovered to have a GitHub admin token hardcoded in its login page, exposing critical infrastructure. The token could allow unauthorized access to the company's GitHub repositories. This vulnerability highlights severe supply chain risks in IoT devices, as a single hardcoded token could compromise an entire organization's source code and CI/CD pipelines. It underscores the need for better security practices in firmware development. The token was found in the login page's source code, likely intended for internal use but exposed to all users. The camera is by Hanwha, a Korean security product manufacturer, and the incident also revealed US Department of War IP addresses baked into the firmware.

hackernews · hhh · Jul 24, 11:54 · [Discussion](https://news.ycombinator.com/item?id=49034292)

**Background**: GitHub admin tokens are credentials that grant elevated access to GitHub repositories, often used in automated workflows. Hardcoding such tokens in device firmware is a dangerous practice because anyone who inspects the code can extract them. IoT devices are notoriously insecure due to limited resources and lack of security focus by manufacturers. Supply chain attacks can occur when such tokens are leaked, allowing attackers to inject malicious code into software updates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/sysadmin/comments/v0oy13/iot_devices_are_notoriously_insecure_but_why_how/">IoT devices are notoriously insecure, but why, how are they being exploited? - Reddit</a></li>
<li><a href="https://guide.rladies.org/organizers/tech/github-admin-token/index.html">GitHub Admin Token ( ADMIN _ TOKEN ) :: R-Ladies organizational...</a></li>

</ul>
</details>

**Discussion**: Community members expressed concern over the hardcoded token and the presence of US Department of War IP addresses in the firmware. Suggestions included isolating cameras on separate VLANs without internet access and avoiding Korean security products. Some users noted that many IoT vendors ship devices with insecure defaults and hardcoded credentials.

**Tags**: `#security`, `#IoT`, `#vulnerability`, `#supply-chain`, `#github`

---

<a id="item-4"></a>
## [Compiler Transforms Computation Graphs into Transformer Weights without Training](https://www.reddit.com/r/MachineLearning/comments/1v5fxbe/i_built_a_compiler_that_turns_computation_graphs/) ⭐️ 9.0/10

A new compiler, Torchwright, converts arbitrary Python computation graphs directly into the weights of a standard Phi-3-architecture transformer, which can be loaded in Hugging Face without custom code or trust_remote_code. This eliminates the need for any training or fine-tuning. This bridges mechanistic interpretability and practical deployment by allowing researchers to hand-craft transformer weights for specific algorithms without training. It also enables the creation of known-structure models for interpretability experiments, potentially accelerating transformer understanding. The compiler targets the stock Phi-3 architecture, so the output checkpoint is a standard transformer that requires no custom code. Unlike prior work like Tracr, which compiles from a domain-specific language (RASP), Torchwright accepts ordinary Python code defining a computation graph.

reddit · r/MachineLearning · /u/notforrob · Jul 24, 16:15

**Background**: Transformers are neural network architectures widely used in language models, but understanding what algorithms they can represent is an open question. RASP (Restricted Access Sequence Processing Language) was introduced as a programming language to programmatically describe transformer computations, and Tracr compiles RASP programs into transformer weights. Torchwright extends this idea by compiling from ordinary Python and targeting a vanilla architecture, making the outputs immediately usable with standard frameworks.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2106.06981">[2106.06981] Thinking Like Transformers</a></li>
<li><a href="https://github.com/google-deepmind/tracr">google-deepmind/tracr - TRAnsformer Compiler for RASP.</a></li>

</ul>
</details>

**Tags**: `#compilers`, `#transformers`, `#machine-learning`, `#interpretability`, `#mechanistic-interpretability`

---

<a id="item-5"></a>
## [Postgres LISTEN/NOTIFY scales to 60K notifications per second](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 8.0/10

A detailed analysis demonstrates that PostgreSQL's LISTEN/NOTIFY mechanism can handle up to 60,000 notifications per second, challenging the widespread belief that it does not scale. This finding is significant for developers building real-time features on Postgres, as it validates LISTEN/NOTIFY as a viable option for high-throughput asynchronous messaging within the database, potentially reducing reliance on external message brokers. The article provides performance benchmarks showing sustained throughput of 60,000 notifications per second under specific configurations, though scalability may still be limited by factors like transaction commit locking and payload size.

hackernews · KraftyOne · Jul 24, 19:05 · [Discussion](https://news.ycombinator.com/item?id=49040296)

**Background**: PostgreSQL's LISTEN/NOTIFY is a built-in messaging system that allows sessions to subscribe to named channels and receive asynchronous notifications. It is commonly used for triggering cache invalidations or notifying application servers of data changes. However, many developers and posts (e.g., the article 'Postgres LISTEN/NOTIFY does not scale') have warned that it suffers from global lock contention and does not handle high concurrency or volume well.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.recall.ai/blog/postgres-listen-notify-does-not-scale">Postgres LISTEN/NOTIFY does not scale</a></li>
<li><a href="https://medium.com/@diwasb54/real-time-communication-with-postgresql-listen-notify-and-fastapi-0bfedf66be13">Real‑Time Communication with PostgreSQL LISTEN/NOTIFY and FastAPI | by Diwash Bhandari | Software Developer | Medium</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed. Some commenters (e.g., phamilton) share positive experiences pairing LISTEN/NOTIFY with Rust for high-scale subscriptions, while others (e.g., konstmonst) report message loss under high load. Jerf emphasizes that scalability is a continuum, and using a technology with the wrong scaling profile is a common error.

**Tags**: `#postgresql`, `#listen-notify`, `#scalability`, `#databases`, `#async-notifications`

---

<a id="item-6"></a>
## [Software Quality Declines Despite Coding Advancements](https://ptrchm.com/posts/nothing-works-and-everyone-is-euphoric/) ⭐️ 8.0/10

A widely discussed article argues that software quality has been declining, attributing the problem to misaligned incentives and non-technical decision-makers rather than technical limitations. This matters because it highlights a systemic issue in the tech industry where user experience degrades despite powerful tools, affecting millions of users and challenging the narrative of continuous improvement. The article's author recounts personal experiences, such as macOS updates causing dread and Slack stealing focus, to illustrate UX regressions that persist even in major software.

hackernews · pchm · Jul 24, 09:08 · [Discussion](https://news.ycombinator.com/item?id=49033004)

**Background**: The discussion centers on the observation that while programming tools and AI have advanced, everyday software often feels worse. Common explanations include incentives favoring new features over stability, and non-technical managers prioritizing visual changes over usability.

**Discussion**: Community comments strongly agree with the article, with users sharing anecdotes of updates being 'scary' and blaming non-technical 'imposters' for degraded experiences. Others point to incentive structures that reward creating new tools while neglecting maintenance.

**Tags**: `#software quality`, `#user experience`, `#product management`, `#tech industry`, `#UX regression`

---

<a id="item-7"></a>
## [Tech Giants Warn Against Overregulating Open-Weight AI](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 8.0/10

Nvidia, Microsoft, and Meta co-signed a letter urging US policymakers not to overregulate open-weight AI models, arguing that such regulations could stifle innovation and harm American leadership in AI. This unified stance from three major tech companies signals a significant pushback against growing calls for strict AI regulation, potentially shaping future policy. The outcome could determine the balance between open research and closed, proprietary AI development. The letter specifically defends open-weight models—where neural network weight parameters are publicly released—as critical for transparency, security research, and academic progress. It contrasts with positions held by companies like Anthropic and OpenAI, which have advocated for more regulation.

hackernews · louiereederson · Jul 24, 13:32 · [Discussion](https://news.ycombinator.com/item?id=49035303)

**Background**: Open-weight AI models are a category between fully open-source and fully proprietary, where the trained model weights are released but the training code and data may not be. They enable developers to fine-tune and deploy powerful models without full transparency, raising both innovation and safety concerns. The debate has intensified as Chinese open-weight models like DeepSeek have gained global traction, challenging US dominance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=G0SpJa5viiY">What Are Open - Weight AI Models ? Here’s Why They Matter - YouTube</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**Discussion**: Hacker News comments reveal a sharp divide: some users applaud the letter as a necessary check against corporate-driven regulation, while others point out that Anthropic's recent $40M donation to a regulatory pact shows the closed-source lobby may be outgunned. References to the 2026 startup letter and China's open-weight strategy highlight the broader geopolitical context.

**Tags**: `#AI policy`, `#open-weight models`, `#regulation`, `#Nvidia`, `#tech industry`

---

<a id="item-8"></a>
## [IRGC claims destruction of AWS Bahrain data center](https://houseofsaud.com/irgc-claims-destroyed-amazon-bahrain-data-center/) ⭐️ 8.0/10

The Islamic Revolutionary Guard Corps (IRGC) has claimed responsibility for destroying an Amazon Web Services (AWS) data center in Bahrain, part of the me-south-1 region. This claim has sparked debate about its feasibility given AWS's multi-data center design. If true, this would represent a significant physical attack on critical cloud infrastructure, highlighting vulnerabilities in geopolitical conflict zones. It raises urgent questions about redundancy, disaster recovery, and the security of major cloud providers' facilities. AWS regions like me-south-1 are designed with at least three Availability Zones (data centers) located kilometers apart. Community analysis specifically identified data center BAH53 in Manama and a nearby substation that reportedly suffered damage around July 16-22, 2026.

hackernews · thisislife2 · Jul 24, 09:52 · [Discussion](https://news.ycombinator.com/item?id=49033240)

**Background**: AWS data centers employ physical security measures such as restricted access, video surveillance, and intrusion detection. The IRGC, while known for cyber warfare capabilities, also conducts physical operations. This incident underscores the intersection of cyber and physical threats to cloud infrastructure in the Middle East.

<details><summary>References</summary>
<ul>
<li><a href="https://radar.offseq.com/threat/iranian-strikes-on-amazon-data-centers-highlight-i-daf77fd0">Iranian Strikes on Amazon Data Centers Highlight... | OffSeq.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/Islamic_Revolutionary_Guard_Corps_Cyber_Command">Islamic Revolutionary Guard Corps Cyber Command - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/khannaash_leadingintech-cloudresilience-geopoliticalrisk-activity-7434484469023141891-wZB0">AWS Data Center Strikes: Physical Security Threats to... | LinkedIn</a></li>

</ul>
</details>

**Discussion**: Community members expressed skepticism about the claim, noting that an AWS region consists of multiple data centers kilometers apart, making simultaneous destruction difficult. Some pointed out that ATM services in Dubai are still operational, contradicting alleged bank infrastructure outages. Others discussed the importance of disaster planning and the broader implications for AWS's global operations.

**Tags**: `#cloud infrastructure`, `#cybersecurity`, `#AWS`, `#geopolitical risk`, `#data center`

---

<a id="item-9"></a>
## [Buz: Fork of Bun Achieves Sub-Second Incremental Builds](https://ziggit.dev/t/buz-a-drop-in-replacement-for-bun-using-modern-zig-with-sub-1s-incremental-builds/16891) ⭐️ 8.0/10

A developer forked Bun to create Buz, using modern Zig and achieving sub-1s incremental builds. The project uncovered over 11,000 lines of dead code in Bun's codebase and demonstrated potential for much faster build times. This fork demonstrates that Bun could have had fast builds all along, highlighting significant code quality issues. It could inspire improvements in Bun or other Zig-based projects, affecting performance for JavaScript/TypeScript developers. Buz relies on Zig's incremental compilation, but it currently only supports Linux and x86_64, lacking aarch64 support. The fork has also modernized parts of the codebase, fixing numerous bugs.

hackernews · kristoff_it · Jul 24, 09:26 · [Discussion](https://news.ycombinator.com/item?id=49033099)

**Background**: Bun is an all-in-one JavaScript runtime written in Rust, designed as a drop-in replacement for Node.js. Zig is a system programming language focused on robustness and performance, and its incremental compilation feature allows fast rebuilds by only recompiling changed code. Buz is a fork that replaces Rust with Zig for the runtime core.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise at the 11,000 lines of dead code, with some questioning how such neglect occurred. Others noted the irony of using LLMs to clean up code that LLMs may have helped create. The overall sentiment was positive about the technical achievement but skeptical about broader platform support.

**Tags**: `#zig`, `#bun`, `#incremental-builds`, `#performance`, `#fork`

---

<a id="item-10"></a>
## [India orders GitHub to remove Bluetooth chat app Bitchat](https://www.thehindu.com/news/national/government-orders-github-to-remove-bluetooth-based-chat-app-bitchat-over-security-concerns-jack-dorsey/article71262049.ece) ⭐️ 8.0/10

The Indian government has ordered GitHub to remove the open-source Bluetooth-based chat app Bitchat, citing security risks. Jack Dorsey, former Twitter CEO, publicly highlighted this action. This move raises concerns about government overreach in controlling open-source projects and censoring communication tools, potentially undermining developers' trust in GitHub and limiting freedom of speech in India. Bitchat enables encrypted messaging entirely offline over Bluetooth, requiring no phone number or internet, which makes it resistant to surveillance and censorship. The government claims it poses a risk of misuse by terrorists and criminal groups.

hackernews · rootkea · Jul 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=49036433)

**Background**: Bitchat is a peer-to-peer messaging app designed to function without internet access by using Bluetooth for local communication, making it popular in protest movements and regions with internet shutdowns. India has historically taken strict measures to monitor communications, especially after the 2008 Mumbai attacks, including banning satellite phones.

<details><summary>References</summary>
<ul>
<li><a href="https://bitchat.free/">bitchat</a></li>
<li><a href="https://medium.com/@rajinderdevstory/what-is-bitchat-app-a-complete-guide-for-users-and-developers-in-2025-23fda96ebd68">What Is Bitchat App ? A Complete Guide for Users and... | Medium</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some criticize the government's reasoning as a pretext for control, while others note India's security concerns post-Mumbai attacks. There is also discussion about the ongoing protests led by Sonam Wangchuk and the government's broader efforts to block communications.

**Tags**: `#censorship`, `#open-source`, `#government`, `#privacy`, `#India`

---

<a id="item-11"></a>
## [AMD Challenges NVIDIA's CUDA Dominance at Advancing AI 2026](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

AMD announced the Helios rack with Instinct MI455X GPUs and a new Agentic Kernel Generation technique to automate kernel optimization, alongside aggressive pricing strategies including up to 105% discounts via financial engineering. This marks AMD's most comprehensive attempt to break NVIDIA's CUDA moat, combining powerful hardware with software automation and aggressive pricing to lower AI compute costs and challenge NVIDIA's dominance in data centers. The MI455X features 432GB of HBM4 memory and a 2nm process, with peak MXFP8 performance up to 4x the MI355X. The Helios rack costs $5-5.5 million and integrates 72 GPUs. However, AMD faces internal instability in development clusters and production ramp challenges.

rss · Semianalysis · Jul 25, 00:33

**Background**: NVIDIA's CUDA platform has long been the dominant software ecosystem for GPU-accelerated computing, creating a significant barrier for competitors. AMD's ROCm software stack aims to compete but has historically suffered from quality and compatibility issues. Agentic Kernel Generation uses large language models to automatically generate and optimize low-level GPU kernels, reducing manual effort. Financial engineering in this context refers to using complex financial instruments to offer deep discounts, potentially subsidizing hardware to gain market share.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/AMD-Instinct-MI455X-Helios">AMD Launches Instinct MI455X, Helios AI Rack - Phoronix</a></li>
<li><a href="https://www.emergentmind.com/topics/agentic-kernel-generation">Agentic Kernel Generation</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/amd-takes-the-wraps-off-its-instinct-mi455x-ai-accelerator-cdna-5-and-helios-rack-scale-architecture-combine-to-take-the-fight-to-nvidia-in-the-data-center">AMD takes the wraps off its Instinct MI455X AI accelerator — CDNA 5 and Helios rack-scale architecture combine to take the fight to Nvidia in the data center | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#CUDA`, `#AI hardware`, `#software ecosystem`, `#semiconductors`

---

<a id="item-12"></a>
## [OpenAI Releases Enterprise AI Product Presence, Software Stocks Plunge](https://www.businessinsider.com/openai-release-turns-a-bad-week-ugly-for-software-stocks-2026-7) ⭐️ 8.0/10

OpenAI has launched Presence, an enterprise AI agent platform that automates customer support, sales, and internal workflows, directly competing with SaaS vendors. Following the announcement, stocks of major software companies like Workday, Atlassian, HubSpot, and Salesforce dropped significantly. This marks a significant escalation in OpenAI's competition with traditional SaaS providers, as it offers an integrated AI agent solution that could reduce demand for existing SaaS products. The stock market reaction indicates investor concern that SaaS companies may face disruption from AI-native offerings. Presence powers OpenAI's own customer support, resolving 75% of inbound issues without human assistance within weeks, and outperforming frontline human quality. According to TD Cowen analysts, the product integrates AI agent capabilities that SaaS vendors have been promoting, causing the IGV software index to fall about 3% on Wednesday and continue declining.

telegram · zaihuapd · Jul 24, 12:05

**Background**: OpenAI Presence is an enterprise platform that connects AI agents to internal corporate data, policies, existing software, and workflows, enabling automation with human oversight. Traditional SaaS companies like Salesforce and HubSpot have been adding AI features to their products, but OpenAI's direct entry into enterprise automation poses a more direct threat by offering a standalone solution that can replace parts of their offerings.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-openai-presence/">Introducing OpenAI Presence | OpenAI</a></li>
<li><a href="https://www.businessinsider.com/openai-presence-corporate-software-customer-service-sales-2026-7">OpenAI Presence Is About to Take Another Leap Into Corporate Software - Business Insider</a></li>
<li><a href="https://www.nojitter.com/ai-automation/openai-makes-its-presence-felt-in-cx">OpenAI makes its Presence felt in CX</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI产品`, `#SaaS`, `#股市影响`, `#企业AI`

---

<a id="item-13"></a>
## [Telegram Zero-Click Crash Vulnerability Silently Patched](https://x.com/Fried_rice/status/2080200610985689222) ⭐️ 8.0/10

Security researcher Kimi K3 disclosed a zero-click vulnerability that crashes Telegram Desktop and iOS clients via a crafted message, and Telegram Desktop has been silently patched. This zero-click vulnerability poses a serious risk as it requires no user interaction, making it easy to exploit for denial-of-service or potentially further attacks on a widely-used messaging app. The vulnerability affects Telegram Desktop and iOS; a test bot (@kimifuckingbot) is available to verify the crash. Telegram's update log did not mention the fix, making it a silent patch.

telegram · zaihuapd · Jul 24, 15:06

**Background**: Zero-click attacks exploit vulnerabilities that require no action from the victim, such as opening a message. Telegram is a popular messaging app with end-to-end encryption, but clients can still have bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://endersinsurance.com/blog/cyber-bytes-what-is-a-zero-click-attack/">Cyber Bytes: What Is a Zero-Click Attack? - Enders Insurance</a></li>

</ul>
</details>

**Discussion**: No community comments were provided in the news source. The post urges immediate updates and warns against using unofficial Telegram clients.

**Tags**: `#security`, `#vulnerability`, `#telegram`, `#zero-click`, `#update`

---

<a id="item-14"></a>
## [Ctrip unit fined $1.4M for illegal data exports](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

Shanghai Ctrip Business Company was fined 10 million yuan by the Shanghai Cyberspace Administration for failing to comply with data export security assessment requirements and illegally transferring personal data abroad. The company has since cooperated and taken corrective actions. This enforcement action highlights China's strict enforcement of cross-border data transfer regulations, serving as a warning to all businesses operating in China to ensure compliance with data export security assessment obligations. It signals that regulators are actively monitoring and penalizing violations in the consumer sector. The fine was announced on June 13, 2024, and the company has since implemented corrective measures. The case underscores that the government is intensifying enforcement against enterprises that illegally transfer personal data abroad, particularly in sectors closely related to people's livelihoods.

telegram · zaihuapd · Jul 25, 02:24

**Background**: China's Personal Information Protection Law (PIPL) and related regulations require companies that transfer personal data abroad to undergo a security assessment by the Cyberspace Administration. The measures for security assessment of cross-border data transfers, effective September 1, 2022, specify conditions triggering the assessment, such as the volume and sensitivity of data. This fine is one of the first major enforcement actions under these rules, demonstrating the government's commitment to data sovereignty and user privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.china-briefing.com/news/cross-border-data-transfer-new-measures-offer-clarification-on-security-review/">Cross-Border Data Transfer - New Measures for Security Review</a></li>

</ul>
</details>

**Tags**: `#data privacy`, `#regulation`, `#China`, `#data export`, `#fine`

---

<a id="item-15"></a>
## [Qualcomm announces across-the-board price hike starting September 1](https://tw.news.yahoo.com/%E7%8D%A8%E5%AE%B6-%E9%AB%98%E9%80%9A%E6%BC%B2%E5%83%B9%E4%BF%A1%E6%9B%9D%E5%85%89-%E5%85%A8%E7%B7%9A%E7%94%A2%E5%93%819-1%E8%B5%B7%E8%AA%BF%E6%BC%B2-%E7%9B%B4%E8%A8%80-142730846.html) ⭐️ 8.0/10

On July 24, 2026, Qualcomm notified customers that it will raise prices on all products shipped on or after September 1, citing rising costs in wafer fabrication, packaging, testing, advanced packaging, substrate materials, and capacity constraints from AI and data center demand. This price increase affects a wide range of products including smartphones, PCs, IoT devices, and automotive chips, and could lead to higher consumer prices or reduced product features. It reflects a structural shift in semiconductor manufacturing costs driven by AI demand. Qualcomm did not disclose a uniform increase percentage or specific product models; instead, account managers will contact customers individually with new quotes. Some orders already placed but scheduled for shipment after September may also be re-quoted.

telegram · zaihuapd · Jul 25, 03:01

**Background**: Advanced packaging refers to techniques like 2.5D/3D IC integration, fan-out wafer-level packaging, and chip-on-wafer-on-substrate (CoWoS) that combine multiple dies or chiplets in a single package, improving performance and reducing signal paths. Substrate materials, such as ABF (Ajinomoto Build-Up Film) or ceramic substrates, provide the base for mounting chips and interconnects. Rising demand for AI accelerators and data center chips has strained advanced packaging and substrate capacity, contributing to cost increases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_packaging_(semiconductors)">Advanced packaging (semiconductors)</a></li>
<li><a href="https://hilelectronic.com/semiconductor-substrate/">Semiconductor Substrate vs PCB: Key Differences Explained</a></li>
<li><a href="https://pcbmake.com/chip-substrate-material/">Chip Substrate Material : Enhancing Semiconductor Design</a></li>

</ul>
</details>

**Tags**: `#Qualcomm`, `#chip pricing`, `#semiconductor industry`, `#supply chain`

---