---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 37 items, 8 important content pieces were selected

---

1. [Google Removes Manifest V2 Extensions from Chrome Web Store](#item-1) ⭐️ 8.0/10
2. [NAT: Original Sin of Internet Centralization?](#item-2) ⭐️ 8.0/10
3. [Sliding-window attention beats linear attention on long-context reasoning](#item-3) ⭐️ 8.0/10
4. [Entropic Scree Tool Gauges Signal Strength in Dirty Data](#item-4) ⭐️ 8.0/10
5. [Claude shared chat links exposed by search engines, leaking sensitive user data](#item-5) ⭐️ 8.0/10
6. [OpenClaw 2.0: Largest Update Ever, 16,000+ Pull Requests](#item-6) ⭐️ 8.0/10
7. [DeepSeek Releases Experimental Vision-Language Model on API](#item-7) ⭐️ 8.0/10
8. [Xiaomi Unveils Three Xuanjie Chips; O3 SoC to Debut in 18 Fold](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google Removes Manifest V2 Extensions from Chrome Web Store](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has begun removing Manifest V2 (MV2) extensions from the Chrome Web Store, effectively delisting popular tools like uBlock Origin. Users upgrading to Chrome 139 and later will no longer be able to use these extensions. This marks a major milestone in Chrome's forced transition to Manifest V3, which many privacy advocates say weakens ad-blocking. It affects millions of users, fuels concerns about Google's control over the web, and is pushing users toward alternative browsers like Firefox. Manifest V3 restricts extensions by replacing the blocking webRequest API with declarativeNetRequest and limiting filter rules to roughly 30,000. uBlock Origin's developer recommends Firefox, where its full version remains available; Chrome users are offered uBlock Origin Lite instead.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Manifest V2 was the extension specification Chrome had used for years, allowing powerful extensions like uBlock Origin to intercept network requests and block ads before they load. Google announced MV3 in 2019 as a more secure, private, and performant replacement, but critics including the EFF argue it harms ad blocking and user autonomy. Chrome 139 disables all remaining MV2 extensions.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V 2 support timeline | Chrome for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2021/12/googles-manifest-v3-still-hurts-privacy-security-innovation">Google’s Manifest V 3 Still Hurts Privacy, Security, and Innovation</a></li>

</ul>
</details>

**Discussion**: Commenters largely condemn Google's decision, describing ad blocking as a safety necessity and suspecting Google of protecting its ad revenue. Many recommend switching to Firefox, with some noting that uBlock Origin has always worked better there. Overall sentiment is strongly anti-Chrome and in favor of browser diversity.

**Tags**: `#Chrome`, `#MV2`, `#uBlock Origin`, `#ad-blocking`, `#privacy`

---

<a id="item-2"></a>
## [NAT: Original Sin of Internet Centralization?](https://dreamstation.systems/personal/ntppost.html) ⭐️ 8.0/10

A reflective essay argues that NAT (Network Address Translation) was a key early enabler of Internet centralization, and the original Linux NAT implementer, Rusty Russell, commented to acknowledge and expand on the technical decisions he made decades ago. 这一讨论为关于开放、对等的互联网为何让位于如今客户端-服务器、云主导模式的长期辩论，提供了罕见的内部视角。它也重新引发人们对 NAT 在塑造安全、地址稀缺性以及自托管难度方面作用的关注。 Rusty Russell explained that he prioritized squeezing more connections into a single IP address by avoiding port reservation, which made inbound connections from different addresses unroutable, effectively eliminating public endpoints. Commenters distinguish between ordinary controllable NAT, which they see as acceptable, and Carrier Grade NAT (CGNAT), which they call 'truly evil' for restricting users' freedoms.

hackernews · robinpie · Aug 31, 02:23 · [Discussion](https://news.ycombinator.com/item?id=49504905)

**Background**: NAT was invented as a temporary workaround for IPv4 address exhaustion, allowing many private devices to share one public IP address. It remaps outgoing connection ports so return traffic can be sorted out, but it also blocks unsolicited inbound connections, which is why port forwarding and UPnP are needed for self-hosted services. IPv6 was designed to restore end-to-end connectivity, but NAT has persisted due to inertia, security justifications, and carrier deployment of CGNAT.

**Discussion**: Comments show a mix of agreement and pushback: some mourn the loss of easy self-hosting and the normalization of client-server thinking, while others argue regular NAT is fine and has even protected insecure devices. Rusty Russell's confession adds weight to the idea that NAT's consequences were not fully foreseen, sparking broader concerns about meatspace norms being wrongly applied to cyberspace.

**Tags**: `#NAT`, `#Internet`, `#Networking`, `#Centralization`, `#IPv6`

---

<a id="item-3"></a>
## [Sliding-window attention beats linear attention on long-context reasoning](https://www.reddit.com/r/MachineLearning/comments/1w3j1vw/slidingwindow_attention_beats_linear_on/) ⭐️ 8.0/10

A new arXiv preprint claims that sliding-window attention (SWA) with sinks outperforms linear attention variants by 2 to 10 times on long-context reasoning benchmarks such as BABILong and Needle-in-a-Haystack, all without any post-training. This result challenges the linear attention research direction and may affect labs that have invested heavily in post-training to produce linear models. It suggests the field has been benchmarking against the wrong baselines, which could reshape how long-context efficiency methods are evaluated. SWA requires no post-training, runs fast, and keeps memory usage low. The authors strongly recommend switching to SWA instead of post-training linear models, noting that linear attention may need to be trained from scratch or undergo extensive post-training to match SWA.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Aug 31, 16:35

**Background**: Standard transformer self-attention scales quadratically with sequence length, making long-context processing expensive. Linear attention aims to reduce this to linear complexity, but often requires post-training to work well; sliding-window attention reduces computation by only attending to a local window, and attention sinks retain early tokens to stabilize generation. BABILong is a benchmark that uses a needle-in-a-haystack approach to test reasoning across facts embedded in extremely long documents.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.28444v1">Sliding - window beats linear attention</a></li>
<li><a href="https://www.alphaxiv.org/abs/2608.28444">Sliding - window beats linear attention | alphaXiv</a></li>
<li><a href="https://arxiv.org/abs/2406.10149">[2406.10149] BABILong: Testing the Limits of LLMs with Long Context Reasoning-in-a-Haystack</a></li>

</ul>
</details>

**Tags**: `#Attention`, `#Long-context`, `#LLM`, `#Efficiency`, `#Research`

---

<a id="item-4"></a>
## [Entropic Scree Tool Gauges Signal Strength in Dirty Data](https://www.reddit.com/r/MachineLearning/comments/1w3br9c/how_to_assess_if_there_is_a_strong_signal_in_your/) ⭐️ 8.0/10

A new diagnostic tool called Entropic Scree (v1.0.0) is now available as an R function, with a preprint, and it estimates signal-to-noise ratio, intrinsic rank, and linear sufficiency in high-dimensional real-world data using a transformed mutual information metric instead of variance-based PCA. This matters because standard PCA-based methods rely on linear variance assumptions that break down on messy, high-dimensional data; Entropic Scree's mutual information approach gives practitioners a more robust way to know whether their data contains a learnable signal before building models. The tool also provides an exploratory map of decoupled variable sub-networks and serves as a practical diagnostic for the 'From Garbage to Gold' framework, which explains when uncurated data can still support accurate prediction. Python and R packages are planned, but currently only the R function Entropic.Scree.v1.0.0 is available, and the approach has not yet undergone broad community validation or extensive real-world benchmarking.

reddit · r/MachineLearning · /u/Chocolate_Milk_Son · Aug 31, 12:02

**Background**: Principal component analysis (PCA) and related methods summarize variance and assume linear relationships, which often make them misleading for 'dirty' datasets with errors, missing values, and nonlinear dependencies. Mutual information measures how much knowing one variable tells you about another without assuming a relationship shape; Entropic Scree uses it to estimate how much genuine signal a dataset holds relative to its idiosyncratic noise. Linear sufficiency, in turn, asks whether a linear projection preserves all the information needed for estimation, which the tool reports to indicate whether standard PCA assumptions are appropriate. The referenced 'From Garbage to Gold' framework argues that data quality should be evaluated at the portfolio level rather than item by item, providing theoretical support for learning directly from messy enterprise data.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.12288">[2603.12288] From Garbage to Gold: A Data-Architectural Theory of Predictive Robustness</a></li>
<li><a href="https://arxiv.org/html/2603.12288">From Garbage to Gold: A Data-Architectural Theory of Predictive Robustness</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sufficient_statistic">Sufficient statistic - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#data-analysis`, `#mutual-information`, `#dimensionality-reduction`, `#tabular-data`, `#diagnostic-tool`

---

<a id="item-5"></a>
## [Claude shared chat links exposed by search engines, leaking sensitive user data](https://t.me/zaihuapd/43511) ⭐️ 8.0/10

Anthropic's Claude shared-chat feature generates public links without noindex tags, so Google and other search engines have indexed them. Sensitive content such as API keys, crypto wallet information, resumes, legal consultation records, internal company project data, and Social Security numbers is now publicly searchable. This is a serious privacy flaw because anyone can discover private conversations through ordinary web searches, exposing credentials and personal data that can be misused or sold. It affects all Claude users who have used the share feature, and Anthropic's slow response heightens the risk while ChatGPT's similar bug was patched quickly. The leak includes API keys, cryptocurrency wallets, resumes, attorney-client consultations, internal company documents, and Social Security numbers. Anthropic has not yet fixed the vulnerability, so users are advised to manually delete private or financial chats from the Settings > 'Shared Chats' management page.

telegram · zaihuapd · Aug 31, 03:22

**Background**: Claude is a series of large language models and AI assistants developed by Anthropic, released as a chatbot in March 2023. A noindex HTML meta tag instructs search engine bots such as Google not to index a page, and shared public links normally need this tag to stay out of search results. An API key is a code used to authenticate an application or user in computer systems, and leaking it can allow unauthorized access. About a year ago, ChatGPT suffered a similar shared-links indexing bug that was quickly fixed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Noindex">noindex - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/API_key">API key - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#security`, `#Claude`, `#Anthropic`, `#vulnerability`

---

<a id="item-6"></a>
## [OpenClaw 2.0: Largest Update Ever, 16,000+ Pull Requests](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

OpenClaw released version 2.0 on August 30, its largest update ever, incorporating over 16,000 pull requests from 933 contributors, including 569 first-time contributors. The update overhauls installation, messaging, memory, skills, models, browser, plugins, security, and adds shared cloud sessions for collaboration. This release significantly expands OpenClaw's capabilities and demonstrates strong community momentum, reinforcing its position in the open-source AI agent ecosystem. The scale of contributions—roughly half of all pull requests in the project's history—could attract more developers and users to agentic AI tools. The team went nearly seven weeks without a release to consolidate the update. It simplifies the installation process, rebuilds the browser-side experience, and introduces shared cloud sessions that allow multiple users to collaborate in real time.

telegram · zaihuapd · Aug 31, 04:38

**Background**: OpenClaw is a free, open-source autonomous AI agent that runs on a user's machine and uses messaging platforms as its primary interface. AI agents use large language models to pursue goals, use tools, and perform multi-step tasks with some autonomy. Pull requests are GitHub's collaboration feature for proposing, reviewing, and merging code changes, which is how the 16,000+ contributions were aggregated.

<details><summary>References</summary>
<ul>
<li><a href="https://openclaw.ai/">OpenClaw — Open -Source AI Assistant</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://docs.github.com/en/pull-requests/reference/pull-requests">Pull requests - GitHub Docs</a></li>

</ul>
</details>

**Tags**: `#OpenClaw`, `#open-source`, `#release`, `#AI agents`, `#developer tools`

---

<a id="item-7"></a>
## [DeepSeek Releases Experimental Vision-Language Model on API](https://t.me/zaihuapd/43518) ⭐️ 8.0/10

DeepSeek has released the experimental vision-language model deepseek-v4-flash-vision-exp, now available via its API. The official documentation and pricing were updated on the same day. This marks DeepSeek's expansion into multimodal AI, allowing developers to build applications that interpret images and text together. It strengthens DeepSeek's position against commercial rivals like OpenAI's GPT-4V and Anthropic's Claude with vision capabilities. The model accepts mixed text-and-image input in Chat Completions, Responses, and the Anthropic-compatible Messages API, supporting image input via URL, Base64 and files. Compared to DeepSeek-V4-Flash-0731, it substantially improves multimodal agent capabilities while maintaining comparable text-only agent performance.

telegram · zaihuapd · Aug 31, 11:41

**Background**: A vision-language model (VLM) is an AI system that interprets and generates information from both images and text, extending large language models beyond text-only tasks. Many major providers such as OpenAI, Google, Anthropic and Microsoft have added vision capabilities to their flagship models. DeepSeek's experimental release gives developers an open alternative for multimodal applications like image description, OCR from screenshots, and chart analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/guides/vision/?ref=upstract.com">Vision | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-Vision-Exp">deepseek-ai/ DeepSeek - V 4 - Flash - Vision - Exp · Hugging Face</a></li>
<li><a href="https://chat-deep.ai/docs/deepseek-api-vision-input/">DeepSeek Vision API: Image Input via URL, Base64 & Files</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#API`, `#vision-language model`, `#AI release`, `#LLM`

---

<a id="item-8"></a>
## [Xiaomi Unveils Three Xuanjie Chips; O3 SoC to Debut in 18 Fold](https://t.me/zaihuapd/43524) ⭐️ 8.0/10

Xiaomi announced three new Xuanjie chips: the AI flagship SoC Xuanjie O3, the 1.22 TB/s AI accelerator Xuanjie O100, and the 3nm smart-driving chip Xuanjie D100, with all three completing tape-out validation. The O3 SoC will be the first to power the Xiaomi 18 Fold. This marks Xiaomi's push into proprietary silicon across mobile, AI acceleration, and automotive, reducing reliance on external chip vendors. The O3's claim of being the world's first LPDDR6-capable mobile processor and its strong benchmark scores could intensify competition among smartphone SoC makers. The Xuanjie O3 uses a ten-core all-large-core CPU and its multi-core benchmark reportedly broke the 15,000-point mark. It also debuts the 16-core G2-Ultra NX GPU, claimed to deliver 85% higher performance and 64% lower power draw than the previous O1, and supports LPDDR6 memory with higher bandwidth.

telegram · zaihuapd · Aug 31, 15:15

**Background**: Tape-out validation means the chip design has been sent to a foundry and the first physical samples have come back for testing, confirming the design works. LPDDR6 is the latest low-power memory standard from JEDEC, designed to provide higher bandwidth for on-device AI workloads in smartphones and other mobile devices; Xiaomi's partner CXMT also recently announced LPDDR6 mass production, and Xiaomi phones are expected to debut the first commercial LPDDR6 chips.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR</a></li>
<li><a href="https://www.tomshardware.com/pc-components/dram/chinas-cxmt-beats-western-chipmakers-to-announcement-of-lpddr6-mass-production-xiaomi-smartphones-to-debut-industrys-first-lpddr6-chips">China's CXMT beats Western chipmakers to... | Tom's Hardware</a></li>
<li><a href="https://gadgets.beebom.com/guides/xiaomi-xring-o3-benchmark-specs">Xiaomi Xring O3: Benchmarks and Specs | Beebom Gadgets</a></li>

</ul>
</details>

**Tags**: `#Xiaomi`, `#chip`, `#AI`, `#SoC`, `#hardware`

---