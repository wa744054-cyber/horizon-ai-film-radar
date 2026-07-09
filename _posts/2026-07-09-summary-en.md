---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 34 items, 12 important content pieces were selected

---

1. [TypeScript 7.0 Released with Go-Powered Compiler](#item-1) ⭐️ 9.0/10
2. [Ant LingBot open-sources LingBot-Video, first MoE embodied video model](#item-2) ⭐️ 9.0/10
3. [John Deere Settles FTC, Grants Right to Repair](#item-3) ⭐️ 8.0/10
4. [OpenAI Tackles Noise in Coding Benchmarks](#item-4) ⭐️ 8.0/10
5. [Cloudflare Drop launches drag-and-drop deployment](#item-5) ⭐️ 8.0/10
6. [Bun Rewrites Runtime from Zig to Rust Using AI](#item-6) ⭐️ 8.0/10
7. [Chatto Open-Sourced: Self-Hosted Chat App Now Available](#item-7) ⭐️ 8.0/10
8. [Kenton Varda Bans AI-Written Change Descriptions](#item-8) ⭐️ 8.0/10
9. [Cloudflare and OpenAI Pilot Network Data for AI Search](#item-9) ⭐️ 8.0/10
10. [Researchers Identify Smartphone Apps via Electromagnetic Signals with 99% Accuracy](#item-10) ⭐️ 8.0/10
11. [LineageOS Introduces Browser-Based Flashing Tool](#item-11) ⭐️ 8.0/10
12. [National Supercomputing Internet Core Node Goes Live in Zhengzhou](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [TypeScript 7.0 Released with Go-Powered Compiler](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has released TypeScript 7.0, a major version featuring a complete rewrite of the compiler in Go, achieving up to ~12x faster build times (e.g., 125.7s to 10.6s for the VS Code codebase). This significant performance improvement removes a key bottleneck for large TypeScript codebases, making development more efficient and potentially accelerating adoption of TypeScript in performance-sensitive projects. The new compiler supports shared-memory multithreading with customizable parallelism via --checkers and --builders flags, and includes a compatibility package for coexistence with TypeScript 6; however, embedded language tools for Vue and Svelte are not yet supported.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript, widely used in large-scale web development. The previous compiler was written in TypeScript itself, which could be slow for large projects. By rewriting the compiler in Go, a language known for fast compilation and efficient concurrency, Microsoft drastically improved performance while maintaining full type system compatibility.

**Discussion**: Community members expressed excitement about the massive speed improvements, with some noting the incredible feat of maintaining two codebases simultaneously. Others celebrated TypeScript's role in popularizing type systems, and a few users highlighted ongoing focus on JSDoc syntax while acknowledging migration challenges for embedded toolchains.

**Tags**: `#TypeScript`, `#compiler`, `#performance`, `#Go`, `#type system`

---

<a id="item-2"></a>
## [Ant LingBot open-sources LingBot-Video, first MoE embodied video model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

Ant LingBot has open-sourced LingBot-Video, claimed to be the world's first Mixture-of-Experts (MoE) based embodied intelligence video foundation model, adopting a DiT+MoE architecture with 30B total parameters but only ~3B activated per inference. On the RBench benchmark for robot manipulation videos, it achieved an overall score of 0.620, surpassing models like Wan2.6, Seedance1.5 Pro, and Cosmos3 Super. This is significant because it is the first open-source embodied video generation model to use a sparse MoE architecture, dramatically improving inference efficiency while maintaining high quality. It can be used for robot action prediction, simulation data generation, and world model research, potentially accelerating development in embodied AI and robotics. LingBot-Video uses a single-stream Diffusion Transformer with a DeepSeek-V3-style sparse MoE (128 experts, top-8 routing), and post-training with six-reward reinforcement learning including a physical-plausibility reward graded by a VLM. It is released under the Apache 2.0 license, with weights, code, and inference stack available on GitHub and Hugging Face.

telegram · zaihuapd · Jul 9, 04:30

**Background**: Mixture of Experts (MoE) is a neural network architecture that activates only a subset of parameters for each input, improving efficiency while keeping a large total parameter count. Diffusion Transformer (DiT) replaces the traditional U-Net backbone with a transformer for diffusion models, offering better scalability. Embodied intelligence refers to AI systems that perceive and act in the physical world, such as robots, and video foundation models for embodied tasks aim to understand and generate videos of interactions with the environment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://github.com/facebookresearch/dit">GitHub - facebookresearch/DiT: Official PyTorch Implementation of "Scalable Diffusion Models with Transformers" · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Embodied_intelligence">Embodied intelligence</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights technical specifics (single-stream DiT, 128 experts, top-8, 1.4B active of 13B total, six-reward RL) but raises concerns: whether a VLM can reliably judge physical plausibility (risk of Goodhart's law), and whether the model truly acts as a policy evaluator or remains a video generator without closed-loop robot results. On RBench it achieves top average, but reasoning-heavy dimensions still favor closed models, and it ranks second on general T2V in its own evaluation.

**Tags**: `#MoE`, `#具身智能`, `#视频生成`, `#开源模型`, `#机器人`

---

<a id="item-3"></a>
## [John Deere Settles FTC, Grants Right to Repair](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

John Deere has settled with the Federal Trade Commission (FTC) and five states, agreeing to allow farmers and independent repair shops to fix their own equipment, a major victory for the right-to-repair movement. This settlement sets a precedent for the agricultural sector and could pressure other manufacturers to adopt similar policies, addressing long-standing consumer frustration over costly, restricted repairs. John Deere must pay $1 million in penalties to the five states and is subject to 10 years of compliance monitoring; the FTC decision highlights ongoing antitrust concerns and the modest fine has drawn criticism.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: The right-to-repair movement advocates for consumers and third-party repair shops to have access to the tools, parts, and information needed to fix products. John Deere had been criticized for using proprietary software and digital locks to prevent independent repairs, forcing farmers to use authorized dealers at higher costs.

**Discussion**: Commenters celebrated the win, with thanks to activists like Louis Rossmann, but criticized the small $1 million fine as insufficient for a company with billions in profit. Some noted the irony of tech enthusiasts opposing right-to-repair while building their own moats.

**Tags**: `#right-to-repair`, `#FTC`, `#agriculture`, `#consumer rights`, `#John Deere`

---

<a id="item-4"></a>
## [OpenAI Tackles Noise in Coding Benchmarks](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI published an article analyzing how noise—such as ambiguous prompts or flawed tests—undermines coding evaluation benchmarks, and demonstrates methods to clean the signal using models to inspect prompts and tests at scale. This work directly impacts the reliability of AI coding benchmarks, which are critical for comparing model performance and guiding development. If benchmarks are noisy, rankings may be misleading, wasting resources on chasing false improvements. The article highlights that even widely-used benchmarks like SWE-Bench contain hidden issues; OpenAI used models to systematically detect problems in prompts, tests, and patches. They also note that evaluation flaws become easier to catch as model capabilities improve.

hackernews · sk4rekr0w · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: Coding evaluation benchmarks like HumanEval and SWE-Bench are used to measure how well AI models can write or fix code. However, these benchmarks can contain 'noise'—incorrect test cases, ambiguous problem descriptions, or even deliberate cheating (e.g., modifying timeouts). Clean benchmarks are essential for fair model comparison.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations | OpenAI</a></li>
<li><a href="https://deepeval.com/docs/benchmarks-human-eval">HumanEval | DeepEval - The LLM Evaluation Framework</a></li>
<li><a href="https://www.augmentcode.com/blog/we-benchmarked-7-ai-code-review-tools-on-real-world-prs-here-are-the-results">We benchmarked 7 AI code review tools on large open-source projects. Here are the results. | Augment Code</a></li>

</ul>
</details>

**Discussion**: The community discussion reflects mixed reactions: some appreciate OpenAI's effort to clean benchmarks, while others express skepticism about pervasive cheating and unrealistic evaluations. Commenters like 'jjcm' propose new benchmarks that combine efficiency and intelligence, while 'GodelNumbering' points out fake results and harness-level cheating.

**Tags**: `#AI benchmarks`, `#coding evaluations`, `#machine learning`, `#software engineering`, `#OpenAI`

---

<a id="item-5"></a>
## [Cloudflare Drop launches drag-and-drop deployment](https://www.cloudflare.com/drop/) ⭐️ 8.0/10

Cloudflare launched Drop, a tool that lets users deploy a static website by dragging and dropping a folder into the browser, with no account required and a 60-minute default expiration. This service dramatically lowers the barrier for quick website deployment, but the fine print grants Cloudflare a broad, perpetual license to user content, sparking significant debate about privacy and control. Deployments expire after 60 minutes unless the user explicitly claims them, and the terms of service grant Cloudflare a perpetual, irrevocable, worldwide license to submitted content.

hackernews · coloneltcb · Jul 8, 19:18 · [Discussion](https://news.ycombinator.com/item?id=48836233)

**Background**: Drag-and-drop deployment services like Netlify Drop have existed for years, allowing developers to quickly deploy static sites without complex setup. Cloudflare is a major content delivery network and cloud provider that already offers various web services, including Workers and Pages.

<details><summary>References</summary>
<ul>
<li><a href="https://app.netlify.com/signup">Sign up | Netlify</a></li>
<li><a href="https://docs.netlify.com/start/quickstarts/netlify-drop-quickstart/">Netlify Drop Quickstart | Netlify Docs</a></li>
<li><a href="https://answers.netlify.com/t/a-few-questions-about-netlify-drop-services/68469">A few questions about Netlify Drop Services - Support - Netlify Support Forums</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the ease of use and innovation, while others criticize the broad content license in the fine print and note that Netlify Drop offered similar functionality years ago. There are also concerns about Cloudflare's role as infrastructure that users pass through without opting in.

**Tags**: `#cloudflare`, `#deployment`, `#drag-and-drop`, `#web hosting`

---

<a id="item-6"></a>
## [Bun Rewrites Runtime from Zig to Rust Using AI](https://bun.com/blog/bun-in-rust) ⭐️ 8.0/10

Bun, the JavaScript runtime, announced it is rewriting its core from Zig to Rust, leveraging AI-assisted code translation to accelerate the migration. The Rust version, Bun 1.4, aims to fix memory leaks, improve stability, and reduce binary size by 20%. This migration could significantly improve Bun's reliability and performance, while the use of AI for code translation may set a precedent for large-scale software rewrites. The shift from Zig to Rust also highlights Rust's growing dominance in systems programming for memory safety and performance. The rewrite was done using an AI tool that translated Zig code to Rust, with human engineers reviewing and fixing issues. The resulting Rust version reportedly fixed a 3MB memory leak, improved stability, and achieved a 5% performance boost and 20% smaller binary without new features.

hackernews · afturner · Jul 8, 21:49 · [Discussion](https://news.ycombinator.com/item?id=48837877)

**Background**: Bun is an all-in-one JavaScript runtime and toolkit, designed as a drop-in replacement for Node.js, with built-in bundler, transpiler, and package manager. Originally built in Zig, a systems programming language focused on simplicity and performance, the project's decision to rewrite in Rust was influenced by Rust's memory safety guarantees and ecosystem maturity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.com/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed reactions: some appreciate the disciplined AI-assisted approach and cost savings, while others criticize the handling of the transition, such as abandoning LTS support for the Zig version and a 3MB memory leak left unpatched to push users to the Rust version. Some also note the rewrite inadvertently highlights Zig's shortcomings compared to Rust.

**Tags**: `#Bun`, `#Rust`, `#AI-assisted programming`, `#software engineering`, `#runtime`

---

<a id="item-7"></a>
## [Chatto Open-Sourced: Self-Hosted Chat App Now Available](https://www.hmans.dev/blog/chatto-is-open-source) ⭐️ 8.0/10

Chatto, a self-hosted chat application prioritizing ease of deployment and data privacy, has been open-sourced by developer Hendrik Mans on GitHub. This provides a practical, privacy-focused alternative to proprietary chat platforms, giving users full control over their data and infrastructure. The use of NATS messaging and S3 storage makes it scalable and modern, appealing to both individuals and organizations. Chatto ships as a compact, self-contained binary and uses NATS as its message broker with built-in stream persistence. It also supports external S3-compatible object storage and features per-user encryption keys that shred upon account deletion.

hackernews · speckx · Jul 8, 15:19 · [Discussion](https://news.ycombinator.com/item?id=48833116)

**Background**: Self-hosted applications allow users to run services on their own servers, enhancing privacy and control compared to cloud-hosted alternatives. NATS is a high-performance, open-source messaging system under the Cloud Native Computing Foundation, widely used in distributed systems. Chatto leverages NATS for lightweight messaging and persistence, simplifying deployment for self-hosters.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NATS_Messaging">NATS Messaging - Wikipedia</a></li>
<li><a href="https://nats.io/">NATS.io – Cloud Native, Open Source, High-performance Messaging</a></li>
<li><a href="https://github.com/awesome-selfhosted/awesome-selfhosted">GitHub - awesome-selfhosted/awesome-selfhosted: A list of Free Software network services and web applications which can be hosted on your own servers · GitHub</a></li>

</ul>
</details>

**Discussion**: Community feedback is mixed: many praise the ease of deployment and the developer's skill, noting that Chatto uses NATS and S3 effectively. However, some criticize the documentation for being confusing, particularly around onboarding steps like signing in or creating users, which hampers the initial experience.

**Tags**: `#open source`, `#chat`, `#self-hosted`, `#NATS`, `#privacy`

---

<a id="item-8"></a>
## [Kenton Varda Bans AI-Written Change Descriptions](https://simonwillison.net/2026/Jul/8/kenton-varda/#atom-everything) ⭐️ 8.0/10

Kenton Varda, a prominent software engineer, announced a moratorium on AI-generated change descriptions for pull requests and commits, citing that they lack necessary high-level context and are worse than useless for code review. This highlights a critical limitation of generative AI in software development: while AI can summarize code changes at a low level, it often misses the strategic intent and broader context that human reviewers need. It challenges the assumption that AI can fully automate code review documentation. Varda specifically noted that AI-written descriptions outline code details visible in the diff but omit higher-level framing needed to understand what the code is doing broadly. The moratorium applies to his team and covers change descriptions, issues, and tickets.

rss · Simon Willison · Jul 8, 20:03

**Background**: Kenton Varda is a well-known software engineer, co-creator of the Cap'n Proto serialization protocol and the Sandstorm.io platform. AI-assisted programming tools, like GitHub Copilot and ChatGPT, are increasingly used to generate commit messages and PR descriptions. However, critics argue these tools often produce verbose yet shallow summaries that fail to convey the developer's reasoning and design decisions.

**Tags**: `#ai-assisted-programming`, `#code-review`, `#generative-ai`, `#software-engineering`, `#kenton-varda`

---

<a id="item-9"></a>
## [Cloudflare and OpenAI Pilot Network Data for AI Search](https://36kr.com/newsflashes/3886946347694593) ⭐️ 8.0/10

Cloudflare and OpenAI launched a research pilot on July 8, 2025 to explore using real-time network insights from Cloudflare's global network to help AI search engines index web content more efficiently. This partnership could significantly improve the accuracy and timeliness of AI-generated answers by feeding fresh, high-quality web signals into search indexing, potentially setting a new standard for how AI systems retrieve real-time information. The pilot focuses on signals like content freshness, traffic quality, and actual page changes from participating websites on Cloudflare's network, aiming to improve AI crawling efficiency and answer relevance.

telegram · zaihuapd · Jul 8, 15:27

**Background**: AI search engines rely on web crawlers to index content, but traditional methods struggle with dynamic web pages and stale data. Cloudflare operates one of the largest global networks, handling traffic for millions of websites, and can provide real-time signals about page changes and quality. This pilot explores how such network-level intelligence can complement traditional crawling to keep AI models up-to-date.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investing.com/news/company-news/cloudflare-openai-launch-research-pilot-on-ai-search-indexing-93CH-4781484">Cloudflare, OpenAI launch research pilot on AI search indexing By Investing.com</a></li>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-announces-research-pilot-with-openai/">Cloudflare Announces Research Pilot with OpenAI | Cloudflare</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#OpenAI`, `#AI search`, `#web indexing`, `#partnership`

---

<a id="item-10"></a>
## [Researchers Identify Smartphone Apps via Electromagnetic Signals with 99% Accuracy](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

Chinese researchers have developed a non-contact forensic technique that identifies smartphone apps with up to 99.07% accuracy by analyzing leaked electromagnetic signals, even when the device is offline or locked. This side-channel attack method poses significant privacy and security implications, as it can infer app usage without access to the device's system or data, potentially enabling surveillance or forensic analysis in controlled environments. The technique was tested on iPhone 15 Pro, Xiaomi 15 Pro, and OPPO Reno 13, achieving highest accuracy on apps like Douyin, WeChat video calls, Baidu Maps, SMS, browser, camera, and cloud storage.

telegram · zaihuapd · Jul 8, 16:05

**Background**: Electromagnetic emanations from electronic devices can be captured and analyzed to infer internal operations, a technique known as TEMPEST or side-channel analysis. This research extends that approach to smartphone app identification, leveraging low-frequency signals that leak even when the device is in flight mode or encrypted.

**Tags**: `#security`, `#side-channel attack`, `#privacy`, `#electromagnetic emanation`, `#forensics`

---

<a id="item-11"></a>
## [LineageOS Introduces Browser-Based Flashing Tool](https://www.androidauthority.com/lineageos-summertime-update-2026-3685112/) ⭐️ 8.0/10

LineageOS has launched Lineage Flash Tools, allowing users to flash devices directly from a browser via WebUSB, without needing local ADB or Fastboot installations. Additionally, the Updater app receives a Material 3 redesign and LineageOS 24 (based on Android 17) is now in development. This update significantly lowers the barrier for custom ROM flashing, making it more accessible to average users by eliminating complex command-line setup. It also signals LineageOS's continued commitment to modernizing the user experience and supporting newer Android versions. The web-based tool supports Fastboot, ADB, and Samsung Odin protocols, but requires Chrome or Edge browsers with WebUSB support and must be used alongside device-specific Wiki guides. The new Updater app shows Android security patch levels before installation and uses streaming installation for A/B OTA packages to save space.

telegram · zaihuapd · Jul 9, 01:46

**Background**: LineageOS is a popular open-source custom ROM for Android devices, offering enhanced features and longer support than stock firmware. Traditionally, flashing a custom ROM required installing platform tools like ADB and Fastboot locally, which could be intimidating for beginners. WebUSB allows web applications to communicate with USB devices, enabling browser-based flashing.

**Tags**: `#LineageOS`, `#Android`, `#Custom ROM`, `#WebUSB`, `#Software Update`

---

<a id="item-12"></a>
## [National Supercomputing Internet Core Node Goes Live in Zhengzhou](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

The core node of the National Supercomputing Internet was officially launched on July 9, providing over 100,000 cards of domestic AI computing power. This launch significantly enhances China's ability to coordinate computing resources nationwide and supports the development of domestic AI ecosystems, reducing dependence on foreign hardware. The node represents the largest single pool of domestic AI computing power on the National Supercomputing Internet platform, and it will handle operations management, resource scheduling, and supply-demand integration services.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The National Supercomputing Internet is a national initiative to connect supercomputing centers across China, enabling efficient sharing of computing resources. The core node in Zhengzhou serves as a central hub for scheduling and management, facilitating coordination of distributed computing resources.

**Tags**: `#超算`, `#AI算力`, `#国产算力`, `#基础设施`, `#新闻`

---