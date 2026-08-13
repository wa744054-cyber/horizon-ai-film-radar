---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 32 items, 10 important content pieces were selected

---

1. [Spaghettifying DRAM: New Attack Scrambles Memory to Expose Hidden CPU Regions](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 Released with 1.7T Open-Weight Model](#item-2) ⭐️ 9.0/10
3. [DeepMind's SL2T sign language-to-text model debuts on Pixel 11](#item-3) ⭐️ 9.0/10
4. [DeepSeek Open-Sources Harness, Releases V4-Pro-0813 Weights](#item-4) ⭐️ 9.0/10
5. [Google Launches Gemini 3.7 Flash with Vision-to-HTML Prowess](#item-5) ⭐️ 8.0/10
6. [Cerebras and OpenAI unveil GPT-5.6 Sol Ultrafast with 7x faster inference](#item-6) ⭐️ 8.0/10
7. [Choose Boring Technology: Spend Innovation Tokens Wisely](#item-7) ⭐️ 8.0/10
8. [DeepSeek Releases Developer Preview of Open-Source Agent Harness](#item-8) ⭐️ 8.0/10
9. [Pixel metrics can't rank world models on robot video; open-source tool diagnoses why](#item-9) ⭐️ 8.0/10
10. [OpenAI Rolls Out GPT-5.6 with Think Button, Expands Free Access](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Spaghettifying DRAM: New Attack Scrambles Memory to Expose Hidden CPU Regions](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas released 'skitter-creek-bath-salts', a hardware security tool that rewrites the DRAM controller's physical address translations to scramble memory. The technique, demonstrated on AMD Family 16h CPUs, can bypass higher-level protections and expose hidden regions such as the Platform Security Processor, System Management Mode, and CPU microcode. This matters because DRAM address decoding was long assumed to be a trusted abstraction; exposing it turns the memory controller into an active attack surface. If exploitable on current CPUs, it could undermine memory isolation and reveal secrets normally protected by negative-ring hardware, reshaping how we think about hardware security. The attack flips a single bit in the memory controller and uses linear algebra to reconstruct the proprietary DRAM address scrambling. It is demonstrated on AMD Jaguar (Family 16h) from 2013; notes mention Zen 3 has a different memory controller base address, so the exact attack surface on newer CPUs remains unclear.

hackernews · matt_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**Background**: DRAM address decoding is the process that maps a CPU's physical address to specific row, column, and bank coordinates inside memory chips. Modern memory controllers apply proprietary scrambling to this mapping, partly for signal integrity and partly to hide details from software. By poking the controller, an attacker can make addresses land outside their intended physical locations, potentially reaching regions like SMM, PSP, or microcode that normally live in negative-ring territory.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">Spaghettifying DRAM</a></li>
<li><a href="https://zeli.app/en/story/49286341">Spaghettifying DRAM: Unlock Everything on the CPU | Zeli</a></li>
<li><a href="https://upstract.com/x/201aa8130cc32a64">Spaghettifying DRAM - upstract.com</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic, praising Christopher Domas and looking forward to his Black Hat talk. Some raised questions about the practical scope: the attack is demonstrated on 2013-era AMD Jaguar, and it remains unclear how far it extends to Zen 3 or other modern CPUs. Others noted that although reaching ring 0 on consoles like Xbox or PlayStation is difficult, once achieved this technique would open up everything.

**Tags**: `#security`, `#DRAM`, `#hardware`, `#exploitation`, `#reverse-engineering`

---

<a id="item-2"></a>
## [DeepSeek V4 Pro 0813 Released with 1.7T Open-Weight Model](https://simonwillison.net/2026/Aug/12/deepseek-v4-pro-0813/) ⭐️ 9.0/10

DeepSeek V4 Pro 0813 is now available via OpenRouter API, with open weights released on Hugging Face (1.7T parameters, 893 GB). Simon Willison reported that no official announcement page exists yet. This is a major open-weights release of a large language model, continuing DeepSeek's pattern of timely releases. It gives developers and researchers access to a 1.7T parameter model via API and downloadable weights, which is significant for the AI community in China and globally. The Hugging Face release is 893 GB in size, indicating a massive model. Simon Willison noticed that different reasoning levels (low, medium, high) produced very different image outputs, an unusual behavior compared to other models. Benchmarks were shared through the Official DeepSeek WeChat Group and then reposted on Hacker News after a Reddit post was deleted.

rss · Simon Willison · Aug 12, 23:59

**Background**: DeepSeek is a Chinese AI company known for releasing powerful open-weights language models, such as DeepSeek V3 and V4 series. Open-weights models allow developers to download and modify the model parameters, enabling local deployment and fine-tuning, in contrast to closed API-only models. OpenRouter is a unified API gateway that provides access to hundreds of models from different providers, making it convenient for comparing and using AI models. In 2026, DeepSeek continues to release updates like V4 Pro and V4 Flash, making these weights available to the public.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/openrouter">OpenRouter API and Models | OpenRouter</a></li>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open - Weights Model? | AI 21</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#open-weights`, `#ai`, `#machine-learning`

---

<a id="item-3"></a>
## [DeepMind's SL2T sign language-to-text model debuts on Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 9.0/10

Google DeepMind has released SL2T, a large-scale multilingual sign language-to-text model, and deployed it in Gboard and Live Transcribe on the Pixel 11. The model currently supports American Sign Language (ASL) to English translation. This marks the first time sign language AI has been integrated into consumer smartphones, giving Deaf and hard of hearing users a voice-dictation equivalent. It sets a precedent for accessibility features in mainstream devices and could expand to more languages and platforms. The model was trained on over 100,000 hours of data covering more than 50 sign languages, and achieves a zero-shot score of 70 BLEURT on the FLEURS-ASL benchmark. For privacy, it processes only hand and body pose keypoints rather than raw video.

telegram · zaihuapd · Aug 13, 08:55

**Background**: FLEURS-ASL is a benchmark dataset extending the FLORES/FLEURS multilingual parallel corpora to American Sign Language as video. BLEURT is a learned evaluation metric for natural language generation that scores how well a candidate text matches a reference. Sign language-to-text AI has lagged behind speech and text translation, largely due to a lack of large-scale training data and benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://arxiv.org/abs/2408.13585">[2408.13585] FLEURS-ASL: Including American Sign Language in Massively Multilingual Multitask Evaluation</a></li>
<li><a href="https://www.techtimes.com/articles/324242/20260813/sign-language-dictation-reaches-smartphones-last-via-googles-gloss-free-ai.htm">Sign Language Dictation Reaches Smartphones at Last, via ...</a></li>

</ul>
</details>

**Tags**: `#DeepMind`, `#sign language AI`, `#accessibility`, `#Pixel`, `#NLP`

---

<a id="item-4"></a>
## [DeepSeek Open-Sources Harness, Releases V4-Pro-0813 Weights](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 9.0/10

DeepSeek published its Harness application as open source under the MIT license and made the DeepSeek-V4-Pro-0813 model weights available on Hugging Face. The Harness developer preview implements an 'everything is a plugin' architecture powered by the Cordis framework, with four run modes: Standard, PTC, Minimalist, and Creative. This is a significant milestone for the AI/ML community because it lowers the barrier for building custom agent harnesses and gives researchers access to a powerful new model. The plugin architecture enables developers to swap models, tools, and UI components without forking the codebase, potentially accelerating agent-engineering workflows. The project is packaged as an npm package (`@deepseek-ai/dsh`) with source code on GitHub, and capabilities such as sessions, sandboxes, storage, scheduling, and UI are all implemented as replaceable plugins. The DeepSeek-V4-Pro-0813 page on Hugging Face briefly returned a 404 earlier before being restored, suggesting possible deployment hiccups.

telegram · zaihuapd · Aug 13, 12:39

**Background**: An agent harness is the runtime environment that orchestrates an AI agent's interactions with models, tools, and external services. DeepSeek Harness (dsh) is built on Cordis, a plugin framework that handles mounting, unmounting, and dependency resolution of plugins, and its design is described in 'A Programming Paradigm for Spatiotemporal Composability'. The MIT license allows commercial and personal use with few restrictions, which is why the release has drawn broad attention.

<details><summary>References</summary>
<ul>
<li><a href="https://www.deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">DeepSeek Harness - GitHub</a></li>
<li><a href="https://deepseek-harness.github.io/deepseek-harness/en/reference/cordis-primer">Cordis Primer | DeepSeek Harness</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#open-source`, `#AI`, `#Hugging Face`, `#model release`

---

<a id="item-5"></a>
## [Google Launches Gemini 3.7 Flash with Vision-to-HTML Prowess](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

Google released Gemini 3.7 Flash, its latest workhorse AI model, with improved reasoning, customizable thinking levels, and notably strong vision-to-HTML performance. Pricing starts at $0.375 per million input tokens and $1.875 per million output tokens on OpenRouter, with an introductory rate that will double on December 31, 2026. This release intensifies competition in the AI model market, especially as community tests validate Gemini's strong vision-to-HTML capabilities at a lower price point than rivals. Developers seeking cost-effective, high-volume text and vision tasks may increasingly adopt Flash models, disrupting the prevailing pricing structures of competing large language models. Gemini 3.7 Flash features a 1,048,576-token context window and maximum output of 65,536 tokens, and supports low, medium, and high thinking configurations. The model card describes enhancements to its core reasoning foundation, and community comments note it arrived just three weeks after Gemini 3.6 Flash, making the introductory pricing timeline feel unusual.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**Background**: Gemini Flash models are designed as fast, cost-efficient 'workhorses' for high-volume tasks like summarization, parsing, and agentic workflows. Vision-to-HTML is a benchmark where models convert an image or screenshot into functional HTML code, a task useful for web prototyping and accessibility; Gemini has historically performed well at it. The 3.7 Flash model card notes it is the next iteration in the Gemini 3 family, with improvements in multi-step planning and tool-calling fidelity.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://openrouter.ai/google/gemini-3.7-flash">Gemini 3 . 7 Flash - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3 . 7 Flash - Model Card — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but engaged. One tester (jjcm) found Opus 5 remains best-in-class for image-to-HTML, though Gemini 3.7 offers surprisingly good results for its price; another (simonw) called the introductory-pricing schedule 'really weird' and noted the quick succession of 3.6 and 3.7 releases. Others compared it against GPT-5.6 Luna, arguing Luna is cheaper and performs better on DeepSWE 1.1, while one commenter noted the benchmarks position it as more of a Terra competitor than a Luna one.

**Tags**: `#Google Gemini`, `#AI model release`, `#LLM`, `#benchmarks`, `#pricing`

---

<a id="item-6"></a>
## [Cerebras and OpenAI unveil GPT-5.6 Sol Ultrafast with 7x faster inference](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras and OpenAI announced GPT-5.6 Sol Ultrafast, a new service tier powered by Cerebras hardware that runs GPT-5.6 Sol up to 14x faster than standard processing, achieving roughly 7x faster inference on frontier benchmarks like HLE. The preview is launching first in the OpenAI API. This marks a significant step in LLM inference speed, potentially enabling real-time AI applications in incident response, customer service, financial analysis, and e-commerce. It also highlights the growing importance of hardware-software co-design, with Cerebras' wafer-scale engine challenging NVIDIA's dominance in AI acceleration. OpenAI says Ultrafast generates up to 750 output tokens per second, up to 14x faster than Standard processing. The collaboration delivers comparable accuracy on the 2,500-question HLE benchmark in 11 hours 11 minutes, versus 78 hours 27 minutes for Claude Fable 5, though community members note there is no explicit confirmation of identical output quality to the regular GPT-5.6 Sol.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**Background**: Cerebras builds wafer-scale engines (WSE), the world's largest AI processors, such as the CS-3 with 900,000 AI-optimized cores and 44GB of on-chip SRAM. The Ultrafast tier is part of a broader trend where AI labs like OpenAI and Anthropic offer accelerated versions of their models, with OpenAI positioning this as 'more useful work per second.'

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT-5.6 Sol at up to 14X the speed | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/08/13/openai-introduces-ultrafast-a-new-mode-that-makes-gpt-5-6-sol-work-at-14x-the-speed/">OpenAI introduces 'Ultrafast,' a new mode that makes GPT-5.6 Sol work at 14x the speed | TechCrunch</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive but cautious. Some users praise the speedup's potential to enable iterative thinking, while others (e.g., Topfi) point out that neither Cerebras nor OpenAI explicitly states Ultrafast performs identically to the standard GPT-5.6 Sol, suggesting that if it were 1:1, they'd 'scream that off the rooftops.' Another commenter notes the absence of pricing info, implying it might be expensive or still gauging interest.

**Tags**: `#AI`, `#LLM`, `#Inference`, `#Hardware`, `#OpenAI`

---

<a id="item-7"></a>
## [Choose Boring Technology: Spend Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

Dan McKinley's 2015 essay 'Choose Boring Technology' argues that companies should prefer well-understood, 'boring' technologies to conserve limited 'innovation tokens' for areas where novelty truly matters. The essay has become a classic, highly influential piece on technology choice and risk management. The essay gives engineering leaders a memorable mental model for making and explaining technology tradeoffs, balancing innovation against operational risk. It remains highly relevant, especially in the age of AI-generated code, where boring technology makes AI outputs easier to review and verify. McKinley proposes that every company starts with about three 'innovation tokens,' spending one each time it adopts a novel technology, while boring choices cost nothing. He recommends saving tokens for the few areas that are genuine differentiators for the business.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**Background**: McKinley developed the idea while working at Etsy, where the engineering team was known for high productivity despite, or because of, favoring proven technologies. The 'innovation tokens' metaphor has since been widely adopted and debated, with some practitioners using it to guide technology decisions and others criticizing it as overly simplistic.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/technical-debt-innovation-tokens-case-boring-technology-jeffrey-henry-lhexe">Technical Debt, Innovation Tokens , and the Case for Boring...</a></li>
<li><a href="https://blog.glyph.im/2024/07/against-innovation-tokens.html">Deciphering Glyph :: Against Innovation Tokens</a></li>
<li><a href="https://mattrickard.com/innovation-tokens">Innovation Tokens | Matt Rickard</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive, with NickNaraghi calling the innovation-token concept one of the most useful ideas in his career as a product and engineering leader. However, some pushed back, such as insanitybit, who argued the token model is arbitrary and that 'new' is only a weak proxy for tradeoffs. Others, like theptip, noted that in the age of agents, teams might want to spend all their tokens on agents to gain leverage.

**Tags**: `#technology-strategy`, `#engineering-culture`, `#software-architecture`, `#innovation`, `#decision-making`

---

<a id="item-8"></a>
## [DeepSeek Releases Developer Preview of Open-Source Agent Harness](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek released an MIT-licensed developer preview of DeepSeek Harness, an open-source agent harness with traceable session logs and hot-reloadable plugin capabilities. This release from a major AI lab directly addresses the growing need for observability and flexibility in AI agent tooling. The traceable session logs and dynamic plugin system could make agent development significantly more transparent and maintainable across the ecosystem. The harness uses an append-only session log that records everything the model sees, including system prompts, reasoning, tool calls, and results, viewable in a Trajectory view. The plugin system is built on Cordis v4, supporting hot-reload and full state/side-effect cleanup on unload.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**Background**: An agent harness is the software infrastructure around an LLM that enables it to act as an agent: it manages tool use, memory, state persistence, execution environments, and feedback loops. Because LLMs are stateless and produce only text, the harness is what lets models take multi-step actions, use external tools, and sustain long-running tasks. This release is aimed at developers building such agentic systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://harness-engineering.ai/blog/agent-harness-complete-guide/">The Complete Guide to Agent Harness: What It Is and Why It ...</a></li>

</ul>
</details>

**Discussion**: Community reaction was positive, with commenters praising the append-only session log as a 'killer feature' and noting that, unlike some US models, traces are not encrypted or obfuscated. A DeepSeek Harness author confirmed it is an early developer preview with expected rough edges and invited feedback. Others discussed the Cordis v4 foundation and compared the framework to existing libraries like Bytedance's Eino.

**Tags**: `#DeepSeek`, `#AI agents`, `#developer tools`, `#open source`, `#LLM`

---

<a id="item-9"></a>
## [Pixel metrics can't rank world models on robot video; open-source tool diagnoses why](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

The author released worldproof, an open-source diagnostic tool that compares world-model rollouts against ground truth and physical invariants. Validation with a trivial last-frame copy baseline on real robot videos showed the baseline achieves near-perfect SSIM (0.983) and PSNR (53.9 dB) scores with flat error across horizons, proving these pixel metrics cannot rank models in such settings. This finding challenges the common practice of using SSIM and PSNR to evaluate video prediction and world models, especially on real robot data. It indicates that evaluation setups with high frame rates relative to task speed lack discriminative power, which could push the community toward more meaningful evaluation windows and diagnostic metrics. On a real SO-101 arm recording at 30fps with 64 rollouts and a 6-step horizon, the score-only-on-dynamic-regions baseline reached 0.983 SSIM and 53.9 dB PSNR with no error growth over steps. On DROID footage out to 48 steps, SSIM fell monotonically only between roughly steps 4–24, then floored around 0.20, suggesting a usable evaluation window of about 8–24 steps; LPIPS failed to separate the datasets and pointed the other way in the masked variant.

reddit · r/MachineLearning · /u/georgia_bucea · Aug 13, 19:58

**Background**: World models are machine learning systems that learn an internal representation of an environment and predict how it changes in response to actions, often to support planning and reasoning in agents. SSIM and PSNR are classic image similarity metrics, but they are known to correlate poorly with perceptual quality and can be insensitive to meaningful differences when scenes are nearly static. In high-frame-rate robot videos, predicting the next few frames may be nearly as easy as copying the last frame, so any model that simply predicts 'nothing changes' can score almost perfectly, leaving no room to rank more sophisticated models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Structural_similarity_index_measure">Structural similarity index measure - Wikipedia</a></li>
<li><a href="https://uk.mathworks.com/help/images/ref/psnr.html">psnr - Peak signal - to - noise ratio ( PSNR ) - MATLAB</a></li>

</ul>
</details>

**Tags**: `#world models`, `#evaluation metrics`, `#robotics`, `#open-source`, `#machine learning`

---

<a id="item-10"></a>
## [OpenAI Rolls Out GPT-5.6 with Think Button, Expands Free Access](https://t.me/zaihuapd/43176) ⭐️ 8.0/10

OpenAI has announced the GPT-5.6 model series, giving Plus and Pro subscribers access to GPT-5.6 Sol with more reliable factual answers and a slider to control thinking depth. Free users will default to GPT-5.6 Luna this week, gain unlimited text conversations next week, and receive a new Think button for complex reasoning tasks. This update brings advanced reasoning features to a broader audience, especially free users, and signals OpenAI's push to balance model capability with cost efficiency. Expanding free unlimited text access could significantly boost ChatGPT's user engagement and intensify competition among AI assistants. The GPT-5.6 series reportedly includes three tiers: Sol (flagship, for paid users), Terra (balanced), and Luna (fast and low-cost, for free users). Internal evaluations suggest Luna shows fewer factual errors than previous models on finance, medical, and legal questions, and the new Think button explicitly triggers deeper reasoning.

telegram · zaihuapd · Aug 13, 17:04

**Background**: OpenAI regularly updates ChatGPT's underlying models, and the GPT-5.6 series appears to be a multi-tier release allowing different trade-offs between intelligence, speed, and cost. The Think button was previously introduced on reasoning models like o1, letting users explicitly request step-by-step thinking before answering. The Luna tier reportedly uses lower per-token pricing, making it well-suited for high-volume or free usage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/gpt-5-6-luna">GPT - 5 . 6 Luna : OpenAI ' s fastest, cheapest model tier... | eesel AI</a></li>
<li><a href="https://qcode.cc/en/gpt-5-6-guide">GPT - 5 . 6 Sol , Terra & Luna — Benchmarks, Pricing... | QCode.cc</a></li>
<li><a href="https://appleinsider.com/articles/26/08/06/new-chatgpt-version-has-a-think-button-will-find-more-reliable-facts">New ChatGPT version has a 'Think' button, will find 'more reliable facts'</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#ChatGPT`, `#AI model release`, `#Free access`

---