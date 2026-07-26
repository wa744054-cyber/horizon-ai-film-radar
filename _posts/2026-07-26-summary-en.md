---
layout: default
title: "Horizon Summary: 2026-07-26 (EN)"
date: 2026-07-26
lang: en
---

> From 31 items, 13 important content pieces were selected

---

1. [Science Reports Gene Editing Trial Death Cover-Up in China](#item-1) ⭐️ 10.0/10
2. [vLLM v0.26.0 Adds Inkling, Boosts DeepSeek-V4, Flexible Attention](#item-2) ⭐️ 9.0/10
3. [Anthropic's New Context Engineering Rules for Claude 5](#item-3) ⭐️ 8.0/10
4. [JetZero's Blended-Wing Aircraft Promises 50% Fuel Efficiency](#item-4) ⭐️ 8.0/10
5. [Running 28.9M LLM on $8 Microcontroller](#item-5) ⭐️ 8.0/10
6. [GM Invests in Sodium-Ion Batteries for U.S. Grid Storage](#item-6) ⭐️ 8.0/10
7. [Fly.io Pivots to AI Sandboxes, Replaces CEO Amid Sprite Bugs](#item-7) ⭐️ 8.0/10
8. [Ruff v0.16.0 expands default rules from 59 to 413](#item-8) ⭐️ 8.0/10
9. [YOLO26n Inference from Scratch in ARM64 Assembly](#item-9) ⭐️ 8.0/10
10. [LLMs Tested on IMO 2026: Harness Boosts Smaller Models](#item-10) ⭐️ 8.0/10
11. [Microsoft to Use TPM Chips to Block Pirated Windows Activation](#item-11) ⭐️ 8.0/10
12. [DeepSeek pauses funding round over leaked internal remarks](#item-12) ⭐️ 8.0/10
13. [Nearly 200 Silicon Valley firms urge Trump not to ban Chinese open-weight AI](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Science Reports Gene Editing Trial Death Cover-Up in China](https://t.me/zaihuapd/42777) ⭐️ 10.0/10

Science magazine published an exclusive investigation on July 23, 2026, revealing that a 6-year-old girl died in March 2025 after receiving experimental base editing gene therapy at Xinhua Hospital in Shanghai, and the incident was never publicly disclosed. This incident represents a severe breach of research ethics and regulatory oversight, potentially undermining public trust in gene therapy and highlighting the dangers of unregulated clinical trials. The girl suffered from a rare single-base mutation genetic disorder and received trillions of AAV viral vectors via intrathecal injection into the spinal fluid to target brain neurons; she died 7 days later from a severe immune reaction. Her parents paid over $800,000 out of pocket, and the ClinicalTrials.gov record has not been updated for over a year.

telegram · zaihuapd · Jul 26, 06:01

**Background**: Base editing is a genome editing technique that precisely changes single DNA bases without creating double-strand breaks. AAV (adeno-associated virus) vectors are commonly used to deliver therapeutic genes, but high doses can trigger immune responses. Intrathecal injection delivers drugs directly into the cerebrospinal fluid to bypass the blood-brain barrier. Clinical trials in China are subject to regulation, but this case reportedly bypassed proper oversight.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Base_editing">Base editing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adeno-associated_virus">Adeno-associated virus - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intrathecal_injection">Intrathecal injection</a></li>

</ul>
</details>

**Tags**: `#gene editing`, `#bioethics`, `#clinical trial`, `#regulation`, `#science misconduct`

---

<a id="item-2"></a>
## [vLLM v0.26.0 Adds Inkling, Boosts DeepSeek-V4, Flexible Attention](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 introduces support for the Inkling model family, including base modeling, piecewise CUDA graphs, and speculative decoding, and delivers significant performance improvements for DeepSeek-V4 via a specialized routing kernel and fused operations. The release also adds fp32 lm_head selection, flexible attention backends per KV-cache group, and matures KV offloading infrastructure. This release significantly expands vLLM's model support and performance optimization capabilities, making it a more versatile and efficient inference engine for the latest large language models. The Inkling family, with its Mamba-hybrid and MoE architecture, and the DeepSeek-V4 improvements will benefit a wide range of users deploying advanced LLMs in production. The Inkling model family is supported with a full stack including piecewise CUDA graph support, Hopper FA4 relative attention, MTP=1 speculative decoding, LoRA, and NVFP4 quantization. DeepSeek-V4 gains a specialized routing kernel (2.94% E2E TPOT improvement), fused_topk_bias kernel (1.5-2x speedup), and sparse decode/prefill optimizations across Nvidia, AMD, and Intel XPU.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source library for high-throughput LLM inference, known for its PagedAttention and efficient memory management. It supports many model architectures including dense transformers and mixture-of-experts (MoE). The Inkling model from Thinking Machines Lab is a Mamba-hybrid, 256-expert MoE model with multimodal capabilities. Speculative decoding techniques like Multi-Token Prediction (MTP) use a draft model to predict multiple tokens per forward pass, reducing latency. Kernel fusion combines multiple GPU operations into one to reduce memory traffic and improve performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/vllm-project_inkling-our-open-weights-model-activity-7483227870585311232-81uL">Thinking Machines Lab Releases TML Inkling 1T-Parameter Model</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/inkling/nvidia/moe/">moe - vLLM</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#inference`, `#vllm`, `#open-source`, `#performance`

---

<a id="item-3"></a>
## [Anthropic's New Context Engineering Rules for Claude 5](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic published new guidelines for context engineering in Claude 5, focusing on optimizing instructions and memory management. The community response highlights concerns about data retention limits and the reliability of AutoMemory features. These guidelines represent Anthropic's attempt to standardize effective prompting for advanced models, but community criticism reveals potential flaws that could undermine trust. The debate over data retention and automemory reliability has practical implications for AI agent development. The Claude Code tool reportedly deletes context history after 30-45 days by default, which users find problematic. Community members also note that AutoMemory makes unreliable contextual leaps, especially when reasoning traces are hidden.

hackernews · mellosouls · Jul 25, 20:42 · [Discussion](https://news.ycombinator.com/item?id=49051361)

**Background**: Context engineering refers to the process of designing and optimizing instructions and relevant context for large language models to perform tasks effectively. It encompasses managing short-term and long-term memory, including techniques like AutoMemory that aim to help AI agents recall relevant information. Anthropic's Claude 5 is a next-generation model with advanced capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://weaviate.io/blog/context-engineering">Context Engineering - LLM Memory and Retrieval for AI Agents | Weaviate</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some propose designing explicit languages for precise control, while others criticize the reliance on AutoMemory as unreliable. A user reported that Claude Code deletes context history after 30-45 days, which they consider unacceptable, while another warns that AutoMemory makes large contextual leaps that may lead to unintended decisions.

**Tags**: `#Claude 5`, `#context engineering`, `#AI prompting`, `#Anthropic`, `#LLM best practices`

---

<a id="item-4"></a>
## [JetZero's Blended-Wing Aircraft Promises 50% Fuel Efficiency](https://www.jetzero.aero/) ⭐️ 8.0/10

JetZero, founded in 2020, is developing the Z4, the world's first commercial all-wing airplane with up to 50% better fuel efficiency compared to conventional airliners. This breakthrough could significantly reduce aviation's carbon footprint, offering a viable path to net-zero emissions by 2050 while potentially lowering operating costs for airlines. The blended-wing design faces challenges such as structural pressurization, emergency evacuation, and compatibility with existing airport gates. JetZero's Z4 aims to address these with innovative solutions like large cabin screens instead of windows.

hackernews · lisper · Jul 26, 02:55 · [Discussion](https://news.ycombinator.com/item?id=49054224)

**Background**: Conventional commercial aircraft use a tube-and-wing design, which is aerodynamically less efficient. Blended-wing body (BWB) aircraft merge the fuselage and wings into a single lifting body, reducing drag and improving fuel efficiency. The concept dates back to the late 1920s in Germany but has not yet been commercialized for passenger aviation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/future/article/20251107-blended-wings-the-sci-fi-look-that-may-shape-tomorrows-airliners">Blended wings : The sci-fi aircraft concept that could appear at an...</a></li>
<li><a href="https://natilus.co/">Sustainable Aircraft for a Greener Future</a></li>
<li><a href="https://www.aol.com/jetzero-groundbreaking-blended-wing-demonstrator-095758049.html">JetZero: Groundbreaking ‘ blended - wing ’ demonstrator plane... - AOL</a></li>

</ul>
</details>

**Discussion**: The Hacker News community discussion highlights several concerns: one commenter notes that changing flight plans to avoid cloud formation could halve contrail warming effects, but this hasn't been widely adopted. Another suggests modular passenger compartments for faster boarding. A third points out challenges with pressurization, evacuation, and gate compatibility. Overall, the sentiment is cautiously optimistic about the technology but skeptical about practical implementation.

**Tags**: `#aviation`, `#sustainability`, `#aircraft-design`, `#climate-tech`, `#startups`

---

<a id="item-5"></a>
## [Running 28.9M LLM on $8 Microcontroller](https://github.com/slvDev/esp32-ai) ⭐️ 8.0/10

A project demonstrates running a 28.9 million parameter LLM on an ESP32 microcontroller costing $8, using a per-layer embedding trick to fit the model into limited memory. This breakthrough pushes the boundary of edge AI, enabling LLM inference on ultra-low-cost hardware for the first time. It could democratize AI capabilities in IoT devices and open new applications like offline voice assistants or smart sensors. The model uses a per-layer embedding trick to reduce memory footprint, making it fit on an ESP32 with only 520KB SRAM. The ESP32 is a dual-core microcontroller with Wi-Fi and Bluetooth, but no hardware accelerator for AI.

hackernews · boveyking · Jul 25, 18:59 · [Discussion](https://news.ycombinator.com/item?id=49050512)

**Background**: The ESP32 is a popular low-cost microcontroller by Espressif Systems, widely used in IoT projects. Edge AI refers to running machine learning models locally on devices rather than in the cloud. LLMs typically require powerful GPUs; running them on microcontrollers requires extreme optimization techniques like quantization and memory sharing.

<details><summary>References</summary>
<ul>
<li><a href="https://micropython.org/download/">MicroPython - Python for microcontrollers</a></li>
<li><a href="https://precisionaiacademy.com/blog/edge-ai-explained">Edge AI Explained 2026: Running ML on Tiny Devices</a></li>
<li><a href="https://zbotic.in/esp32-edge-ai-run-tensorflow-lite-micro-on-microcontroller/">ESP32 Edge AI : Run TensorFlow Lite Micro on Microcontroller - Zbotic</a></li>

</ul>
</details>

**Discussion**: Commenters found the project impressive, noting that cheap microcontrollers like Milk-V boards with more memory and TPUs exist. Some discussed combining the LLM with small TTS models for offline voice interaction. Others were more amazed by the training that produced the weights than the inference itself.

**Tags**: `#edge AI`, `#microcontroller`, `#LLM`, `#efficiency`, `#embedded ML`

---

<a id="item-6"></a>
## [GM Invests in Sodium-Ion Batteries for U.S. Grid Storage](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 8.0/10

General Motors has announced backing for sodium-ion batteries for U.S. grid storage, emphasizing potential operational savings over LFP batteries by reducing HVAC energy consumption. This investment signals growing interest in sodium-ion technology, which could lower grid storage costs and reduce lithium dependence, especially where thermal management is a major expense. Sodium-ion batteries offer stable performance over a wider temperature range than LFP, eliminating the need for expensive heating and cooling systems, but they have lower energy density and a less flat discharge voltage curve.

hackernews · rbanffy · Jul 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=49051947)

**Background**: Lithium-ion batteries, particularly LFP, dominate grid storage but require thermal management to maintain performance. Sodium-ion batteries use abundant sodium, potentially lowering costs and supply chain risks, but manufacturing lines are optimized for lithium, slowing adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_battery">Sodium-ion battery - Wikipedia</a></li>
<li><a href="https://battlebornbatteries.com/blogs/articles/sodium-ion-vs-lithium-batteries">Sodium-Ion Batteries: The Hype vs. Reality</a></li>
<li><a href="https://physics.aps.org/articles/v17/73">Physics - Sodium as a Green Substitute for Lithium in Batteries</a></li>

</ul>
</details>

**Discussion**: Commenters debate manufacturing inertia due to lithium price drops and technical trade-offs like discharge profiles. Some see HVAC savings as a strong driver, while others question GM's role and potential reliance on Chinese hardware.

**Tags**: `#sodium-ion batteries`, `#grid storage`, `#energy storage`, `#GM`, `#battery technology`

---

<a id="item-7"></a>
## [Fly.io Pivots to AI Sandboxes, Replaces CEO Amid Sprite Bugs](https://fly.io/blog/kurt-scott-money-sprites/) ⭐️ 8.0/10

Fly.io announced a strategic pivot to AI sandboxes, admitting critical bugs in their Sprite product and replacing CEO Kurt Mackey with Scott Johnston. This shift reflects the growing demand for reliable, persistent code execution environments for AI agents, a competitive space. The CEO change signals a move toward operational stability after product reliability failures. Sprites are persistent, hardware-isolated Linux microVMs that hibernate when idle and wake on demand, but initial versions suffered from data loss and zombie states. The new iteration will target AI agents and evals.

hackernews · subarctic · Jul 25, 20:43 · [Discussion](https://news.ycombinator.com/item?id=49051369)

**Background**: Fly.io is a cloud platform known for hosting Elixir apps and edge computing. Sprites are stateful sandboxes designed for running arbitrary code, competing with products like E2B and Docker Sandboxes. The company's pivot aims to capture the growing market for AI code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://fly.io/">Computers for agents · Fly</a></li>
<li><a href="https://lewoudar.medium.com/lets-talk-about-fly-io-sprites-aka-stateful-sandboxes-509796942fdd">Let’s talk about Fly . io Sprites aka stateful sandboxes | Medium</a></li>
<li><a href="https://northflank.com/blog/e2b-vs-sprites-dev">E2B vs Sprites dev: comparing AI code execution... — Northflank</a></li>

</ul>
</details>

**Discussion**: Community members reported severe reliability issues with Sprites, including data loss and inconsistent state, leading to frustration. Some view the pivot as a desperate move into a commoditized market, while others see it as a necessary adaptation to AI trends.

**Tags**: `#fly.io`, `#sprites`, `#infrastructure`, `#AI sandboxes`, `#CEO change`

---

<a id="item-8"></a>
## [Ruff v0.16.0 expands default rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 was released on July 23rd, changing its default rule set from 59 to 413 rules. This means many previously optional checks are now enabled by default, potentially breaking CI pipelines that rely on earlier configurations. This major version increase significantly impacts developer workflows by catching more severe issues like syntax errors and runtime errors without any configuration. However, it may cause existing CI pipelines to fail due to new violations, requiring project maintainers to either fix issues or update linter settings. The total number of rules in Ruff has grown from 708 to 968 since v0.1.0, and many new default rules catch issues such as 'datetime.datetime.now()' without a 'tz' argument, blind exception catching, and useless attribute access. The upgrade command 'uvx ruff@latest check . --fix --unsafe-fixes' can automatically fix many violations, as demonstrated on sqlite-utils where 1538 out of 1618 errors were fixed.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is a fast Python linter written in Rust, known for its performance and extensive rule set. Previously, only 59 rules were enabled by default, requiring users to manually enable additional rules. With v0.16.0, the Astral team expanded the default set to include many rules that catch severe issues, aiming to improve code quality out of the box.

**Tags**: `#Python`, `#linter`, `#Ruff`, `#tooling`, `#release`

---

<a id="item-9"></a>
## [YOLO26n Inference from Scratch in ARM64 Assembly](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/) ⭐️ 8.0/10

A developer implemented YOLO26n neural network inference entirely in ARM64 Assembly and C, without any framework, optimizing for edge AI on Raspberry Pi 4. This work demonstrates low-level optimization techniques (Winograd convolutions, NEON SIMD, cache-aware tiling) that can significantly accelerate CNN inference on resource-constrained devices, benefiting the edge AI community. The implementation includes custom ARM64 micro-kernels, operator fusion, and a custom binary format for model parameters, but the author notes performance gains were lower than expected and seeks feedback.

reddit · r/MachineLearning · /u/Forward_Confusion902 · Jul 26, 06:43

**Background**: YOLO (You Only Look Once) is a popular family of real-time object detection models. Winograd convolution reduces the number of multiplications in convolutional layers, and ARM NEON SIMD enables parallel data processing on ARM processors. C2PSA is a dual-branch attention module introduced in YOLOv11 to enhance feature representation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/winograd-convolution">Winograd Convolution in CNNs</a></li>
<li><a href="https://www.emergentmind.com/topics/c2psa-module">C2PSA Module: Dual-Branch Attention</a></li>
<li><a href="https://docs.ultralytics.com/guides/yolo-architecture">YOLO Architecture Explained | Ultralytics Docs</a></li>

</ul>
</details>

**Tags**: `#ARM64`, `#YOLO`, `#edge AI`, `#assembly`, `#inference optimization`

---

<a id="item-10"></a>
## [LLMs Tested on IMO 2026: Harness Boosts Smaller Models](https://www.reddit.com/r/MachineLearning/comments/1v6wskz/we_compared_different_llms_on_imo_2026_r/) ⭐️ 8.0/10

A study compared LLMs on new IMO 2026 problems, finding that frontier models (sol, fable) achieve near-perfect scores regardless of harness, while harness engineering (Claude Code, AutoFyn) significantly improves performance of smaller models like Sonnet, Opus, and GLM. This benchmark provides rigorous evidence that model scale and native reasoning ability still dominate in hard math, but harness can substantially close the gap for smaller models, guiding practical deployment of AI for complex problem-solving. Grading was performed by a frontier model and manually verified by former IMO medalists; hallucination persisted (e.g., Sonnet on P3), and no sub-frontier model solved the hardest problem's key reduction even with a 20-hour run.

reddit · r/MachineLearning · /u/pequalnp92 · Jul 26, 07:21

**Background**: The International Mathematical Olympiad (IMO) features novel, multi-step math problems that test general intelligence and are not in LLM training data. An LLM harness is a surrounding ecosystem that provides retrieval, verification, and multi-agent coordination to improve model performance on complex tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EleutherAI/lm-evaluation-harness">GitHub - EleutherAI/lm-evaluation- harness : A framework for few-shot...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://open-data-analytics.medium.com/what-is-an-agent-harness-and-why-it-decides-how-good-your-ai-agent-is-fe1c120f05af">What Is an Agent Harness , and Why It Decides How Good... | Medium</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#benchmark`, `#mathematical reasoning`, `#IMO`, `#multi-agent`

---

<a id="item-11"></a>
## [Microsoft to Use TPM Chips to Block Pirated Windows Activation](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

Microsoft announced it will add TPM-based hardware identity verification to its KMS activation system, requiring KMS servers to prove their hardware identity is certified by Microsoft before processing activation requests. This change will become mandatory starting with the next Windows Server release and will be previewed in Windows Server 2025 from August 2026. This anti-piracy measure could effectively shut down the widely used Online KMS activation methods that rely on fake KMS servers, impacting enterprise software licensing and the piracy ecosystem. However, the cat-and-mouse dynamic continues as groups like Massgrave claim to have developed bypasses like TSforge. The TPM attestation mechanism ensures that only genuine KMS hosts with properly certified hardware can activate clients. Microsoft already blocked the KMS38 exploit in 2025, and the new TPM proof could make Online KMS activations that require periodic reconnection to a fake server obsolete.

telegram · zaihuapd · Jul 25, 15:55

**Background**: A Trusted Platform Module (TPM) is a specialized chip that provides hardware-level security by storing cryptographic keys unique to a device, enabling authentication of hardware identity. KMS (Key Management Service) is a volume activation method used by enterprises to activate multiple Windows clients using a single KMS host key. Pirated activations have long exploited KMS by setting up fake KMS servers that mimic legitimate ones.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-server/get-started/kms-client-activation-keys">Key Management Services (KMS) client activation and product keys | Microsoft Learn</a></li>
<li><a href="https://www.notebookcheck.net/Microsoft-Windows-and-Office-activation-cracked-again-TSforge-introduces-a-new-more-permanent-DRM-bypass.963349.0.html">Microsoft Windows and Office activation cracked again: TSforge ...</a></li>

</ul>
</details>

**Tags**: `#TPM`, `#Windows activation`, `#DRM`, `#KMS`, `#cybersecurity`

---

<a id="item-12"></a>
## [DeepSeek pauses funding round over leaked internal remarks](https://www.bloomberg.com/news/articles/2026-07-25/deepseek-said-to-tell-backers-of-funding-pause-after-viral-posts) ⭐️ 8.0/10

DeepSeek has orally notified some prospective second-round investors to pause signing investment agreements, partly due to founder Liang Wenfeng's dissatisfaction with leaked internal discussions circulating online. This funding pause signals potential governance challenges at a major Chinese AI startup, impacting its valuation and IPO timeline, and could affect investor confidence in the broader AI sector. DeepSeek completed its first funding round in June 2026, raising $7 billion, and the paused second round aimed to raise at least 10 billion RMB at a pre-money valuation of no less than 480 billion RMB.

telegram · zaihuapd · Jul 26, 01:17

**Background**: DeepSeek is a prominent Chinese artificial intelligence company that develops large language models. The company recently secured $7 billion in its first funding round from investors including Tencent, CATL, and a national AI industry investment fund. This pause comes as the company prepares for an initial public offering, possibly filing as early as 2026.

**Tags**: `#AI`, `#DeepSeek`, `#funding`, `#business`, `#China`

---

<a id="item-13"></a>
## [Nearly 200 Silicon Valley firms urge Trump not to ban Chinese open-weight AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

Nearly 200 Silicon Valley companies, including Proton and Y Combinator, sent a letter to the Trump administration opposing a potential ban on US access to Chinese open-weight AI models. Such a ban would severely harm US startups that rely on cost-effective Chinese open-weight models, undermining their competitiveness and stifling innovation. The letter was organized by the Little Tech Association, which argues for targeted security measures instead of an outright ban. Reports of a possible ban had already caused panic in the startup community.

telegram · zaihuapd · Jul 26, 02:00

**Background**: Open-weight AI models are models whose trained parameters are publicly released, allowing anyone to download, inspect, modify, and run them on their own hardware. They are distinct from fully open-source models as the training data and code may not be included. Chinese companies like DeepSeek have produced popular open-weight models that many global startups use to build applications.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open-weight models`, `#Silicon Valley`, `#geopolitics`, `#startups`

---