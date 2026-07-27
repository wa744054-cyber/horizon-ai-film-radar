---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 33 items, 12 important content pieces were selected

---

1. [Moonshot AI Releases Kimi-K3, a 3T Parameter Open-Source LLM](#item-1) ⭐️ 9.0/10
2. [Small 4B Open-Weight Models Approach o3 on Swedish Medical QA](#item-2) ⭐️ 9.0/10
3. [Google reveals Gemini 4 as most ambitious pre-training, due end of 2026](#item-3) ⭐️ 9.0/10
4. [Critical RCE in Fastjson 1.x Without Gadget or AutoType](#item-4) ⭐️ 9.0/10
5. [vLLM v0.26.0 Boosts DeepSeek-V4, Adds Inkling Support](#item-5) ⭐️ 8.0/10
6. [US citizen charged after GrapheneOS phone wipes at airport](#item-6) ⭐️ 8.0/10
7. [Progress in Proof Automation for Formal Verification](#item-7) ⭐️ 8.0/10
8. [Introduction to Data-Oriented Design PDF (2004)](#item-8) ⭐️ 8.0/10
9. [EU Proposes Browser-Level Privacy to Kill Cookie Banners](#item-9) ⭐️ 8.0/10
10. [Inside Look at LLM Token Relay Market for Fraud and Reselling](#item-10) ⭐️ 8.0/10
11. [Claude shared chats indexed by search engines, exposing user data](#item-11) ⭐️ 8.0/10
12. [SpaceX Rejects Falcon 9 Orders, Bets Big on Starship](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Moonshot AI Releases Kimi-K3, a 3T Parameter Open-Source LLM](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

On July 27, Moonshot AI released Kimi-K3, a 2.8 trillion parameter open-source large language model, on HuggingFace. It is built on the company's proprietary Kimi Delta Attention (KDA) mechanism and supports a 1M-token context window. Kimi-K3 is the world's first open-source model in the 3-trillion-parameter class, marking a significant milestone in making ultra-large-scale AI accessible. Its release could drive competition in the AI market, potentially lowering inference costs and spurring innovation in agentic coding and knowledge work. The model requires approximately 1.5TB of VRAM to host using native MXFP4 quantization, pushing the limits of current hardware like 8x B200 GPUs. It integrates native visual understanding and is designed for frontier intelligence scenarios such as long-horizon coding and reasoning.

hackernews · nateb2022 · Jul 27, 06:18 · [Discussion](https://news.ycombinator.com/item?id=49065752)

**Background**: Large language models with trillions of parameters require enormous computational resources for training and inference. Open-source releases like Kimi-K3 allow developers and researchers to study and fine-tune the model, but the high hardware requirements limit practical deployment to well-funded organizations or cloud providers.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://www.kimi.com/en">Kimi AI with K3 | Built for Agentic Coding & Knowledge Work</a></li>

</ul>
</details>

**Discussion**: The community expressed excitement about the model but focused heavily on practical barriers, particularly the enormous VRAM requirements (~1.5TB) and hosting costs. Some commenters discussed how competition from similar models like GLM-5.2 has driven prices down, suggesting that Kimi-K3 could further accelerate price declines. Others speculated about future hardware innovations, such as ROM-like chips for massive model storage.

**Tags**: `#AI`, `#LLM`, `#HuggingFace`, `#Moonshot AI`, `#model release`

---

<a id="item-2"></a>
## [Small 4B Open-Weight Models Approach o3 on Swedish Medical QA](https://www.reddit.com/r/MachineLearning/comments/1v71wds/openweight_4b_models_approach_o3level_medical/) ⭐️ 9.0/10

A developer post-trained Gemma-1.5-4B and tested newer 4B models (Gemma4-E4B, Qwen3.5-4B) on the Swedish medical licensing exam dataset MedQA-SWE, achieving up to 87% accuracy—matching OpenAI's o3 model (88%) in a related benchmark. This demonstrates that small open-weight models can rival top-tier reasoning models like o3 in specialized domains, lowering deployment costs and enabling private, efficient medical AI for low-resource languages like Swedish. Qwen3.5-4B with reasoning enabled reached 87% accuracy; an early exit intervention from the S-GRPO paper was used to prevent reasoning traces from looping. The model performs all reasoning in English despite Swedish prompts, highlighting language-agnostic capability.

reddit · r/MachineLearning · /u/AccomplishedCat4770 · Jul 26, 11:58

**Background**: Open-weight models like Gemma and Qwen release their trained parameters publicly, enabling fine-tuning for specialized tasks. OpenAI's o3 is a reasoning model that uses extended chain-of-thought to achieve high accuracy on benchmarks. MedQA-SWE is a dataset of Swedish medical licensing exam multiple-choice questions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_o3">OpenAI o3 - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2505.07686">[2505.07686] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models Images S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models (PDF) S-GRPO: Early Exit via Reinforcement Learning in ... [PDF] S-GRPO: Early Exit via Reinforcement Learning in ... S-GRPO: Early Exit via Reinforcement Learning in Reasoning ...</a></li>
<li><a href="https://medium.com/@kimanited73/open-weight-models-f504be677b1c">Open Weight Models . What are they, and why should you... | Medium</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#medical AI`, `#open-weight models`, `#LLM`, `#Swedish`

---

<a id="item-3"></a>
## [Google reveals Gemini 4 as most ambitious pre-training, due end of 2026](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 9.0/10

Google CEO Sundar Pichai announced during the Alphabet Q2 2026 earnings call that Gemini 4 is now in training, calling it the company's most ambitious pre-training project yet. The model is expected to launch by the end of 2026, likely in November or December. This signals Google's continued commitment to leading AI frontier development with larger foundation models. The release of Gemini 4 could significantly impact the competitive landscape of large language models and advance capabilities toward AGI. Pichai emphasized that Google will prioritize compute allocation for frontier AGI research to ensure Gemini 4 remains state-of-the-art upon release. Meanwhile, the Gemini 3.x Flash series will maintain nearly monthly updates with focus on improving intelligent coding and other capabilities.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Pre-training is the initial phase of training large language models on massive text datasets to learn grammar, facts, and reasoning. After pre-training, models undergo fine-tuning to specialize for specific tasks. Gemini is a family of multimodal large language models developed by Google DeepMind, succeeding LaMDA and PaLM 2.

<details><summary>References</summary>
<ul>
<li><a href="https://www.entrypointai.com/blog/pre-training-vs-fine-tuning-vs-in-context-learning-of-large-language-models/">Pre-training vs Fine-Tuning vs In-Context Learning of Large Language Models | Entry Point AI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#large language model`, `#pre-training`

---

<a id="item-4"></a>
## [Critical RCE in Fastjson 1.x Without Gadget or AutoType](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a severe remote code execution vulnerability in Fastjson versions 1.2.68 to 1.2.83 that does not require autoType or gadget chains, affecting JDK 8, 17, and 21. This vulnerability is critical because Fastjson 1.x is widely used in Java applications and is now end-of-life with no official patch, forcing affected projects to upgrade to Fastjson 2 or implement risky mitigations. The vulnerability does not require enabling autoType or specific gadget chains in the classpath, making exploitation easier across JDK 8/17/21. Fastjson 1.x reached end-of-life in October 2024, so no official fix is expected.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular Java library for JSON serialization/deserialization developed by Alibaba. Deserialization vulnerabilities often rely on 'gadget chains' — sequences of classes that can lead to arbitrary code execution. 'autoType' is a Fastjson feature that allows specifying the target type via JSON, which has been a common attack vector in previous CVEs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson">GitHub - alibaba/fastjson: FASTJSON 2.0.x has been released ...</a></li>
<li><a href="https://www.klogixsecurity.com/scorpion-labs-blog/gadget-chains">Java Deserialization Gadget Chains</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki/enable_autotype">enable_autotype · alibaba/fastjson Wiki · GitHub</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#Fastjson`, `#RCE`, `#Java`

---

<a id="item-5"></a>
## [vLLM v0.26.0 Boosts DeepSeek-V4, Adds Inkling Support](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 adds support for the Inkling model family, introduces DeepSeek-V4 performance improvements with specialized kernels, and enables flexible attention backends selectable per KV-cache group. This release significantly expands vLLM's model coverage with the cutting-edge Inkling models and delivers critical latency optimizations for DeepSeek-V4, benefiting AI practitioners deploying large-scale inference. The flexible attention mechanism also paves the way for hybrid models combining sliding window and full attention. The release includes 411 commits from 212 contributors, with features such as fp32 lm_head via head_dtype, KV offloading maturation, and a Rust frontend with multimodal video/audio. Notably, it introduces piecewise CUDA graph support and ModelOpt NVFP4 quantization for the Inkling family.

github · khluu · Jul 27, 01:06

**Background**: vLLM is an open-source high-throughput LLM inference engine that manages GPU memory with PagedAttention. The Inkling model is an open-weights multimodal foundation model released by Thinking Machines Lab in July 2026, supporting text, image, and audio inputs. NVFP4 quantization reduces memory footprint by using 4-bit floating point weights, commonly used for deploying large models on NVIDIA GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.sglang.io/docs/sglang-diffusion/quantization">Quantization - SGLang Documentation</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#open-source`

---

<a id="item-6"></a>
## [US citizen charged after GrapheneOS phone wipes at airport](https://www.techspot.com/news/113236-us-prosecutors-charge-atlanta-man-after-grapheneos-phone.html) ⭐️ 8.0/10

A US citizen was charged after his GrapheneOS phone automatically wiped its data during a border search at an airport. The incident highlights the legal risks of using duress PINs or auto-wipe features at borders. This case underscores the tension between security features designed to protect privacy and the legal authority of border agents. It may influence how security-conscious individuals and developers approach threat modeling for border crossings. The charge reportedly stems from the phone's automatic wipe triggered by entering a duress PIN or similar mechanism. The device was running GrapheneOS, a security-focused Android-based OS known for such privacy features.

hackernews · eecc · Jul 26, 22:21 · [Discussion](https://news.ycombinator.com/item?id=49063022)

**Background**: GrapheneOS is an open-source mobile OS focused on security and privacy, based on the Android Open Source Project. It includes features like duress PINs that can wipe the device to protect data. US border agents have broad authority to search electronic devices, and interfering with such searches can lead to charges.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Commenters expressed divided opinions: some emphasized that users must accept legal consequences of using duress PINs, while others pointed out the need for better threat modeling and alternative privacy tools like VeraCrypt's hidden volumes. There was also discussion about the balance between security practices and legal compliance at borders.

**Tags**: `#GrapheneOS`, `#privacy`, `#border search`, `#security`, `#legal`

---

<a id="item-7"></a>
## [Progress in Proof Automation for Formal Verification](https://www.imperialviolet.org/2026/07/26/zstd-lean.html) ⭐️ 8.0/10

Adam Langley's article discusses recent progress in proof automation for formal verification, including cost reductions from 20x overhead to potentially lower levels, and the integration of LLMs to assist with proof generation. This matters because formal verification provides strong correctness guarantees but has been prohibitively expensive; making it cheaper and more automated could significantly improve software security and reliability across the industry. The article notes that proof automation is fundamentally challenging due to undecidability, but recent advances (e.g., Verus, LLM-guided proofs) show promise. Cost comparisons suggest automation could reduce verification effort from 20x to near parity with development for certain projects.

hackernews · zdw · Jul 26, 20:53 · [Discussion](https://news.ycombinator.com/item?id=49062291)

**Background**: Formal verification uses mathematical proofs to confirm that software meets its specifications. Traditionally, it requires extensive manual effort—often 10-20x more than development. Proof automation aims to reduce this burden through tools like Coq, Lean, and now LLM-assisted reasoning, making verification more accessible.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2512.09758">Towards Language Model Guided TLA+ Proof Automation</a></li>
<li><a href="https://martin.kleppmann.com/2025/12/08/ai-formal-verification.html">Prediction: AI will make formal verification go mainstream — Martin...</a></li>
<li><a href="https://veriprajna.com/services/formal-verification-proof-automation">Formal Verification & Proof Automation for AI | Veriprajna</a></li>

</ul>
</details>

**Discussion**: Commenters have mixed views: some argue dependent types and total functions don't scale for maintenance (el_pollo_diablo), while others believe LLMs will enable programmers to write formal specs and proofs automatically (gz09). Another commenter highlights the risk of LLMs implementing features backwards, suggesting verification is needed.

**Tags**: `#formal verification`, `#security`, `#programming languages`, `#software engineering`

---

<a id="item-8"></a>
## [Introduction to Data-Oriented Design PDF (2004)](https://www.gamedevs.org/uploads/introduction-to-data-oriented-design.pdf) ⭐️ 8.0/10

A foundational PDF presentation by Mike Acton from 2004 introduces Data-Oriented Design (DOD), a performance-oriented programming approach that prioritizes data layout over object-oriented abstractions. DOD has become highly influential in game development and systems programming for optimizing CPU cache usage, and this document remains a classic reference that shapes modern performance engineering. The PDF emphasizes designing algorithms by first defining the data structures and transformations, leading to cache-friendly code; however, some community members note that practical requirements often change, making DOD difficult to sustain in evolving projects.

hackernews · tosh · Jul 26, 18:11 · [Discussion](https://news.ycombinator.com/item?id=49060724)

**Background**: Data-Oriented Design is an approach to programming that focuses on the data layout in memory and efficient processing, especially to avoid CPU cache misses. It contrasts with Object-Oriented Design, which often scatters related data across objects. DOD became popular in game development where performance is critical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data - oriented design - Wikipedia</a></li>
<li><a href="https://medium.com/mirum-budapest/introduction-to-data-oriented-programming-85b51b99572d">Introduction to Data - Oriented Design | by Tamás Losonczi | Medium</a></li>
<li><a href="https://stackoverflow.com/questions/1641580/what-is-data-oriented-design">What is data oriented design ? - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of enthusiasm and caution: dustbunny explains the core principle of data-first algorithm design; ghosty141 warns that frequent requirement changes undermine DOD's assumptions; ChicagoDave argues that domains should own their data for complex systems; PessimalDecimal notes DOD seems to be a rebranding of cache-aware algorithms.

**Tags**: `#data-oriented design`, `#software engineering`, `#game development`, `#performance optimization`

---

<a id="item-9"></a>
## [EU Proposes Browser-Level Privacy to Kill Cookie Banners](https://killthecookiebanner.eu/) ⭐️ 8.0/10

The European Commission has proposed a regulation that would allow users to set privacy preferences once in the browser, eliminating the need for cookie banners on every website. If implemented, this could drastically improve user experience and privacy compliance by shifting consent from individual sites to browser standards, reducing annoyance and increasing transparency. The proposal builds on existing opt-out signals like Global Privacy Control (GPC), but would make browser-level preferences legally binding for all websites in the EU.

hackernews · rapnie · Jul 26, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49057175)

**Background**: Cookie banners were mandated by the EU ePrivacy Directive to obtain consent for tracking cookies, but have been criticized as intrusive and ineffective. Browser-level preferences like GPC already exist as a technical mechanism, and the new regulation would codify them into law, potentially replacing banners entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://globalprivacycontrol.org/">Global Privacy Control — Take Control Of Your Privacy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Privacy_Control">Global Privacy Control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters support the move, noting cookie banners rarely constitute informed consent. Others debate technical details, such as default site-isolated cookies and explicit cross-site sharing prompts.

**Tags**: `#privacy`, `#cookie banners`, `#EU regulation`, `#web standards`, `#user experience`

---

<a id="item-10"></a>
## [Inside Look at LLM Token Relay Market for Fraud and Reselling](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard's investigation reveals a market in China where LLM tokens are resold at discounts through API key pooling via proxies like one-api and new-api, abusing free trials and stolen credentials. This market exposes a sophisticated fraud ecosystem that increases security risks for LLM providers and legitimate users, highlighting the urgent need for better API key management and strict spending caps. The proxies primarily use open-source tools like one-api and its fork new-api, which are legitimate API gateways repurposed for abuse. Buyers seek cheaper tokens, bypass geo-restrictions, or perform model distillation.

rss · Simon Willison · Jul 26, 19:30

**Background**: LLM API keys authenticate access to models like GPT-4, often with rate limits per key. API key pooling aggregates multiple keys to bypass these limits. The relay market exploits free trials, unprotected endpoints, and stolen credit cards to gather keys and resell access at a discount.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/songquanpeng/one-api/blob/main/README.en.md">one-api/README.en.md at main · songquanpeng/one-api</a></li>
<li><a href="https://github.com/QuantumNous/new-api">GitHub - QuantumNous/new-api: A unified AI model hub for aggregation & distribution. It supports cross-converting various LLMs into OpenAI-compatible, Claude-compatible, or Gemini-compatible formats. A centralized gateway for personal and enterprise model management. 🍥</a></li>
<li><a href="https://keyd.cloudwaddie.com/">Credit-based API key pooling platform</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#fraud`, `#LLM`, `#API`

---

<a id="item-11"></a>
## [Claude shared chats indexed by search engines, exposing user data](https://search.brave.com/search?q=site%3Aclaude.ai%2Fshare&amp;source=android) ⭐️ 8.0/10

Hundreds of Claude AI shared conversation links have been indexed by search engines like Google and Bing, exposing sensitive user data including API keys, social security numbers, and internal company documents without users' consent. This privacy vulnerability puts countless users at risk of identity theft and corporate espionage, as anyone with a search bar can access private conversations. It also highlights a recurring issue in AI chat platforms, as a similar problem with ChatGPT was fixed a year ago but Anthropic has not yet addressed it. Google has since blocked these indexed pages, but Brave and Bing still serve them in search results. Approximately 600 Claude conversations were indexed by Google, and over 143,000 AI chatbot chats are stored on Archive.org according to research.

telegram · zaihuapd · Jul 26, 11:16

**Background**: Claude is an AI assistant developed by Anthropic that offers a feature to share conversations via public links. When users share a link, the content is meant to be private to those who receive the link, but if the page lacks a 'noindex' HTML meta tag, search engines can crawl and index it, making it publicly searchable. A 'noindex' tag instructs search engines not to include the page in their index.

<details><summary>References</summary>
<ul>
<li><a href="https://startupfortune.com/claude-shared-chats-have-been-indexed-by-google-and-anyone-with-a-search-bar-can-find-them/">Claude shared chats have been indexed by Google and anyone ...</a></li>
<li><a href="https://thecybersecguru.com/news/claude-shared-chats-google-search-privacy/">Claude Shared Chats Indexed by Search Engines Raise Privacy ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#security`, `#Claude`, `#Anthropic`, `#search engine`

---

<a id="item-12"></a>
## [SpaceX Rejects Falcon 9 Orders, Bets Big on Starship](https://www.bloomberg.com/news/articles/2026-07-23/spacex-is-turning-away-falcon-customers-in-major-bet-on-starship) ⭐️ 8.0/10

SpaceX has started rejecting satellite operator requests for dedicated Falcon 9 launches after 2028 and has stopped accepting new bookings for rideshare missions, while also cutting production of some non-reusable Falcon parts to accelerate the transition to Starship. This strategic shift could create a launch capacity gap for many space companies if Starship fails to enter commercial service by late 2028, impacting satellite operators, government missions, and the broader commercial space market. SpaceX may still reserve Falcon 9 for U.S. Department of Defense and NASA missions, but Starship's delays have contributed to a roughly 25% drop in SpaceX's stock price since its IPO in June 2026.

telegram · zaihuapd · Jul 26, 12:42

**Background**: Falcon 9 is SpaceX's workhorse reusable rocket that has dominated the commercial launch market for years. Starship is a next-generation fully reusable super-heavy launch vehicle designed to carry large payloads and crew to the Moon, Mars, and beyond, but it has not yet entered commercial operations and has faced testing delays.

**Tags**: `#SpaceX`, `#Starship`, `#Falcon 9`, `#space launch`, `#strategic shift`

---