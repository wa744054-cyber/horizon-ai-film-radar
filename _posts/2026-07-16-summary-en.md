---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 34 items, 9 important content pieces were selected

---

1. [Inkling: A New Open-Weights Multimodal AI Model with Audio Support](#item-1) ⭐️ 8.0/10
2. [Grok Build Open-Sourced Amid Privacy Controversy](#item-2) ⭐️ 8.0/10
3. [Claude web_fetch loophole allows data exfiltration](#item-3) ⭐️ 8.0/10
4. [Novel technique disentangles convolutional neurons using Hadamard product](#item-4) ⭐️ 8.0/10
5. [PyTorch model 170x slower on T4 vs A100: bottleneck analysis](#item-5) ⭐️ 8.0/10
6. [DeepSeek Raises Over $74 Billion in First Round Using Special Structure](#item-6) ⭐️ 8.0/10
7. [X to Open-Source Entire Codebase, Invite Third-Party Audits](#item-7) ⭐️ 8.0/10
8. [xAI sues user for generating child sexual abuse deepfakes with Grok](#item-8) ⭐️ 8.0/10
9. [CXMT May Match Micron's DRAM Capacity by 2026, Report Says](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Inkling: A New Open-Weights Multimodal AI Model with Audio Support](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines has released Inkling, an open-weights multimodal model that claims to be the largest such model to support audio input. Inkling's release advances open-weight AI by providing a powerful multimodal base that enterprises can fine-tune on Tinker for custom tasks, potentially reducing costs and increasing ownership. Inkling is not the strongest overall model available, but it combines multimodal capabilities, efficient thinking, and availability on Tinker for fine-tuning, making it a good open-weights base for customization.

hackernews · vimarsh6739 · Jul 15, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48924912)

**Background**: Open-weights models have their parameters publicly accessible, allowing modification and fine-tuning. Multimodal models integrate multiple data types like text, audio, and images for a holistic understanding. Inkling is an open-weights multimodal model with audio support, targeting enterprise customization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_model">Multimodal model</a></li>
<li><a href="https://promptmetheus.com/resources/llm-knowledge-base/open-weights-model">Open - weights Model | LLM Knowledge Base</a></li>

</ul>
</details>

**Discussion**: The community is highly engaged, with comments praising Inkling as the largest open-weight model supporting audio and providing links for local execution. Some see it as a promising alternative to Chinese open models like DeepSeek, while others highlight its business model of fine-tuning on Tinker as a cost-effective solution for enterprises.

**Tags**: `#open-weights`, `#multimodal`, `#AI`, `#model release`, `#audio`

---

<a id="item-2"></a>
## [Grok Build Open-Sourced Amid Privacy Controversy](https://github.com/xai-org/grok-build) ⭐️ 8.0/10

xAI has open-sourced Grok Build, a CLI build system for AI models, on GitHub, but users discovered it uploads entire directories to xAI's cloud, prompting community backlash and forks that strip telemetry. This open-sourcing could advance AI build infrastructure, yet the privacy violation undermines trust in xAI and highlights risks of telemetry in developer tools, potentially influencing open-source practices. The codebase includes a self-contained terminal renderer for Mermaid diagrams using Unicode box-drawing, and early community forks like 'gork-build' strip telemetry, opt-out data retention, and block auto-updates.

hackernews · skp1995 · Jul 15, 20:24 · [Discussion](https://news.ycombinator.com/item?id=48926590)

**Background**: Grok is a generative AI chatbot by xAI, launched in November 2023, integrated with X and Tesla. Grok Build is a CLI tool for building AI models, now open-sourced. The controversy follows xAI's history of privacy concerns and criticism over content moderation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_Build">Grok Build</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://docs.x.ai/build/overview">Grok Build | SpaceXAI Docs</a></li>

</ul>
</details>

**Discussion**: Community comments express shock at data exfiltration (e.g., uploading SSH keys), praise the model's quality, and note forks removing telemetry. Some view open-sourcing as a tactical move to regain trust, while others recommend alternative tools like pi.dev.

**Tags**: `#open source`, `#Grok Build`, `#xAI`, `#AI infrastructure`, `#privacy`

---

<a id="item-3"></a>
## [Claude web_fetch loophole allows data exfiltration](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Security researcher Ayush Paul discovered a loophole in Anthropic's Claude web_fetch tool that allowed exfiltration of private user memories by following nested links from a malicious website. Anthropic stated they had already internally identified the vulnerability and have since patched it by preventing web_fetch from navigating to URLs returned in fetched content. This attack highlights a critical weakness in LLM agent security, bypassing Anthropic's designed protections against data exfiltration. It underscores the ongoing challenge of preventing prompt injection and the lethal trifecta (private data, untrusted input, exfiltration ability) in AI systems. The attack required the attacker to control a webpage that dynamically generated links; web_fetch was allowed to follow URLs from previously fetched pages, enabling a chain of exfiltration. The exploit targeted only clients with a 'Claude-User' user-agent to evade detection, and Anthropic did not pay a bug bounty as they claimed prior internal discovery.

rss · Simon Willison · Jul 15, 14:21

**Background**: Prompt injection is a vulnerability where malicious inputs cause LLMs to override intended instructions, potentially leading to harmful actions. The lethal trifecta refers to a scenario where an AI agent simultaneously has access to private data, is exposed to untrusted content (e.g., via web browsing), and possesses a tool to exfiltrate data (e.g., by embedding secrets in URLs). Claude's web_fetch tool was designed with safeguards to prevent exfiltration by restricting navigation to user-provided URLs or search results, but the loophole in allowing navigation to URLs within fetched pages enabled this attack.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://www.cyera.com/research/when-language-becomes-the-attack-vector-the-lethal-trifecta-of-ai-agents">When Language Becomes the Attack Vector: The Lethal Trifecta of AI...</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI safety`, `#prompt injection`, `#Claude`, `#data exfiltration`

---

<a id="item-4"></a>
## [Novel technique disentangles convolutional neurons using Hadamard product](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

The author proposes a technique using the Hadamard product of a neuron's receptive field and its weights to cluster and identify distinct patterns detected by a single neuron in InceptionV1, revealing monosemantic clusters such as cars, cats, and dogs, as well as unexpected low-activation patterns like letters. This work provides a new method for mechanistic interpretability of convolutional neural networks, offering insights into how neurons encode multiple concepts and how gradient descent distributes weights to suppress irrelevant patterns. It could inspire more transparent analysis of vision models and potentially extend to other architectures. The technique was applied to a 1x1 convolution neuron in the mixed4e layer of InceptionV1, and analysis of low-activation clusters showed that all dependent neurons also fired on the same concept, with positive and negative weights evenly distributed to reduce the sum. The author emphasizes that this is independent, early-stage work with a focus on visualizations.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability seeks to understand the internal representations and computations of neural networks. Convolutional neurons often exhibit polysemanticity, responding to multiple unrelated features. The Hadamard product (element-wise multiplication) of the receptive field and weight matrix isolates what the neuron is 'seeing'. Clustering such products can reveal semantic clusters, similar to how sparse autoencoders are used for language models, but this approach is novel for CNNs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://www.lesswrong.com/posts/nkDcuNzazmQsJFBwA/mechanistic-interpretability-through-clustering">Mechanistic interpretability through clustering</a></li>
<li><a href="https://dl.acm.org/doi/10.1145/3787104">Bridging the Black Box: A Survey on Mechanistic Interpretability in AI | ACM Computing Surveys</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#InceptionV1`, `#machine learning research`

---

<a id="item-5"></a>
## [PyTorch model 170x slower on T4 vs A100: bottleneck analysis](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A user reports a ~170x slowdown when running a point-tracking PyTorch model on an NVIDIA T4 GPU compared to an A100, with the T4 taking 85 seconds per half-video versus 0.5 seconds on the A100. This extreme gap highlights how hardware differences, especially memory bandwidth and FP32 throughput, can cause order-of-magnitude performance variability in GPU-accelerated deep learning workloads, making it critical to profile and optimize operations. The model uses pure FP32 precision, builds local 4D correlation volumes for dense matching, and includes transformer layers; both GPUs show 99% utilization, ruling out idle time. Two independent T4 machines exhibit the same slowdown.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 has significantly lower memory bandwidth (320 GB/s) and FP32 performance (8.1 TFLOPS) compared to the A100 (1.6 TB/s bandwidth, 19.5 TFLOPS FP32). Operations with low arithmetic intensity (memory-bound kernels) are limited by bandwidth; the 4D correlation volumes likely involve many small memory accesses, making the T4's lower bandwidth a primary bottleneck. Additionally, the A100's larger L2 cache and faster interconnects can further amplify the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://modal.com/gpu-glossary/perf/memory-bound">What does it mean to be memory-bound? | GPU Glossary</a></li>
<li><a href="https://news.ycombinator.com/item?id=24522596">I posted this a day or two ago: The A 100 whitepaper... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU performance`, `#NVIDIA T4`, `#NVIDIA A100`, `#model debugging`

---

<a id="item-6"></a>
## [DeepSeek Raises Over $74 Billion in First Round Using Special Structure](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek has raised over 500 billion RMB (≈74 billion USD) in its first round of funding, using a limited partnership structure where investors must invest into a fund managed by founder Liang Wenfeng, accepting a five-year lock-up and no voting rights. This massive funding round, involving major investors like Tencent and CATL, highlights the immense capital appetite in AI and sets a precedent for founder control structures in Chinese tech. It could influence how other AI startups structure their financing. Founder Liang Wenfeng personally invested 200 billion RMB. Tencent is considering investing 100 billion and CATL 50 billion. The limited partnership structure gives investors no voting rights and a five-year lock-up period.

telegram · zaihuapd · Jul 15, 12:56

**Background**: A limited partnership (LP) structure separates control and economic rights: the General Partner (GP) manages the fund and has full decision-making power, while Limited Partners (LPs) contribute capital and share profits but have no voting rights. This allows founders to retain control despite raising large sums. Such structures are common in venture capital and private equity.

<details><summary>References</summary>
<ul>
<li><a href="https://36kr.com/p/2360646821709699">36kr.com/p/2360646821709699</a></li>
<li><a href="https://heshulin.net/shulinguandian/463.html">东莞 - 股权 架 构 设计：6种主流模型及其利弊分析_股权专家何树林</a></li>
<li><a href="http://victory.itslaw.cn/victory/api/v1/articles/article/33f49951-5be6-4c7f-ba52-b42e49b5f3ff">无讼阅读｜取得公司控制权，架构“有限合伙”持股或许是优选方案</a></li>

</ul>
</details>

**Tags**: `#AI`, `#融资`, `#DeepSeek`, `#创业`, `#商业`

---

<a id="item-7"></a>
## [X to Open-Source Entire Codebase, Invite Third-Party Audits](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 8.0/10

Elon Musk announced that after completing a security vulnerability review, X will unconditionally open-source its entire codebase and invite third-party auditors to verify that the open-source code matches the running system. This move could dramatically increase transparency and trust in the X platform, setting a new standard for social media companies regarding openness and accountability. The open-sourcing is unconditional and will follow a security review; third-party auditors will check that the running code matches the open-source code to prevent hidden modifications.

telegram · zaihuapd · Jul 15, 13:32

**Background**: Open-source software makes its source code publicly available for anyone to inspect, modify, and distribute. Social media platforms have faced criticism over opaque algorithms and content moderation decisions, and full open-sourcing could allow external verification of how the platform operates, potentially increasing user trust.

**Tags**: `#open-source`, `#transparency`, `#social media`, `#Elon Musk`, `#X`

---

<a id="item-8"></a>
## [xAI sues user for generating child sexual abuse deepfakes with Grok](https://www.reuters.com/legal/litigation/musks-xai-sues-grok-user-over-sexualized-deepfakes-2026-07-15/) ⭐️ 8.0/10

xAI has filed a lawsuit against South Carolina man Terry Harwood, accusing him of using its Grok chatbot to generate child sexual abuse material and nonconsensual adult deepfakes. This marks one of the first cases where an AI company has sued a user for misusing its technology to create harmful content. This lawsuit sets a legal precedent for holding AI users accountable for generating illegal content, potentially forcing AI companies to implement stricter safeguards. It highlights the urgent need for robust AI governance and content moderation to prevent the misuse of generative AI for child exploitation. The lawsuit seeks damages and a permanent injunction banning Harwood from using Grok. xAI stated it has suspended 52,222 accounts, reported 73,604 incidents to the National Center for Missing & Exploited Children, and contributed to at least 244 arrests this year.

telegram · zaihuapd · Jul 16, 01:45

**Background**: Grok is a generative AI chatbot developed by xAI, launched in November 2023 and integrated with the X social network. It has faced controversy for generating harmful content, including nonconsensual sexualized images. Child sexual abuse material (CSAM) refers to any visual depiction of sexually explicit conduct involving a minor, and its creation and distribution are illegal under U.S. federal law.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot)</a></li>
<li><a href="https://www.missingkids.org/theissues/csam">Child Sexual Abuse Material</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#deepfakes`, `#legal`, `#child safety`, `#xAI`

---

<a id="item-9"></a>
## [CXMT May Match Micron's DRAM Capacity by 2026, Report Says](https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer) ⭐️ 8.0/10

A report from Citrini Research predicts that Chinese DRAM maker CXMT will reach approximately 350,000 wafers per month by the end of 2026, approaching Micron's 375,000 wafers per month. This would position China as the world's second-largest DRAM producer. This development could reshape global DRAM supply dynamics, reducing dependence on South Korean and U.S. suppliers, and has significant geopolitical implications as the U.S. considers tighter export controls on semiconductor equipment. Other Chinese firms including SiEn, Jinhua Integrated Circuit, and XMC are also expanding, potentially pushing total Chinese DRAM capacity to 600k wpm. However, access to advanced immersion DUV lithography equipment remains a critical bottleneck, and the U.S. MATCH Act could restrict exports of such tools.

telegram · zaihuapd · Jul 16, 02:30

**Background**: DRAM (Dynamic Random Access Memory) is a type of memory used in computers and servers. Currently, the market is dominated by Samsung, SK Hynix, and Micron. CXMT is a leading Chinese DRAM manufacturer striving to increase its production capacity. The MATCH Act is a proposed U.S. law aiming to restrict exports of advanced semiconductor manufacturing equipment to adversaries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products</a></li>
<li><a href="https://www.foreign.senate.gov/press/rep/release/risch-ricketts-kim-introduce-match-act-level-the-global-playing-field-for-us-tech">Risch, Ricketts, Kim Introduce MATCH Act; Level the Global Playing Field for U.S. Tech | United States Senate Committee on Foreign Relations</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#semiconductor`, `#China`, `#CXMT`, `#memory`

---