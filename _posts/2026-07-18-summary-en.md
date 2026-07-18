---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 39 items, 15 important content pieces were selected

---

1. [Huawei Ascend 950 Super Node Debuts, Claims 6.7x NVIDIA Performance](#item-1) ⭐️ 9.0/10
2. [Moonshot AI Releases Open-Source 2.8T Parameter Kimi K3 Model](#item-2) ⭐️ 9.0/10
3. [US Considers FINRA-like Watchdog for Top AI Models](#item-3) ⭐️ 9.0/10
4. [First atmosphere on Earth-like planet LHS 1140b confirmed by JWST](#item-4) ⭐️ 8.0/10
5. [Kimi K3 and the Pelican Benchmark: Training Data Debate](#item-5) ⭐️ 8.0/10
6. [Open source AI models surge in market share](#item-6) ⭐️ 8.0/10
7. [FAA reinstates Boeing's self-certification for 737 MAX and 787](#item-7) ⭐️ 8.0/10
8. [Three Non-Solving Responses to Problems Analyzed](#item-8) ⭐️ 8.0/10
9. [Live SSH Honeypot Visualization Shows Bot Attacks in Real Time](#item-9) ⭐️ 8.0/10
10. [Prism Bug Leaks Researchers' Papers](#item-10) ⭐️ 8.0/10
11. [US Lawmakers Urge Ban on Chinese Memory Chips in Allied Supply Chains](#item-11) ⭐️ 8.0/10
12. [OpenAI CFO Proposes 'Useful Intelligence Per Dollar' Metric for AI ROI](#item-12) ⭐️ 8.0/10
13. [Meta Negotiates $100B AI Compute Lease with Anthropic](#item-13) ⭐️ 8.0/10
14. [Spacex in Talks for Pentagon AI Compute Deal](#item-14) ⭐️ 8.0/10
15. [TSMC Announces A14 Process for 2028 Production](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Huawei Ascend 950 Super Node Debuts, Claims 6.7x NVIDIA Performance](https://www.ithome.com/0/978/019.htm) ⭐️ 9.0/10

Huawei publicly demonstrated the Ascend 950 SuperPoD (Atlas 950) for the first time at WAIC 2026, claiming it delivers 1 EFLOPS FP8 and 2 EFLOPS FP4 compute power with 256 TB unified memory across 1024 cards, achieving 6.7 times the total compute of NVIDIA's 144-card NVL144 system per a China Securities report. This marks a major milestone in AI chip competition between China and the US, potentially reshaping the large-scale AI training infrastructure landscape and reducing reliance on NVIDIA hardware for Chinese enterprises. The Ascend 950 uses Huawei's proprietary Lingqu (UnifiedBus) interconnect protocol and super node architecture, supporting up to 1024 cards without network convergence. Additionally, the earlier Ascend 384 SuperPoD has been commercially deployed in over 750 units across internet, telecom, and finance sectors.

telegram · zaihuapd · Jul 17, 10:27

**Background**: Super nodes are AI computing systems that tightly interconnect multiple servers via high-speed fabric to act as a single massive computer, essential for training trillion-parameter large language models. Huawei's Lingqu protocol is a five-layer stack replacing PCIe, NVLink, and RDMA to enable scale-up of up to 8192 cards without performance loss. The Ascend 950 represents Huawei's latest push to challenge NVIDIA's dominance in AI accelerators.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/cn/news/2026/7/atlas-950-superpod">昇腾950超节点真机亮相2026世界人工智能大会</a></li>

</ul>
</details>

**Tags**: `#华为`, `#昇腾950`, `#AI芯片`, `#算力`, `#数据中心`

---

<a id="item-2"></a>
## [Moonshot AI Releases Open-Source 2.8T Parameter Kimi K3 Model](https://t.me/zaihuapd/42637) ⭐️ 9.0/10

Moonshot AI has released Kimi K3, the first open-source model with 2.8 trillion parameters. It achieved the top score of 1679 in the Frontend Code Arena benchmark, surpassing Claude Fable 5. This release demonstrates that massive open-source models can compete with proprietary leaders in specialized coding tasks. It may accelerate the adoption of large open-weight models in frontend development and beyond. Kimi K3 is built on the Kimi Delta Attention and Attention Residuals architecture, offering native vision capabilities and a 1 million token context window. It jumped from 18th place with its predecessor Kimi k2.6 to 1st, leading in 6 out of 7 Frontend Code Arena domains.

telegram · zaihuapd · Jul 18, 02:29

**Background**: Large language models consume massive computational resources, making efficient attention mechanisms critical. Kimi Delta Attention is a linear attention variant that extends Gated DeltaNet with per-channel decay, reducing memory usage while maintaining quality. Attention Residuals replace standard residual connections with learned attention to improve depth efficiency. The Frontend Code Arena evaluates AI-generated web application code across categories like branding, responsiveness, and interactivity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/moonshot-releases-2-8-trillion-parameter-kimi-k3">China's 2.8-trillion-parameter Kimi K3 beats Claude Fable 5 in Frontend Code Arena benchmark— Moonshot AI delivers largest open-weight AI model ever, as China works around U.S. compute limits | Tom's Hardware</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear [2505.11254] Delta Attention: Fast and Accurate Sparse ... Attention Mechanisms | NVlabs/GatedDeltaNet | DeepWiki hwilner/kimi-delta-attention - GitHub Delta Attention Residuals — cere-bro DeltaNet Explained (Part I) | Songlin Yang</a></li>
<li><a href="https://arxiv.org/pdf/2603.15031">Attention Residuals</a></li>

</ul>
</details>

**Tags**: `#大语言模型`, `#开源`, `#月之暗面`, `#2.8T参数`, `#前端编程`

---

<a id="item-3"></a>
## [US Considers FINRA-like Watchdog for Top AI Models](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 9.0/10

The Trump administration is considering establishing an independent AI oversight body modeled after the Financial Industry Regulatory Authority (FINRA) to review the safety of top AI models. The proposal, led by Treasury Secretary Scott Bessent, is currently under review by White House Chief of Staff Susie Wiles. This policy move could reshape AI regulation in the U.S., addressing Wall Street's cybersecurity concerns and Silicon Valley's grievances over temporary government controls. If implemented, it would give both industries a greater role in setting safety standards for advanced AI models. The proposal aligns with a suggestion from Google DeepMind CEO Demis Hassabis for an industry-funded independent regulator. However, President Trump has not yet reviewed the plan, and the framework remains under discussion and subject to changes.

telegram · zaihuapd · Jul 18, 05:45

**Background**: FINRA is a private U.S. corporation that acts as a self-regulatory organization for broker-dealers and exchange markets. The proposed AI watchdog would similarly be industry-funded and operate independently, reporting to the Securities and Exchange Commission. This approach aims to balance innovation with safety, drawing from the financial sector's regulatory model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Financial_Industry_Regulatory_Authority">Financial Industry Regulatory Authority - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#government policy`, `#Trump administration`, `#AI safety`, `#FINRA`

---

<a id="item-4"></a>
## [First atmosphere on Earth-like planet LHS 1140b confirmed by JWST](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

Astronomers have detected an atmosphere on LHS 1140b, a rocky planet in the habitable zone of a red dwarf star, using JWST emission spectroscopy, ruling out the mini-Neptune scenario. This is the first confirmed atmosphere on a rocky, Earth-sized exoplanet in a habitable zone, a milestone for exoplanet characterization and the search for potential biosignatures. LHS 1140b is about 1.7 times Earth's size and 48 light-years away; JWST's spectroscopy during a secondary eclipse revealed spectral features inconsistent with a thick hydrogen-helium envelope.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Exoplanets larger than Earth but smaller than Neptune are often classified as super-Earths or mini-Neptunes. Mini-Neptunes have thick hydrogen-helium atmospheres. JWST transit spectroscopy analyzes starlight filtered through a planet's atmosphere during transits or eclipses to determine its composition.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2301.04191">[2301.04191] A JWST transmission spectrum of a nearby Earth-sized exoplanet</a></li>

</ul>
</details>

**Discussion**: Comments expressed surprise that a red dwarf planet could retain an atmosphere, but noted the JWST data ruled out a mini-Neptune. Others discussed solar lens telescopes, interstellar propulsion, and the Fermi paradox's communication window implications.

**Tags**: `#exoplanet`, `#astronomy`, `#atmosphere`, `#habitable zone`, `#JWST`

---

<a id="item-5"></a>
## [Kimi K3 and the Pelican Benchmark: Training Data Debate](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

Simon Willison evaluated the new Kimi K3 model using his informal 'pelican on a bike' benchmark, sparking debate about training data contamination and tokenization quirks. The community proposed adversarial extensions to the benchmark. This discussion highlights the challenges of LLM evaluation, especially creative benchmarks that can reveal training data contamination. The analysis also sheds light on hidden system prompts and tokenization inconsistencies across models, which affect cost and performance comparisons. Simon noted that Kimi K3 produced a decent pelican SVG but confirmed his suspicion that the prompt is likely in training data. A commenter observed that prompting 'hi' to Kimi K3 used 86 tokens, suggesting an 85-token hidden system prompt related to reasoning effort.

hackernews · droidjj · Jul 17, 14:21 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The 'pelican on a bike' benchmark is an informal test created by Simon Willison that asks LLMs to generate an SVG of a pelican riding a bicycle. It is used to assess creative coding and visual reasoning. Kimi K3 is a 2.8 trillion parameter model from Chinese startup Moonshot AI, featuring a 1M-token context window and open weights.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that training data contamination is likely, with one noting that content from their own blog appeared in LLMs within 6 months. Others proposed adversarial variants, such as SWE-bench with interruptions requiring SVG generation, to better test model robustness.

**Tags**: `#LLM evaluation`, `#Kimi K3`, `#benchmark`, `#AI safety`, `#community discussion`

---

<a id="item-6"></a>
## [Open source AI models surge in market share](https://stateofopensource.ai/) ⭐️ 8.0/10

Open source AI models have overtaken closed models in token processing volume on OpenRouter, with a nearly 5x increase in just four months. This shift challenges the dominance of closed models from companies like OpenAI and Anthropic, potentially reducing costs and increasing accessibility for developers and enterprises. On March 19, open models processed 888 billion tokens; by July they processed 4.19 trillion tokens, according to OpenRouter data. Market share flipped from 60-40 in favor of closed models to 63-37 in favor of open models.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI models are publicly available for use and modification, often without licensing fees, while closed models are proprietary and require payment for access. This growth highlights a broader trend toward democratization of AI technology.

**Discussion**: Commenters are optimistic about open models overtaking closed ones, with one user noting a dramatic increase in token processing volume. Some criticize the original presentation as LLM-generated and lacking genuine analysis.

**Tags**: `#open-source AI`, `#AI models`, `#market trends`, `#LLMs`

---

<a id="item-7"></a>
## [FAA reinstates Boeing's self-certification for 737 MAX and 787](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html) ⭐️ 8.0/10

The FAA has reinstated Boeing's authority to self-issue airworthiness certificates for the 737 MAX and 787 Dreamliner, an ability revoked after the fatal crashes in 2018 and 2019. This marks a significant step in Boeing's regulatory rehabilitation, potentially speeding up aircraft deliveries and reducing FAA oversight, but raises safety concerns among critics who fear a return to lax self-regulation. Under the Organization Designation Authorization (ODA) program, Boeing can now issue airworthiness certificates without direct FAA inspection, though the FAA retains oversight of design type certificates and overall safety compliance.

hackernews · hmm37 · Jul 17, 21:22 · [Discussion](https://news.ycombinator.com/item?id=48952439)

**Background**: Airworthiness certificates confirm that an individual aircraft conforms to its approved type design and is safe to operate, distinct from type certificates which validate the overall design. The FAA's ODA program allows authorized companies like Boeing to perform certification tasks on behalf of the FAA. After the 737 MAX crashes, the FAA revoked Boeing's ODA authority for issuing airworthiness certificates, requiring direct FAA involvement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.faa.gov/newsroom/faa-statement-boeing-airworthiness-certificates">FAA Statement - Boeing Airworthiness Certificates | Federal Aviation Administration</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX_certification">Boeing 737 MAX certification - Wikipedia</a></li>
<li><a href="https://skybrary.aero/articles/organisation-designation-authorisation-oda">Organisation Designation Authorisation ( ODA )</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion between airworthiness and type certificates, with some noting that recertifications have kept the 737 lineage alive. Others voiced fear and cynicism, suggesting political or financial motives behind the reinstatement.

**Tags**: `#aviation`, `#regulation`, `#Boeing`, `#FAA`, `#safety`

---

<a id="item-8"></a>
## [Three Non-Solving Responses to Problems Analyzed](https://improvesomething.today/responses-to-problems/) ⭐️ 8.0/10

An article titled 'Three ways people respond to a problem (other than solving it)' identifies three common non-solving responses: pushing around, preserving, and ignoring/downplaying. This matters because it reveals counterproductive behaviors in organizations and software engineering, helping teams recognize and avoid such pitfalls to improve problem-solving effectiveness. The article is published on improvesomething.today and has high community engagement with 219 points and 120 comments, indicating strong relevance to software engineering and organizational behavior.

hackernews · surprisetalk · Jul 17, 14:00 · [Discussion](https://news.ycombinator.com/item?id=48947490)

**Background**: Problem-solving is a core skill, but people often avoid directly solving problems due to incentives, power dynamics, or lack of clarity. The three responses provide a framework for diagnosing such behaviors and understanding underlying motivations.

**Discussion**: Commenters noted that ignoring problems can be strategic, preserving problems may benefit those in power, and pushing around can be about delegating. They also suggested a fourth response: changing the problem to fit personal objectives.

**Tags**: `#problem-solving`, `#organizational behavior`, `#decision-making`, `#software engineering`

---

<a id="item-9"></a>
## [Live SSH Honeypot Visualization Shows Bot Attacks in Real Time](https://honeypotlive.cc/) ⭐️ 8.0/10

A new website, honeypotlive.cc, provides a live visualization of SSH honeypot interactions, showing bots attempting to log in and execute commands in real time. This project makes invisible automated attacks visible, helping the cybersecurity community understand attack patterns and the importance of honeypots in threat intelligence. The visualization likely uses the Cowrie SSH honeypot as its data source, which logs attacker commands and can be installed via pip. The site also shows real-time command output, including spam and malicious activity.

hackernews · tusksm · Jul 17, 14:05 · [Discussion](https://news.ycombinator.com/item?id=48947548)

**Background**: An SSH honeypot is a decoy server that mimics a real SSH service to lure attackers. It logs all activity for analysis, helping researchers study automated bot attacks and credential stuffing. Cowrie is a well-known open-source honeypot that supports SSH and Telnet, with advanced shell parsing capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Honeypot_(computing)">Honeypot (computing) - Wikipedia</a></li>
<li><a href="https://github.com/jaksi/sshesame">An easy to set up and use SSH honeypot, a fake SSH server ...</a></li>

</ul>
</details>

**Discussion**: The Cowrie author confirmed the site shows typical internet background noise and highlighted recent improvements to Cowrie. Other commenters mentioned a related LLM-powered honeypot project (honeyprompt) and noted that users were abusing the web interface with large text walls, reducing the ability to see genuine bot patterns.

**Tags**: `#cybersecurity`, `#honeypot`, `#SSH`, `#real-time monitoring`

---

<a id="item-10"></a>
## [Prism Bug Leaks Researchers' Papers](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 8.0/10

A bug in OpenAI's Prism LaTeX compiler accidentally returned another user's paper to a researcher, exposing unpublished work. The issue was flagged on Discord and Twitter, and Prism's team took the website down within 10 minutes. This incident highlights serious privacy and security risks in AI-assisted scientific tools, potentially exposing sensitive unpublished research. It erodes trust among researchers who rely on such platforms for collaborative work. The bug occurred during the compilation process, causing cross-user paper leakage. The affected user expressed concern that their own paper might also have been exposed.

reddit · r/MachineLearning · /u/Few-Monitor5103 · Jul 17, 17:59

**Background**: Prism is a free LaTeX editor and AI-native workspace offered by OpenAI, integrating GPT-5.2 to assist researchers with writing and collaboration. It is designed to streamline scientific document creation but, like any cloud-based tool, raises concerns about data privacy and security.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/prism/">Prism | A free, LaTeX Editor and AI-native workspace for ...</a></li>
<li><a href="https://openai.com/index/introducing-prism/">Introducing Prism - OpenAI</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#security`, `#paper leak`, `#Prism`, `#privacy`

---

<a id="item-11"></a>
## [US Lawmakers Urge Ban on Chinese Memory Chips in Allied Supply Chains](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 8.0/10

US House China Committee chair John Moolenaar and Representative George Whitesides sent a letter to Commerce Secretary Howard Lutnick, urging the addition of ChangXin Memory Technologies (CXMT) to the Entity List and further restrictions on Yangtze Memory Technology Corp (YMTC), citing unacceptable risks to national, economic, and supply chain security. This move could reshape global memory chip supply chains by forcing US and allied companies to exclude Chinese DRAM and NAND Flash, potentially creating strategic dependencies and disrupting procurement for major tech firms like Apple. The lawmakers also urged coordination with Japan, South Korea, and the EU to prevent Chinese manufacturers from embedding in allied supply chains amid shortages, especially for AI infrastructure components. CXMT and YMTC were recently removed from the US Department of Defense's CMC list, but compliance risks remain.

telegram · zaihuapd · Jul 17, 14:00

**Background**: CXMT is China's leading DRAM manufacturer, while YMTC specializes in NAND Flash. The US Entity List restricts foreign entities from purchasing American technology without a license. These Chinese memory firms have faced repeated US sanctions due to alleged military ties, despite being removed from one blacklist recently.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/長江存儲">长江存储 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zh.wikipedia.org/zh-hans/實體清單">实体清单 - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#supply chain`, `#China`, `#memory chips`, `#regulation`

---

<a id="item-12"></a>
## [OpenAI CFO Proposes 'Useful Intelligence Per Dollar' Metric for AI ROI](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 8.0/10

OpenAI CFO Sarah Friar introduced a four-dimensional framework centered on 'useful intelligence per dollar' to measure AI ROI, advocating for outcome-based valuation over traditional token cost metrics. The announcement also highlighted the GPT-5.6 Sol model, which achieves state-of-the-art coding performance using 54% fewer output tokens than competing models. This framework shifts enterprise AI evaluation from simplistic adoption metrics to value-based productivity measures, enabling organizations to make more informed investment decisions. It also underscores the importance of model efficiency and reliability, which directly impact total cost of ownership in production. The four dimensions are: useful work completed, full cost per successful task, dependability of AI outputs, and whether value per dollar scales with usage. OpenAI demonstrated that GPT-5.6 Sol, its most capable coding model, outperforms competing models while using less than half the output tokens and costing about one-third less per task.

telegram · zaihuapd · Jul 17, 15:00

**Background**: Traditional AI cost measurement focuses on token prices—the cost per unit of text processed. However, a cheaper model may require multiple attempts or longer outputs to complete a task, making total cost higher. The 'useful intelligence per dollar' metric captures the actual value delivered by AI, accounting for work completed, reliability, and scaling efficiency. This is analogous to measuring productivity in human labor rather than just hourly wages.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://andresseo.expert/ai/openais-new-ai-scorecard-the-metric-that-finally-measures-roi-beyond-token-costs/">OpenAI's AI Scorecard: Measuring Useful Intelligence per Dollar</a></li>
<li><a href="https://tomtunguz.com/tokens-per-result">Intelligence Per Dollar | Tomasz Tunguz</a></li>

</ul>
</details>

**Tags**: `#AI ROI`, `#OpenAI`, `#productivity metrics`, `#GPT-5.6`, `#AI economics`

---

<a id="item-13"></a>
## [Meta Negotiates $100B AI Compute Lease with Anthropic](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta is in early-stage negotiations to lease AI computing power to Anthropic, in a potential two-year deal worth up to $100 billion, proposed by Anthropic in June 2026. This deal highlights the extreme scarcity of AI compute resources and could provide Meta with a new revenue stream while justifying its massive infrastructure spending to investors. Anthropic would pay monthly under the deal and both parties can exit early. Meta is evaluating the proposal and the talks are at an early stage, so the deal may not materialize.

telegram · zaihuapd · Jul 18, 01:14

**Background**: AI computing power, or compute, is a critical resource for training and running large language models like those developed by Anthropic. Meta has been investing heavily in data centers, planning up to $145 billion in 2026 alone, partly to support its own AI efforts. Leasing excess capacity to other companies helps Meta monetize its investments and address investor concerns about capital spending.

**Tags**: `#AI compute`, `#Meta`, `#Anthropic`, `#datacenter`, `#business deal`

---

<a id="item-14"></a>
## [Spacex in Talks for Pentagon AI Compute Deal](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX is in negotiations with the U.S. Department of Defense to provide data center computing power for running AI models, with a potential deal value reaching tens of billions of dollars. This deal would mark a major expansion of SpaceX's role beyond rocket launches and satellite internet into cloud computing for defense AI, potentially reshaping the competitive landscape among AI infrastructure providers. The talks are ongoing and could still fall through. SpaceX has recently signed similar compute supply agreements with Anthropic and Google, and plans to significantly expand its cloud computing business.

telegram · zaihuapd · Jul 18, 01:44

**Background**: SpaceX is best known for its Starlink satellite constellation, which provides broadband internet globally, and its reusable rockets. The Pentagon is accelerating its acquisition of cloud computing capabilities to support AI applications in national security and daily operations, including a new program called 'AI Arsenal' seeking a $30 billion budget.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbeta.com.tw/articles/science/1569346.htm">SpaceX洽谈为 五 角 大 楼 AI 计划提供算力支持 - SpaceX - cnBeta.COM</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starlink">SpaceX Starlink</a></li>

</ul>
</details>

**Tags**: `#AI`, `#云计算`, `#国防`, `#SpaceX`, `#五角大楼`

---

<a id="item-15"></a>
## [TSMC Announces A14 Process for 2028 Production](https://t.me/zaihuapd/42643) ⭐️ 8.0/10

TSMC has announced its next-generation A14 process technology, scheduled to enter production in 2028, offering up to 15% faster speed or 30% lower power consumption compared to its upcoming N2 process. This announcement reaffirms TSMC's roadmap to maintain leadership in advanced semiconductor manufacturing, crucial for AI and high-performance computing chips that demand ever-greater performance and efficiency. A14 will achieve a logic density improvement of over 20% versus N2. TSMC also plans to launch the intermediate A16 process in late 2026, which will integrate Super Power Rail backside power delivery.

telegram · zaihuapd · Jul 18, 05:00

**Background**: TSMC's N2 is its first process node to use gate-all-around (GAA) nanosheet transistors, entering volume production in 2025. A16 is a 1.6nm-class node that combines GAAFET with backside power delivery. A14, likely a 1.4nm-class node, represents the next step beyond A16. These nodes are part of TSMC's strategy to continuously shrink transistors and improve performance per watt for leading-edge chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tsmc.com/english/dedicatedFoundry/technology/logic/l_A16">A16 Technology - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/tsmc-begins-quietly-volume-production-of-2nm-class-chips-first-gaa-transistor-for-tsmc-claims-up-to-15-percent-improvement-at-iso-power">TSMC begins quietly volume production of 2nm-class chips — first GAA transistor for TSMC claims up to 15% improvement at ISO power | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductor`, `#chip manufacturing`, `#A14`, `#process technology`

---