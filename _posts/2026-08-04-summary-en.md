---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 53 items, 11 important content pieces were selected

---

1. [OpenAI presents ten AI-driven advances in math and theoretical CS](#item-1) ⭐️ 9.0/10
2. [LLMs Reward Expertise, Amplifying Skilled Users' Edge](#item-2) ⭐️ 8.0/10
3. [MiniMax H3 Lands on ComfyUI: Open Weights, Native Audio, 2K Video](#item-3) ⭐️ 8.0/10
4. [Andy Pavlo Joins ClickHouse to Launch ClickHouse Labs](#item-4) ⭐️ 8.0/10
5. [Pandoc Turns Twenty: Creator Reflects on Design and Community](#item-5) ⭐️ 8.0/10
6. [Jane Street's Bonsai lets OCaml developers share types across frontend and backend](#item-6) ⭐️ 8.0/10
7. [SemiAnalysis Deep-Dives Kimi K3's Novel Architecture](#item-7) ⭐️ 8.0/10
8. [Qwen3.8-Max, a 2.4T Open-Weight Model, Matches Rivals and Excels at Coding](#item-8) ⭐️ 8.0/10
9. [DeepSeek V4-Flash 284B runs at 33 tok/s on 2× RTX 3090 and used Xeon](#item-9) ⭐️ 8.0/10
10. [ASU Researchers Unlock NVIDIA CMP 170HX Miners to 80GB VRAM, Prices Surge](#item-10) ⭐️ 8.0/10
11. [Apple Photos faces $325B class action over facial data in Illinois](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI presents ten AI-driven advances in math and theoretical CS](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI published a major announcement showcasing ten notable AI-driven advances in mathematics and theoretical computer science. The post generated 801 community comments and sparked broad discussion about the role of AI in mathematical research. This matters because it signals that AI is increasingly capable of contributing to core mathematical and theoretical research, not just applied tasks. It could accelerate proof discovery and change how mathematicians work, while also raising questions about which intellectual tasks will remain uniquely human. The announcement does not provide full details of each advance in the available content, so the specific theorems or problems are not listed. The discussion focuses on whether current models can generate conjectures or merely help disprove them through brute-force computation.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**Background**: AI for mathematics involves using machine learning models to assist with tasks like theorem proving, conjecture generation, and symbolic manipulation. OpenAI and other labs have been developing systems that can reason about mathematical statements, and recent progress has made these tools more practical. Theoretical computer science also includes complex problems that AI can help explore, though human intuition still plays a key role. The community debate reflects broader uncertainty about the pace and limits of AI progress.

**Discussion**: Comments express excitement about the exponential progress of AI, with one user comparing current debates to arguing about whether we are at y-5, y, or y+5 on an exponential curve. Others note that while AI may not intuit conjectures, it can quickly disprove them through grind, echoing a Hitchhiker's Guide scenario. Some argue that any computable problem will eventually fall to computers, but that not all math is automatically solved.

**Tags**: `#AI`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#research`

---

<a id="item-2"></a>
## [LLMs Reward Expertise, Amplifying Skilled Users' Edge](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 8.0/10

Sean Gedecke's article argues that LLMs disproportionately benefit experts, reinforcing and amplifying their existing skills rather than enabling novices to produce expert-level output. This challenges the popular claim that AI levels the playing field for software development. If true, organizations and individuals need to rethink how they invest in AI tools, training, and expertise development. The argument is grounded in practical observations rather than formal experimentation, and commenters note that LLMs generalize poorly outside self-verifiable domains like coding and math. Some commenters call for formal study to rule out confirmation bias.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**Background**: Large language models (LLMs) are AI systems trained on massive text corpora to generate coherent and contextually appropriate responses to prompts. Their output quality heavily depends on how a user formulates prompts, evaluates results, and iterates, which means domain expertise and careful reasoning can create large performance differences. The article contributes to an ongoing debate about whether AI replaces or augments human skill.

**Discussion**: Comments largely support the thesis with real-world anecdotes: one user described a non-expert friend struggling with a simple web app while an expert watching could guide her, and another compared LLMs to an amplifying mirror of the user's own mindset. Others noted that RL environment startups charge frontier labs large sums because expertise is hard to embed, and one commenter said the effect needs formal study to rule out confirmation bias.

**Tags**: `#LLM`, `#AI`, `#software-engineering`, `#expertise`, `#productivity`

---

<a id="item-3"></a>
## [MiniMax H3 Lands on ComfyUI: Open Weights, Native Audio, 2K Video](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI has announced day-0 support for MiniMax H3, an open-weights omni-modal generation model that can produce video with native audio at up to 2K resolution and 15 seconds in length. The model files are repackaged on Hugging Face under Comfy-Org/MiniMax-H3 for direct use in ComfyUI workflows. This integration makes a state-of-the-art video generation model accessible to a wide audience through an open and modular node-based interface, lowering the barrier for creators and researchers. Its memory optimization and VRAM offloading allow 2K video generation to run locally on consumer GPUs such as the RTX 3060, marking notable progress in accessible AI video generation. The model's modulation weights, about 40% of total parameters, can be pruned and replaced with a lookup table, cutting memory footprint from 123.6 GB in full precision to 42.5 GB with the smallest variants — a 66% reduction. Community tests show 10-second 480p generation takes about 10 minutes on a 16 GB RTX 4070 Ti Super, with quality remaining spectacular but degrading in unusual or complex scenarios.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**Background**: ComfyUI is an open-source, node-based graphical user interface and backend for constructing modular workflows with diffusion models, enabling generation of images, videos, and audio. MiniMax H3 is a general-purpose omni-modal generation model that jointly understands text, images, video, and audio, and is designed to support true multimodal input, native audio output, and instruction-based editing in a single model. This release combines these two developments, bringing advanced video generation to a flexible open-source tool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://huggingface.co/Comfy-Org/MiniMax-H3">Comfy-Org/ MiniMax - H 3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/ComfyUI">ComfyUI</a></li>

</ul>
</details>

**Discussion**: Community reactions are largely positive, with users reporting spectacular results and decent speed on consumer GPUs, while noting noticeable slowness (10 minutes for a 10-second 480p clip on a 16 GB card) and persistent jank in non-standard scenarios like spinning a person on a wheel. Some commenters question the validity of the 'no loss in output quality' claim for pruning, asking whether the lookup-table approach could be applied to LLMs.

**Tags**: `#AI`, `#video-generation`, `#ComfyUI`, `#MiniMax`, `#open-weights`

---

<a id="item-4"></a>
## [Andy Pavlo Joins ClickHouse to Launch ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

Andy Pavlo, a prominent database researcher from Carnegie Mellon University, has joined ClickHouse to establish ClickHouse Labs, a new corporate research lab dedicated to fundamental database research. This move signals a strong industry-academia collaboration that could accelerate innovation in OLAP database systems. It also brings renewed attention to database research funding at a time when AI dominates technology investment. ClickHouse is an open-source column-oriented OLAP database known for real-time analytical queries. The new lab's specific research agenda and structure have not yet been detailed, but Pavlo's background in database systems and his popular CMU lecture series suggest a focus on core database engineering.

hackernews · nikolay_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**Background**: ClickHouse is an open-source column-oriented database management system for online analytical processing (OLAP), enabling real-time analytical reports via SQL. OLAP systems are optimized for complex queries over large datasets, typically in business intelligence. Andy Pavlo is a well-known database professor at Carnegie Mellon University who teaches a widely watched database systems course. Corporate research labs have a long history in the tech industry, from Microsoft Research to more recent industry labs, and ClickHouse Labs follows this tradition.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ClickHouse">ClickHouse - Wikipedia</a></li>
<li><a href="https://clickhouse.com/">Fast Open-Source OLAP DBMS | ClickHouse</a></li>
<li><a href="https://en.wikipedia.org/wiki/Online_analytical_processing">Online analytical processing - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community reaction is overwhelmingly positive and enthusiastic. Commenters congratulated Pavlo, expressed hope that academic database research funding gets a boost, and raised technical questions about how ClickHouse will handle decoupled compute/storage and ingestion/indexing trade-offs. Some also hope Pavlo's popular lecture series continue in a ClickHouse-sponsored format.

**Tags**: `#ClickHouse`, `#database research`, `#OLAP`, `#industry-academia collaboration`

---

<a id="item-5"></a>
## [Pandoc Turns Twenty: Creator Reflects on Design and Community](https://pandoc.org/twenty-years-of-pandoc.html) ⭐️ 8.0/10

John MacFarlane, the creator of Pandoc, published a retrospective marking the tool's twentieth anniversary, reflecting on its design choices, philosophy, and the community that shaped it. Pandoc is a foundational open-source document converter used by scholars, writers, and developers worldwide. This milestone highlights how a well-designed, long-lived tool can sustain a vibrant ecosystem and adapt to changing document formats like Typst. Pandoc's architecture uses N parsers (readers) and M renderers (writers) to support N × M conversions. It is written in Haskell and created by John MacFarlane, a philosophy professor at the University of California, Berkeley.

hackernews · fiddlosopher · Aug 3, 15:04 · [Discussion](https://news.ycombinator.com/item?id=49156750)

**Background**: Pandoc is a free and open-source universal document converter that can transform files between a wide range of markup formats, including Markdown, HTML, LaTeX, and many others. It is widely used as a writing tool, especially by scholars, and as a basis for publishing workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pandoc">Pandoc</a></li>
<li><a href="https://pandoc.org/">Pandoc - index</a></li>

</ul>
</details>

**Discussion**: Commenters expressed deep appreciation for Pandoc and admiration for its longevity. Several noted how the choice of Haskell influenced the project's contributor culture, while others shared practical uses, such as daily Markdown-to-Typst conversion or moving content between Outlook and coding tools. One commenter highlighted the contrast to modern 'vibe-coding' hype, praising Pandoc for being built correctly from basic principles.

**Tags**: `#pandoc`, `#document-conversion`, `#haskell`, `#open-source`, `#software-engineering`

---

<a id="item-6"></a>
## [Jane Street's Bonsai lets OCaml developers share types across frontend and backend](https://github.com/janestreet/bonsai) ⭐️ 8.0/10

Bonsai is Jane Street's open-source UI library for building reactive web applications in OCaml, compiled to JavaScript via Js_of_ocaml. It allows developers to use the same OCaml language and types on both the backend and frontend. It addresses the long-standing challenge of sharing code and types between server and client in OCaml, potentially making OCaml more attractive for full-stack web development. Since Jane Street uses Bonsai for almost all of its internal web applications, the library serves as a battle-tested reference for the wider OCaml ecosystem. Bonsai is partly inspired by Elm and compiles OCaml to JavaScript via Js_of_ocaml, rather than relying on the JavaScript framework ecosystem. The GitHub repository's docs directory appears to be missing, breaking links to guides; one commenter also expressed uncertainty about whether Bonsai updates the DOM directly or uses a diffing algorithm.

hackernews · KolmogorovComp · Aug 3, 08:29 · [Discussion](https://news.ycombinator.com/item?id=49152842)

**Background**: OCaml is a general-purpose, high-level, multi-paradigm programming language created in 1996 and maintained by Inria, with uses in static analysis, formal methods, systems programming, and web development. Bonsai builds on js_of_ocaml, a compiler that translates OCaml bytecode to JavaScript, enabling OCaml programs to run in browsers and Node.js. By providing an Elm-inspired reactive model, Bonsai allows Jane Street to write UI logic in the same language as its backend services.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet/bonsai: A library for building dynamic webapps, using Js_of_ocaml · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/OCaml">OCaml - Wikipedia</a></li>
<li><a href="https://numfer.com/ocsigen/js_of_ocaml">Js _ of _ ocaml : OCaml to JavaScript Compiler</a></li>

</ul>
</details>

**Discussion**: Commenters were generally positive, with one saying shared backend/frontend types are "finally possible" and another linking to a Jane Street Signals and Threads podcast episode about building the UI framework. Some raised aesthetic concerns, compared Bonsai to Melange (used by Ahrefs and other OCaml shops), and asked whether it sacrifices the JS ecosystem; others noted the missing docs and questioned the DOM update mechanism.

**Tags**: `#OCaml`, `#UI framework`, `#Jane Street`, `#functional programming`, `#web development`

---

<a id="item-7"></a>
## [SemiAnalysis Deep-Dives Kimi K3's Novel Architecture](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

SemiAnalysis published a detailed technical breakdown of Kimi K3, revealing its compressed attention (Kimi Delta Attention), attention across depth, and latent expert routing (LatentMoE). The article also analyzes K3's inference performance and memory footprint. Kimi K3's design could meaningfully reduce the memory and compute costs of running large language models, especially for long contexts and on-device inference. The breakdown gives practitioners insight into where frontier LLM architecture is heading. Kimi Delta Attention is a compressed attention mechanism similar in spirit to Multi-head Latent Attention (MLA) and aggressively cuts the per-token KV cache footprint. In Stable LatentMoE, tokens are compressed before expert dispatch and decompressed after aggregation, with an RMSNorm applied before the up-projection; a C-based implementation even streams expert weights from NVMe to run on 8GB RAM.

rss · Semianalysis · Aug 3, 19:42

**Background**: Large language models face a memory bottleneck during inference because the key-value cache grows with context length, and mixture-of-experts (MoE) models are heavy due to many expert weights. LatentMoE addresses this by decoupling the routing/expert dimension from the hidden dimension and projecting tokens into a lower-dimensional latent space before expert processing. Attention across depth, such as mixture-of-depths attention, lets attention heads read keys/values from preceding layers, which can reduce the hidden-size bottleneck and improve training efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the">Kimi K3: The Manos, The Mythos, The Legendos</a></li>
<li><a href="https://wan27.org/blog/kimi-k3-vram-guide">Kimi K3 VRAM Requirements: How Much Memory You Actually Need to Run K3 | Wan 2.7</a></li>
<li><a href="https://securityonline.info/kimi-k3-in-c/">Running Kimi K3 in C: Local AI Inference on 8GB RAM</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#Architecture`, `#Inference`, `#Memory`, `#Language Models`

---

<a id="item-8"></a>
## [Qwen3.8-Max, a 2.4T Open-Weight Model, Matches Rivals and Excels at Coding](https://www.reddit.com/r/LocalLLaMA/comments/1vellf2/qwen38max_matches_kimi_k3_and_deepseek_v4_flash/) ⭐️ 8.0/10

Qwen3.8-Max, a 2.4-trillion-parameter open-weight model, was announced with benchmark performance closely matching Kimi K3 and DeepSeek V4 Flash, while beating them in coding and software tasks. The model's weights are scheduled to be released next week. The release adds a highly capable open-weight model to the ecosystem, giving developers and enterprises a competitive alternative to major proprietary models at relatively low API prices. It could also intensify competition in coding-focused AI and accelerate adoption of open-weight technologies. The API pricing is $2.0 per million input tokens, $6.0 per million output tokens, and $0.25 per million tokens for implicit caching. A smaller Qwen3.8-27B model is also expected to become open weight soon.

reddit · r/LocalLLaMA · /u/davidthesong · Aug 3, 18:25

**Background**: Open-weight models are AI models whose core components are publicly released, allowing anyone to download, inspect, modify, and run them on their own infrastructure, although they usually do not include training code or the full training dataset. In LLM API pricing, implicit caching automatically applies a discount when repeated prompt prefixes are reused, helping to lower input costs. Qwen is an open-weight model family from Alibaba, and this announcement reflects the growing trend of extremely large open models matching closed-market competitors.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://www.digitalapplied.com/blog/prompt-caching-2026-cut-llm-costs-engineering-guide">Prompt Caching in 2026: Cut LLM Costs, Keep Quality</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#open-weight`, `#Qwen`, `#benchmarks`

---

<a id="item-9"></a>
## [DeepSeek V4-Flash 284B runs at 33 tok/s on 2× RTX 3090 and used Xeon](https://www.reddit.com/r/LocalLLaMA/comments/1veow4b/deepseek_v4flash_284b_moe_at_33_toks_single_68/) ⭐️ 8.0/10

A user ran the full official DeepSeek V4-Flash-0731 checkpoint (284B total / 13B active MoE, 156 GB) on a used Dell R940 quad-Xeon DDR4 server with 2× RTX 3090s, achieving 33 tok/s single-stream and up to 68 tok/s aggregate decode. The setup uses a vLLM fork (Lvllmds4-x v2.3.8) with the lk_moe v2.3.1 CPU-GPU hybrid engine and DSpark speculative decoding, without any re-quantization. This shows a frontier-class 284B MoE model can serve at usable speeds on roughly $6K of commodity used hardware, rather than requiring a $4K+ unified-memory workstation or expensive datacenter GPUs. It also provides rare prefill/decode numbers for Ampere (sm_86) GPUs running a Blackwell-era checkpoint, which is valuable for the local inference community. The routed experts (~96% of params) natively ship in MXFP4 and are streamed from 768 GB DDR4 by 96 Xeon cores, while FP8 linears run weight-only via Marlin kernels because Ampere lacks native FP8/FP4 compute. Resource usage is ~170 GB system RAM and 6.6 GB VRAM per card; the box draws ~1,000 W under decode, with GPUs only at ~136-145 W. Single-stream decode hits 33 tok/s, while 4 concurrent users get 53-68 tok/s aggregate; comparable ik_llama.cpp hybrid gives 12.2 tok/s single-stream.

reddit · r/LocalLLaMA · /u/AbbreviationsSad5582 · Aug 3, 20:25

**Background**: DeepSeek V4-Flash is a Mixture-of-Experts (MoE) model with 284B total parameters but only 13B activated per token, so a CPU can stream inactive experts from system memory while the GPU only handles the active ones. LLM inference has two phases: prefill (processing the prompt in parallel) and decode (generating tokens one by one), and hybrid CPU-GPU setups often only report decode numbers. DSpark speculative decoding uses 5 draft tokens to boost single-stream speeds.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek - v 4 - flash</a></li>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques: Inference Optimization | NVIDIA Technical...</a></li>

</ul>
</details>

**Discussion**: A commenter criticized the original post for reporting only decode and not prefill, a common issue with hybrid CPU-GPU benchmarks; the author acknowledged this and added prefill results, noting the prefill number determines what the hardware is actually good for. The discussion reflects a community demand for more complete and honest benchmarking.

**Tags**: `#LocalLLM`, `#DeepSeek`, `#AI Inference`, `#Hardware`, `#MoE`

---

<a id="item-10"></a>
## [ASU Researchers Unlock NVIDIA CMP 170HX Miners to 80GB VRAM, Prices Surge](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

Researchers at Arizona State University publicly disclosed a method to unlock NVIDIA CMP 170HX mining GPUs, expanding VRAM up to 80GB and boosting FP32 compute from 0.39 to 94 TFLOPS. The exploit quickly caused secondary-market prices to jump from 300-500 yuan to 3000-4000 yuan, with overseas listings reaching as high as $1500. This breakthrough turns a cheap, heavily locked mining card into a powerful AI accelerator, democratizing access to high-end compute for AI researchers, hobbyists, and small startups. It also challenges NVIDIA's hardware-enforced product segmentation and could disrupt the resale market for mining GPUs. The unlock exploits a stack overflow vulnerability in the Falcon security coprocessor to bypass NVIDIA's one-time programmable (OTP) fuse locks and modify hardware registers. Unlocked cards can run AI image generation and large language model inference on Windows and Linux, but long-term stability and maximum unlock capacity vary between different card batches.

telegram · zaihuapd · Aug 3, 11:29

**Background**: NVIDIA CMP 170HX is a cryptocurrency mining GPU launched in 2021, built around the same GA100 die as the A100 data-center accelerator. At the factory, one-time programmable (OTP) fuses permanently limited its memory, compute, and PCIe capabilities, and the cards were long considered impossible to reconfigure. Community projects have shown that with custom drivers and careful bypassing of these fuse limits, the card can be transformed into a usable AI accelerator.

<details><summary>References</summary>
<ul>
<li><a href="https://gist.github.com/luqiu732/93b54226ccb45ac0b9504b1f87d8cd11">GA100 Fuse & Register Reference Table — Full Ampere Lineup...</a></li>
<li><a href="https://ai-manual.ru/article/cmp-170hx-kak-gpu-dlya-ai-razblokirovka-64-gb-hbm2e-i-173-tflops-v-bf16/">CMP 170 HX как GPU для AI: разблокировка 64 ГБ... | AiManual</a></li>

</ul>
</details>

**Tags**: `#hardware hacking`, `#GPU`, `#AI`, `#security`, `#NVIDIA`

---

<a id="item-11"></a>
## [Apple Photos faces $325B class action over facial data in Illinois](https://appleinsider.com/articles/26/08/03/apple-photos-facial-features-prompt-a-325b-class-action-lawsuit) ⭐️ 8.0/10

On June 30, the Seventh Circuit Court of Appeals denied Apple's appeal, allowing a class action lawsuit to proceed that accuses Apple Photos of collecting facial data without consent under Illinois' Biometric Information Privacy Act (BIPA). The suit seeks up to $325 billion in damages on behalf of estimated 6.5 million Illinois residents. This is one of the largest biometric privacy lawsuits ever filed, with potential damages that could dwarf Apple's annual revenue. The outcome could set a landmark precedent for how BIPA applies to consumer software features like photo management, affecting both tech giants and millions of users nationwide. The lawsuit alleges that Apple Photos uses facial recognition to scan people in photos, generates 'face features' for each person, and syncs this data via iCloud. Apple had argued the process does not constitute a biometric identifier and that privacy protections exist, but the judge ruled the class met certification requirements, and the appeals court upheld that decision on June 30.

telegram · zaihuapd · Aug 3, 14:33

**Background**: Illinois' Biometric Information Privacy Act (BIPA), enacted in 2008, was the first U.S. law to regulate the collection and use of biometric identifiers such as fingerprints and facial scans. BIPA grants private individuals the right to sue for violations, with statutory damages of $1,000 per negligent violation and $5,000 per intentional or reckless violation. Many tech companies, including Google, have faced similar BIPA class actions over photo-tagging features. The act's definition of 'biometric identifier' is central to whether Apple's facial feature data qualifies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Biometric_Information_Privacy_Act">Biometric Information Privacy Act - Wikipedia</a></li>
<li><a href="https://www.mofo.com/resources/insights/240503-getting-bipa-right-biometric-identifiers-must-identify">Getting BIPA Right: Biometric Identifiers Must Identify | Morrison Foerster</a></li>
<li><a href="https://www.commerciallitigationupdate.com/biometric-backlash-the-rising-wave-of-litigation-under-bipa-and-beyond">Biometric Backlash: The Rising Wave of Litigation Under BIPA and Beyond | Epstein Becker Green</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Privacy`, `#Biometric Data`, `#Facial Recognition`, `#Lawsuit`

---