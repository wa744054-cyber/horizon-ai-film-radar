---
layout: default
title: "Horizon Summary: 2026-07-21 (EN)"
date: 2026-07-21
lang: en
---

> From 41 items, 16 important content pieces were selected

---

1. [Chinese Open-Source AI Models Challenge US Dominance](#item-1) ⭐️ 9.0/10
2. [High-risk RCE in Fastjson 1.x without gadgets](#item-2) ⭐️ 9.0/10
3. [US Tech Giants' Hidden AI Debts Reach $1.65 Trillion](#item-3) ⭐️ 8.0/10
4. [AI Outcounterexamples Human Mathematicians](#item-4) ⭐️ 8.0/10
5. [Cursor Scales AI Agent Swarms to 1000 Commits per Second](#item-5) ⭐️ 8.0/10
6. [Corners Don't Look Like That: A Critique of SSAO](#item-6) ⭐️ 8.0/10
7. [AI Writing on arXiv Spikes to 39% by 2026; Detector Reliability Questioned](#item-7) ⭐️ 8.0/10
8. [Perfection Is Not Over-Engineering](#item-8) ⭐️ 8.0/10
9. [Hacker wipes Romania's land registry database](#item-9) ⭐️ 8.0/10
10. [US Law Proposed to Level AI Playing Field with China](#item-10) ⭐️ 8.0/10
11. [Hugging Face Reveals AI Agent Attack, Commercial LLMs Refuse Forensics](#item-11) ⭐️ 8.0/10
12. [Trump Administration May Limit US Use of Chinese AI Models](#item-12) ⭐️ 8.0/10
13. [US Military Apps Found to Contain Chinese and Russian Code](#item-13) ⭐️ 8.0/10
14. [EU Proposed to Share Biometric Data with US for Visa Waiver](#item-14) ⭐️ 8.0/10
15. [Zhipu Completes 1GW Data Center with All-Chinese Chips](#item-15) ⭐️ 8.0/10
16. [Cloudflare Internal DNS Service Launches](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Chinese Open-Source AI Models Challenge US Dominance](https://stratechery.com/2026/whos-afraid-of-chinese-models/) ⭐️ 9.0/10

Chinese open-source AI models, such as Alibaba's Qwen and DeepSeek V4 Pro, are undercutting the pricing strategies of US frontier labs like OpenAI and Anthropic by releasing high-performance models for free. This threatens the enormous valuations of these labs, which were based on premium API pricing. This competition could force US labs to cut prices, benefiting consumers and accelerating AI adoption, but it also jeopardizes the return expectations of venture capital investors. The trend underscores a shift toward open-source AI, potentially reshaping global market leadership. Notable Chinese models include DeepSeek V4 Pro, Qwen 3.7, and Kimi K2.7, which rival proprietary US models in benchmarks. However, user stickiness varies: some find it easy to switch between coding tools like Claude Code and Codex, while others report high switching costs.

hackernews · mfiguiere · Jul 20, 11:05 · [Discussion](https://news.ycombinator.com/item?id=48977128)

**Background**: Frontier AI labs are companies at the forefront of artificial intelligence development, requiring massive compute resources and funding. Open-source AI models, in contrast, are freely available for anyone to use, modify, and distribute, lowering barriers to entry. The Chinese open-source ecosystem has rapidly advanced, with models now competitive on global leaderboards.

<details><summary>References</summary>
<ul>
<li><a href="https://techblog.comsoc.org/2026/01/27/chinas-open-source-ai-models-to-capture-a-larger-share-of-2026-global-ai-market/">China’s open source AI models to capture a larger share of ...</a></li>
<li><a href="https://www.aimadetools.com/blog/best-chinese-open-source-ai-models-june-2026/">Best Chinese Open-Source AI Models June 2026: Pangu, DeepSeek ...</a></li>
<li><a href="https://techwireasia.com/2025/07/china-open-source-ai-models-global-rankings/">China open-source AI models dominate global rankings</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that VCs are most afraid due to high valuations built on premium pricing, while some users find switching between coding tools easy, contradicting the article's stickiness claim. Others note observations of Chinese datacenter buildouts, suggesting long-term infrastructure investment.

**Tags**: `#AI`, `#Chinese AI models`, `#OpenAI`, `#Anthropic`, `#open-source`

---

<a id="item-2"></a>
## [High-risk RCE in Fastjson 1.x without gadgets](https://x.com/k_firsov/status/2078872293745570032) ⭐️ 9.0/10

A high-risk remote code execution vulnerability was disclosed in Fastjson 1.x versions 1.2.68 to 1.2.83, exploitable without enabling autoTypeSupport or relying on classpath gadgets, affecting JDK 8/17/21. This vulnerability is critical because Fastjson 1.x is widely used and no longer maintained, leaving no official patch; users must urgently migrate to Fastjson2 or enable SafeMode to prevent exploitation. The attack works on default configurations without requiring autoTypeSupport enabled, and the vulnerability affects the last supported branch (1.x) which reached end-of-life in October 2024.

telegram · zaihuapd · Jul 20, 14:32

**Background**: Fastjson is a popular JSON processing library for Java. Gadgets refer to classes in the classpath that can be chained to achieve code execution during deserialization. Previous Fastjson exploits required specific gadgets and often autoTypeSupport enabled; this new flaw bypasses both, making it easier to exploit.

<details><summary>References</summary>
<ul>
<li><a href="https://foojay.io/today/explaining-java-deserialization-vulnerabilities-part-2/">Explaining Java Deserialization Vulnerabilities (Part 2) | foojay</a></li>
<li><a href="https://topic.alibabacloud.com/a/com-alibaba-fastjson-jsonexception-autotype-is-not-support-_1_27_32615398.html">Com. alibaba. fastjson . JSONException: autoType is not support</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson _ safemode _en · alibaba/ fastjson Wiki · GitHub</a></li>

</ul>
</details>

**Tags**: `#security`, `#rce`, `#fastjson`, `#java`, `#vulnerability`

---

<a id="item-3"></a>
## [US Tech Giants' Hidden AI Debts Reach $1.65 Trillion](https://asia.nikkei.com/business/technology/five-us-tech-giants-hidden-debts-soar-to-1.65tn-on-opaque-ai-funding) ⭐️ 8.0/10

An investigative report reveals that five major US tech companies have accumulated $1.65 trillion in off-balance-sheet debts through opaque financing structures to fund AI infrastructure. This hidden leverage could pose systemic financial risks, as banks and non-bank investors are exposed to potential defaults if AI revenue fails to materialize. The debts are held by special purpose vehicles (SPVs) that own the data centers, with the tech giants having long-term leasing commitments rather than direct ownership.

hackernews · NordStreamYacht · Jul 21, 03:56 · [Discussion](https://news.ycombinator.com/item?id=48987863)

**Background**: Off-balance-sheet financing allows companies to keep certain liabilities off their balance sheets, often through SPVs or leasing arrangements. This practice can improve financial ratios but obscures true leverage. The AI infrastructure boom has led to massive capital expenditures, and tech giants have used these structures to fund data centers without directly increasing their reported debt.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bis.org/publ/qtrpdf/r_qt2603u.htm">Financing the AI infrastructure boom: on- and off-balance ...</a></li>
<li><a href="https://www.investopedia.com/terms/o/obsf.asp">Off-Balance Sheet Financing: Practices, Impacts, and Legal ... Understanding Off-Balance Sheet Activities: Types and Key ... Off-balance-sheet - Wikipedia Off-Balance Sheet Financing: Definition, Benefits, and Risks ... Section 3.8 Off-Balance Sheet Activities - FDIC What is Off-Balance Sheet Financing? Definition, Structure ...</a></li>

</ul>
</details>

**Discussion**: Commenters debate the risk distribution: some argue that the debt is held by SPVs and banks bear the risk, while others are fatalistic about inevitable losses. One commenter suggests government bailouts if AI is deemed critical like the Manhattan Project.

**Tags**: `#AI funding`, `#tech giants`, `#financial risk`, `#investigative journalism`

---

<a id="item-4"></a>
## [AI Outcounterexamples Human Mathematicians](https://xenaproject.wordpress.com/2026/07/20/human-mathematicians-are-being-outcounterexampled/) ⭐️ 8.0/10

AI language models are now being used to generate counterexamples to mathematical conjectures, potentially saving human mathematicians significant time and effort. This development could dramatically accelerate mathematical research by automatically disproving false conjectures, freeing mathematicians to focus on provable results. The discussion highlights the historical importance of counterexamples, referencing the Jacobian conjecture case where an error in a corollary led to years of wasted effort, and the classic book 'Proofs and Refutations' by Imre Lakatos.

hackernews · artninja1988 · Jul 20, 19:03 · [Discussion](https://news.ycombinator.com/item?id=48983382)

**Background**: In mathematics, a conjecture is a statement believed to be true but unproven. Counterexamples are cases that disprove a conjecture, often leading to refined definitions or new theories. Historically, finding counterexamples required deep insight or exhaustive search.

**Discussion**: Commenters broadly welcome the development, noting it saves time and effort, with one sharing the cautionary tale of Yitang Zhang's wasted years. Another recommends the book 'Proofs and Refutations' and remarks that AI-generated counterexamples could become a new tool, though some wonder about the human champion.

**Tags**: `#AI`, `#mathematics`, `#counterexamples`, `#research methodology`, `#machine learning`

---

<a id="item-5"></a>
## [Cursor Scales AI Agent Swarms to 1000 Commits per Second](https://cursor.com/blog/agent-swarm-model-economics) ⭐️ 8.0/10

Cursor detailed a new system where AI agent swarms achieve 1000 commits per second, a 3600x speedup over their previous browser swarm, using a custom version control system built from scratch. The system was tested on building SQLite in Rust from documentation alone. This extreme scaling demonstrates the potential for massively parallel AI-driven software development, challenging existing assumptions about the cost and speed of AI-assisted coding. It raises important questions about the economics of using large swarms of AI agents and the necessary infrastructure changes. The custom VCS handles collisions and coordination at the version control layer, enabling 1000 commits per second vs. the old system's 1000 per hour. The task of building SQLite in Rust from documentation raised concerns among commenters about potential training data contamination from existing Rust SQLite implementations.

hackernews · jlaneve · Jul 20, 18:06 · [Discussion](https://news.ycombinator.com/item?id=48982535)

**Background**: AI agent swarms involve multiple autonomous AI agents collaborating on tasks like code generation, often coordinated by a central system. Traditional version control systems like Git struggle with the high throughput and coordination needs of such swarms, prompting the development of specialized VCS for agents. The economics of AI coding agents considers the cost of model inference versus developer productivity, which becomes critical at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://relevanceai.com/learn/agent-swarms-orchestrating-the-future-of-ai-collaboration">What is an AI Agent Swarm - Relevance AI</a></li>
<li><a href="https://www.freestyle.sh/blog/engineering/version-control-for-ai-agents">Version Control for AI Agents - Freestyle Blog</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about the experimental nature, comparing it to early 2023 discussions about coding agents when only tab completion existed. Some questioned whether the SQLite-in-Rust task was unfairly testing memorization rather than reasoning, due to potential training data overlap. Others suggested that a single-thread agent with smart context management might be more practical than large swarms.

**Tags**: `#AI agents`, `#swarm intelligence`, `#version control`, `#software engineering`, `#coding automation`

---

<a id="item-6"></a>
## [Corners Don't Look Like That: A Critique of SSAO](https://nothings.org/gamedev/ssao/) ⭐️ 8.0/10

Sean Barrett's 2012 article criticizes screenspace ambient occlusion (SSAO) for producing unrealistic corner shading, using real-world photographs to demonstrate that actual corners do not darken the way SSAO renders them. This critique highlights the trade-off between performance and realism in real-time rendering, sparking ongoing debate about whether visual appeal should prioritize accuracy or artistic style. It remains relevant as SSAO artifacts still appear in modern games, and newer techniques like ray tracing aim to address these limitations. The article provides photographic evidence from real scenes showing that corners in reality are often brighter near the edge due to light bouncing, whereas SSAO darkens them incorrectly. It also notes that SSAO can cause halos and other artifacts, especially in convex corners or near thin geometry.

hackernews · firephox · Jul 20, 15:07 · [Discussion](https://news.ycombinator.com/item?id=48979931)

**Background**: Screen Space Ambient Occlusion (SSAO) is a real-time rendering technique developed by Crytek in 2007, first used in the game Crysis to approximate ambient occlusion. It works by sampling the depth buffer around each pixel to estimate occlusion, but it is a coarse approximation and can produce artifacts like corner darkening. SSAO was widely adopted due to its low performance cost compared to more accurate methods like ray tracing.

<details><summary>References</summary>
<ul>
<li><a href="https://nothings.org/gamedev/ssao/">Corners Don't Look Like That: Regarding Screenspace Ambient Occlusion</a></li>
<li><a href="https://en.wikipedia.org/wiki/Screen_space_ambient_occlusion">Screen space ambient occlusion</a></li>
<li><a href="https://mtnphil.wordpress.com/2013/06/26/know-your-ssao-artifacts/">Know your SSAO artifacts | IceFall Games</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the critique while noting that realism is not always the primary goal; visual appeal and readability of geometry often matter more. Some point out that SSAO was the best performing option for years and newer techniques like FidelityFX CACAO and ray tracing offer better quality. A developer expresses appreciation for the photographic benchmark and shares their experience implementing AO.

**Tags**: `#computer graphics`, `#game rendering`, `#ambient occlusion`, `#technical critique`, `#real-time rendering`

---

<a id="item-7"></a>
## [AI Writing on arXiv Spikes to 39% by 2026; Detector Reliability Questioned](https://unslop.run/blog/measuring-ai-writing-on-arxiv) ⭐️ 8.0/10

A new analysis measured AI-written content on arXiv from 2021 to 2026, finding that by January 2026, 39% of papers were flagged as machine-written, with computer science reaching 65%. The study also highlights significant limitations in detector reliability, raising concerns about false positives and methodological biases. This trend underscores the rapid adoption of AI in academic writing, particularly in computer science, and poses challenges to peer review and academic integrity. The detector's reported inaccuracies, such as false positives on pre-LLM papers, also highlight the need for more robust and transparent detection methods. The detector was specifically tuned to minimize false positives, yet pre-ChatGPT detection rates were 0.4%. The analysis combined three separate detector scores, but the methodology for the final join was not publicly available, making reproducibility difficult.

hackernews · dopamine_daddy · Jul 20, 16:36 · [Discussion](https://news.ycombinator.com/item?id=48981206)

**Background**: arXiv is a preprint repository widely used in physics, mathematics, computer science, and related fields. AI writing detection tools analyze text patterns to identify content generated by large language models (LLMs) like ChatGPT. However, no detection method is 100% accurate, and false positives can occur, especially on technical or formulaic writing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://undetectable.ai/blog/how-to-detect-ai-writing-guide/">How to Detect AI Writing in 2025: Full Guide</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the detector's accuracy. One user uploaded pre-LLM papers and received high AI scores (27% to 74%), questioning whether they wrote like an LLM or the LLM learned from them. Another criticized the lack of source code and potential biases in the combined detector scores.

**Tags**: `#AI detection`, `#arXiv`, `#academic integrity`, `#language models`, `#data analysis`

---

<a id="item-8"></a>
## [Perfection Is Not Over-Engineering](https://var0.xyz/posts/perfection-is-not-over-engineering.html) ⭐️ 8.0/10

A blog post argues that perfection is distinct from over-engineering, challenging the common dismissal of perfection in software development as leading to poor outcomes. This article sparks a valuable debate on engineering philosophy, encouraging developers to reconsider the balance between quality and pragmatism, which can affect code quality and team dynamics. The author defines perfection as meeting stringent requirements precisely, while over-engineering is solving the wrong problem or optimizing for non-existent constraints. The post includes a nuanced framework for distinguishing between the two.

hackernews · var0xyz · Jul 20, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48979120)

**Background**: In software engineering, the phrase 'perfect is the enemy of good' is often used to discourage over-engineering and encourage shipping quickly. However, critics argue this mindset can lead to mediocre or even harmful software. This blog post reframes the debate by distinguishing genuine perfection from wasteful over-engineering.

**Discussion**: Commenters express mixed views: some support the pushback against dismissing perfection, noting that 'good enough' often leads to poor software. Others caution that striving for perfection can cause over-engineering and emotional baggage, and that the phrase is used to avoid covering rare edge cases.

**Tags**: `#software engineering`, `#over-engineering`, `#perfectionism`, `#engineering philosophy`, `#hackernews discussion`

---

<a id="item-9"></a>
## [Hacker wipes Romania's land registry database](https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/) ⭐️ 8.0/10

A hacker infiltrated and wiped Romania's entire land registry database, but officials may have had offline backups and are migrating applications to the government cloud. This attack threatens the integrity of land ownership records, which could cause widespread legal and economic chaos if data is not recoverable; it also highlights vulnerabilities in national critical infrastructure. Officials restored the website and are rebuilding the network from scratch, claiming an offline copy exists; they are migrating to Romania's Government Cloud, coordinated by the Special Telecommunications Service (STS), with completion expected by July 22.

hackernews · speckx · Jul 20, 13:28 · [Discussion](https://news.ycombinator.com/item?id=48978605)

**Background**: A land registry database is a national record of property ownership used for legal transactions, taxation, and planning. Wiping it could paralyze real estate deals and government services. Offline backups are critical for recovery after such ransomware-like attacks.

**Discussion**: Comments note that the agency likely had offline backups, avoiding societal chaos; some speculate the attack stems from corruption in IT contracts, and security firm KELA doxxed the hacker as Zakaria Mahdjoub from Algeria, which has an extradition treaty with Romania.

**Tags**: `#cybersecurity`, `#database breach`, `#Romania`, `#land registry`, `#hacktivism`

---

<a id="item-10"></a>
## [US Law Proposed to Level AI Playing Field with China](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

Ben Thompson proposed that the U.S. pass a law making training data collection fair use and prohibiting terms of service that forbid model distillation, aiming to help U.S. open models compete with Chinese counterparts. Additionally, Alibaba released Qwen 3.8 Max, a 2.4 trillion parameter open-weight model, possibly influenced by Xi Jinping’s call for open-source collaboration. This proposal directly addresses the hypocrisy of AI labs that restrict distillation while training on unlicensed data, and could fundamentally reshape U.S.-China AI competition by fostering innovation through open access. If enacted, it would strengthen the U.S. open-source AI ecosystem against China's rapidly advancing models like Qwen and Kimi. Qwen 3.8 Max has 2.4 trillion parameters, nearly as large as Kimi K3's 2.8 trillion, and was released as open weights after Xi Jinping's speech encouraging open source. Thompson's proposal also includes indemnifying labs against copyright liability for training data, ensuring that what they learn fuels further innovation.

rss · Simon Willison · Jul 20, 17:09

**Background**: Model distillation transfers knowledge from a large model to a smaller one by querying the larger model's API, but many AI companies prohibit it in their terms of service. Fair use in U.S. copyright law determines when copyrighted material can be used without permission, and recent court cases like Bartz v. Anthropic are testing its application to AI training. Open-weight models release the trained parameters publicly, allowing anyone to download and run them, but are not fully open source.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.skadden.com/insights/publications/2025/05/copyright-office-report">Copyright Office Weighs In on AI Training and Fair Use | Skadden, Arps, Slate, Meagher & Flom LLP</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#copyright`, `#distillation`, `#open source`, `#US-China competition`

---

<a id="item-11"></a>
## [Hugging Face Reveals AI Agent Attack, Commercial LLMs Refuse Forensics](https://huggingface.co/blog/security-incident-july-2026) ⭐️ 8.0/10

Hugging Face disclosed a July 2026 security incident where attackers used an autonomous AI agent framework to exploit two code execution vulnerabilities in its data processing pipeline, stealing internal datasets and service credentials. The attack performed tens of thousands of operations over a weekend. This is the first publicly documented case where an AI agent framework was used to automate a sophisticated multi-step intrusion on a major AI platform. It highlights both the offensive potential of agentic AI and the risk that commercial LLM safety guardrails can hinder legitimate security forensics. The vulnerabilities were in data processing pipelines. Hugging Face confirmed no tampering with public models, datasets, or Spaces. For forensics, Hugging Face initially used commercial LLM APIs but hit safety guardrails, so they switched to locally deployed GLM 5.2 to analyze over 17,000 attack records.

telegram · zaihuapd · Jul 20, 10:41

**Background**: Hugging Face is a leading platform for hosting machine learning models, datasets, and AI applications. AI agent frameworks allow LLMs to autonomously execute multi-step tasks, which attackers can weaponize. GLM 5.2 is an open-source large language model developed by Z.ai (formerly Zhipu AI), released under MIT License since July 2025, capable of handling long contexts and coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_5.2">GLM 5.2</a></li>
<li><a href="https://yeasy.gitbook.io/agentic_ai_guide/di-si-bu-fen-wei-lai-zhan-wang/11_future/11.1_security">11.1 安全边界：提示词注入与防御策略 | 智能体AI 权威指南 | Agentic AI Guide</a></li>

</ul>
</details>

**Tags**: `#安全事件`, `#AI智能体`, `#代码执行漏洞`, `#大模型安全`, `#Hugging Face`

---

<a id="item-12"></a>
## [Trump Administration May Limit US Use of Chinese AI Models](https://www.axios.com/2026/07/20/ai-us-china-open-source-kimi) ⭐️ 8.0/10

Axios reported that the Trump administration is considering new restrictions to discourage US companies from using cost-effective Chinese open-weight AI models like Kimi K3, citing insider sources. This move could reshape global AI access and competition, potentially limiting the open-source AI ecosystem's diversity and raising costs for US firms. The restrictions would likely be soft enforcement through procurement rules and entity list threats rather than an outright ban, as noted by a White House AI advisor who criticized OpenAI and Anthropic for seeking to eliminate open-source competitors.

telegram · zaihuapd · Jul 20, 11:49

**Background**: Open-weight models like Kimi K3 allow developers to download, run, and modify the AI, unlike proprietary models from OpenAI or Anthropic. Chinese startup Moonshot AI recently launched Kimi K3, claiming it rivals leading US models at lower cost. The US government has previously warned about risks of Chinese AI models but enforcement was blocked by pro-deregulation officials.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.forbes.com/sites/tylerroush/2026/07/17/chinese-ai-startup-moonshot-unveils-kimi-k3-model-will-it-challenge-openai-and-anthropic/">Should You Try Kimi K 3 ? Here’s How AI Model Compares With...</a></li>
<li><a href="https://www.youtube.com/watch?v=6-ccuwX4gCQ">Chinese AI Startup Moonshot Unveils Kimi K 3 Model - YouTube</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#open-source AI`, `#AI regulation`, `#US-China relations`, `#language models`

---

<a id="item-13"></a>
## [US Military Apps Found to Contain Chinese and Russian Code](https://www.wired.com/story/apps-marketed-to-us-troops-are-shipping-chinese-and-russian-code/) ⭐️ 8.0/10

Researchers at Purdue University and other institutions found that nearly two-thirds of over 220 apps marketed to U.S. military personnel contain third-party code from China, Russia, and other countries, including the Huawei SDK. This poses a significant national security risk because the embedded third-party code, such as the Huawei SDK, could be remotely updated and activated to spy on or disrupt military operations, compromising the security of U.S. troops. The research surveyed 103 military-affiliated individuals, and 76-83% expressed extreme unease about apps containing code from China, Russia, Iran, or North Korea. Although no data was observed flowing to Huawei servers yet, the SDK can be updated remotely, posing a latent threat.

telegram · zaihuapd · Jul 20, 13:42

**Background**: Third-party SDKs are software libraries that provide common functionalities to app developers, but they can also introduce security risks if not properly vetted. Huawei has been designated a national security threat by the U.S. government, and its SDK is subject to scrutiny. Supply chain security in mobile apps is a growing concern, as apps often rely on code from multiple external sources that may not be trustworthy.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.huawei.com/consumer/en/">HUAWEI Developers</a></li>
<li><a href="https://www.reflectiz.com/blog/supply-chain-anz/">Web Supply Chain Security in ANZ – Reflectiz</a></li>

</ul>
</details>

**Tags**: `#supply chain security`, `#national security`, `#mobile apps`, `#Huawei`, `#espionage`

---

<a id="item-14"></a>
## [EU Proposed to Share Biometric Data with US for Visa Waiver](https://edri.org/our-work/the-eu-is-about-to-sell-our-most-sensitive-data-to-the-us-for-visa-free-travel/) ⭐️ 8.0/10

The European Commission is negotiating an Enhanced Border Security Partnership (EBSP) framework agreement with the US, which would require the EU to share biometric data from member states' databases in exchange for US visa-free travel for EU citizens. This deal could set a precedent for large-scale data sharing between democratic governments, potentially undermining privacy rights and enabling surveillance of political dissenters and activists. A leaked draft indicates the EU has largely accepted US demands for unrestricted access to biometric data, including 'risk indicators' based on political views, which could threaten freedom of expression.

telegram · zaihuapd · Jul 20, 15:08

**Background**: The Visa Waiver Program (VWP) allows citizens of certain countries to travel to the US without a visa for up to 90 days. Since 2022, the US has required VWP partner countries to establish an EBSP with the Department of Homeland Security, which includes sharing traveler information. The EU is now negotiating such an agreement, but critics argue it goes too far by demanding access to biometric databases and risk indicators.

<details><summary>References</summary>
<ul>
<li><a href="https://eur-lex.europa.eu/eli/dec/2025/2640/oj/eng">Decision - EU - 2025/2640 - EN - EUR-Lex</a></li>
<li><a href="https://www.dhs.gov/sites/default/files/2024-04/24_0429_priv_pia-dhs-all-095b.pdf">Privacy Impact Assessment Update - Homeland Security</a></li>
<li><a href="https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex:52025PC0447">EUR-Lex - 52025PC0447 - EN - EUR-Lex</a></li>

</ul>
</details>

**Tags**: `#biometric data`, `#privacy`, `#EU-US relations`, `#surveillance`, `#visa waiver`

---

<a id="item-15"></a>
## [Zhipu Completes 1GW Data Center with All-Chinese Chips](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 8.0/10

Zhipu AI (Z. AI) has completed construction of a 1-gigawatt data center that uses exclusively Chinese-made chips, and has begun partial operation. The facility will support the training of the company's GLM AI model. This milestone demonstrates China's ability to build large-scale AI infrastructure without relying on restricted Nvidia chips, advancing the country's goal of AI self-sufficiency. It also positions Z. AI as a major player in the global AI race with a domestic supply chain. The data center has a power capacity of 1 GW, enough to power roughly 750,000 homes simultaneously. Z. AI currently operates multiple computing clusters each with over 10,000 chips, and this facility is among the largest built by a Chinese AI lab.

telegram · zaihuapd · Jul 20, 15:43

**Background**: Z. AI (formerly Zhipu AI) is a Chinese AI company behind the GLM series of large language models, including ChatGLM. Due to US export restrictions on advanced Nvidia chips, Chinese AI firms have sought domestic alternatives from companies like Huawei (Ascend series). However, many have been hesitant due to performance gaps. This data center represents a large-scale deployment of domestic chips for AI training.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai">Z. AI Completes Giant Data Center With Chinese Chips ... - Bloomberg</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI) - Wikipedia</a></li>
<li><a href="https://www.rand.org/pubs/commentary/2025/08/leashing-chinese-ai-needs-smart-chip-controls.html">Leashing Chinese AI Needs Smart Chip Controls | RAND</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Chinese Chips`, `#Data Center`, `#Infrastructure`, `#GLM`

---

<a id="item-16"></a>
## [Cloudflare Internal DNS Service Launches](https://blog.cloudflare.com/internal-dns/) ⭐️ 8.0/10

On July 20, 2026, Cloudflare officially launched its Internal DNS service, providing authoritative and recursive DNS resolution for enterprise private networks, integrated with Zero Trust and the same global network as its public DNS and Gateway. This service simplifies split-horizon DNS management by merging public and private DNS into a single platform, and extends Zero Trust policies to the DNS resolution layer, enhancing enterprise network security and reducing configuration complexity. Existing Cloudflare Gateway customers can use Internal DNS at no additional cost. It supports API, Terraform, and Cloudflare WAN as deployment methods, and allows administrators to define resolver policies controlling which internal views different users and devices can access.

telegram · zaihuapd · Jul 21, 03:49

**Background**: Split-horizon DNS (also known as split-view DNS) provides different DNS responses based on the source address, allowing internal and external users to see different DNS records for the same domain. Cloudflare Gateway is a cloud-native Secure Web Gateway (SWG) that inspects DNS, HTTP, and other traffic as part of Cloudflare's Zero Trust platform. Internal DNS brings these capabilities together, offering a unified control plane for both public and private DNS resolution with built-in Zero Trust enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/gateway/">Secure Web Gateway - Cloudflare</a></li>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>

</ul>
</details>

**Tags**: `#DNS`, `#Cloudflare`, `#Zero Trust`, `#Networking`, `#Security`

---