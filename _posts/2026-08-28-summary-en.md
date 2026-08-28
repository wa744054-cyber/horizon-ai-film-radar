---
layout: default
title: "Horizon Summary: 2026-08-28 (EN)"
date: 2026-08-28
lang: en
---

> From 31 items, 13 important content pieces were selected

---

1. [Cloudflare Optimizes 1.1.1.1 DNS Cache, Saving 100 TB of Memory](#item-1) ⭐️ 9.0/10
2. [Anthropic Opens Research Preview of Model Hardware Standard for AI Agents](#item-2) ⭐️ 9.0/10
3. [Small Models Have Arrived](#item-3) ⭐️ 8.0/10
4. [Google Launches Gemini-3.5-Transcribe, a High-Accuracy Speech-to-Text Model](#item-4) ⭐️ 8.0/10
5. [Microduck: Open-Source Biped Robot Platform from Pollen Robotics](#item-5) ⭐️ 8.0/10
6. [Judge Rules Trump Administration's Blacklisting of Anthropic Illegal](#item-6) ⭐️ 8.0/10
7. [Decompiling a Nintendo 64 Game in 84 Days](#item-7) ⭐️ 8.0/10
8. [Google launches Gemini Omni 1.1 Flash with longer, 4K-capable video generation](#item-8) ⭐️ 8.0/10
9. [Prompt injection attack breaks Claude Code auto mode with 80% success](#item-9) ⭐️ 8.0/10
10. [New Benchmark HarnessOpt-Bench Tests AI's Ability to Improve Other AI](#item-10) ⭐️ 8.0/10
11. [NVIDIA Q4 Revenue Hits $68.1B, Beats Estimates; Q1 Guidance Raised to $78B](#item-11) ⭐️ 8.0/10
12. [OpenAI develops persistent Codex agent that runs until hibernated](#item-12) ⭐️ 8.0/10
13. [US Defense Department Blacklists Anthropic; Defense Firms Drop Claude](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare Optimizes 1.1.1.1 DNS Cache, Saving 100 TB of Memory](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 9.0/10

Cloudflare published a blog post detailing how they saved 100 terabytes of memory by optimizing the cache of their 1.1.1.1 public DNS resolver. The optimizations involve restructuring the in-memory representation of DNS RRsets and using more compact data structures and allocation strategies. This is significant because 1.1.1.1 is one of the world's largest public DNS services, so reducing memory usage by 100 TB lowers operational costs and energy consumption while potentially improving cache performance. The techniques showcased provide a practical reference for other engineers building large-scale, memory-constrained systems. The optimizations include inlining record data directly into CacheEntry structures, consolidating several separate lists into a single one, and leveraging arena allocation. According to the discussion, one commenter noted that merging lists could potentially undermine some of Rust's compile-time safety guarantees regarding bounds checking.

hackernews · TangerineDream · Aug 27, 17:17 · [Discussion](https://news.ycombinator.com/item?id=49468083)

**Background**: The 1.1.1.1 DNS resolver caches DNS responses as Resource Record Sets (RRsets), which group records sharing the same name and type. In a large-scale deployment, the memory footprint of these cached entries can become enormous. To reduce it, engineers used techniques such as arena allocation, which batches many small allocations into larger blocks, and xor filters, a probabilistic data structure that is more space-efficient than the widely known Bloom filter for testing set membership with no false negatives.

<details><summary>References</summary>
<ul>
<li><a href="https://support.dnsimple.com/articles/understanding-rrsets-rrsigs/">What Are RRSETs and RRSIGs in DNSSEC? - DNSimple Help</a></li>
<li><a href="https://arxiv.org/pdf/1912.08258">Xor Filters: Faster and Smaller Than Bloom and Cuckoo Filters</a></li>
<li><a href="https://en.wikipedia.org/wiki/Region-based_memory_management">Region-based memory management - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The comments generally praise the article as a well-executed example of systems-level optimization. Several readers share their own experiences with memory optimizations, such as using a single large malloc for blacklists and being mindful of struct alignment, while one commenter expresses concern that consolidating lists into one may weaken Rust's safety guarantees regarding indexing.

**Tags**: `#DNS`, `#performance`, `#memory-optimization`, `#systems-programming`, `#Rust`

---

<a id="item-2"></a>
## [Anthropic Opens Research Preview of Model Hardware Standard for AI Agents](https://www.anthropic.com/news/model-hardware-standard-research-preview) ⭐️ 9.0/10

Anthropic introduced a research preview of the Model Hardware Standard (MHS), a shared specification that lets AI agents safely operate physical devices like microscopes, liquid handlers, and robotic arms in parallel. Integration time reportedly drops from weeks or months to hours or minutes. This marks a shift from AI operating only in software to directly controlling physical hardware, potentially accelerating automation in biotech, advanced manufacturing, and quantum computing. The involvement of partners like Genentech, Carnegie Mellon, and QuEra suggests broad real-world impact. MHS works with any device that has a programmable interface, according to Anthropic. QuEra's AI controller achieved 99.3% autonomous recovery of laser lock on a quantum computer without human intervention, and Anthropic plans to open-source the standard after safety reviews.

telegram · zaihuapd · Aug 28, 01:38

**Background**: MHS began as a joint project between Anthropic and HHMI Janelia Research Campus to help AI accelerate scientific research. The standard will be developed with partners across science, robotics, electronics, and manufacturing before becoming open source. Quantum computers require precise laser locking, which historically demands painstaking manual tuning — a task well-suited for AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/model-hardware-standard-research-preview">Previewing the Model Hardware Standard \ Anthropic</a></li>
<li><a href="https://www.cnbc.com/2026/08/27/anthropic-pushes-into-physical-world-with-new-standard-to-help-ai-agents-operate-machines.html">Anthropic pushes into physical world with new standard to ...</a></li>
<li><a href="https://www.modelhardwarestandard.com/">Model Hardware Standard</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI Hardware`, `#Robotics`, `#Automation`, `#AI Agents`

---

<a id="item-3"></a>
## [Small Models Have Arrived](https://calv.info/small-models-have-arrived) ⭐️ 8.0/10

The article 'Small Models Have Arrived' argues that small, fast, and inexpensive AI models are now a practical and increasingly preferred choice for many workloads, signaling a shift away from the default reliance on frontier-scale models. This matters because it reflects a maturing AI ecosystem where cost efficiency and speed drive deployment decisions alongside raw capability, affecting developers, startups, and enterprises seeking scalable AI without prohibitive expenses. The piece distinguishes between 'IQ 180' work (rare, high-level solutions) and 'token spewer' work (high-volume, incremental tasks), arguing small models are ideal for the latter. It also notes investors are puzzled by the lack of consumer AI companies, suggesting a contrarian opportunity for product-focused builders.

hackernews · tosh · Aug 27, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49466917)

**Background**: Frontier models are general-purpose AI systems trained at extreme scale that exceed current state-of-the-art performance and exhibit emergent capabilities. Small language models (SLMs), typically with fewer than 40 billion parameters, are designed for efficient operation in resource-constrained environments such as smartphones and embedded systems, making them cheaper and faster to deploy while also reducing hallucination risks compared to larger models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_language_model">Small language model - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the thesis, sharing practical experiences of using specialized small models to cut costs and reduce hallucination, with one noting 'this seems more like a best practice.' Others discuss the distinction between high-level and high-volume work, and the potential for consumer AI companies that focus on meeting real user needs rather than competing with frontier labs.

**Tags**: `#AI`, `#small language models`, `#ML deployment`, `#cost efficiency`, `#industry trends`

---

<a id="item-4"></a>
## [Google Launches Gemini-3.5-Transcribe, a High-Accuracy Speech-to-Text Model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5-transcribe/) ⭐️ 8.0/10

Google announced Gemini-3.5-Transcribe, a new speech-to-text model that reportedly surpasses competitors in transcription accuracy. However, early community testing indicates that its latency still trails specialized real-time STT services such as Soniox and Voxtral. This release intensifies competition in the speech-to-text market, giving developers a high-accuracy option from Google while highlighting the continuing importance of low latency for real-time transcription applications. The community's rapid benchmarking suggests that accuracy alone may not be enough to win developer adoption. Community members who tested the model note that while Gemini-3.5-Transcribe beats other models on accuracy, it needs work on latency. The model also supports function calling to delegate tasks like image generation to other Gemini models, and some users worry about unintended text simplification that can alter meaning.

hackernews · k9294 · Aug 27, 18:03 · [Discussion](https://news.ycombinator.com/item?id=49468818)

**Background**: Speech-to-text (STT) models convert spoken language into written text, and real-time STT requires both high accuracy and low latency to be useful in live translation, dictation, and captioning. Competing solutions include Soniox, a real-time voice AI platform, and Voxtral, an open-source multimodal audio chat model from Mistral AI. Google's Gemini-3.5-Transcribe is part of the Gemini model family, which is designed for multimodal tasks including audio understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://soniox.com/">Soniox | Multilingual Speech AI platform: Realtime STT, TTS ...</a></li>
<li><a href="https://arxiv.org/abs/2507.13264">[2507.13264] Voxtral - arXiv.org Voxtral TTS: Free Open-Source AI Voice Generator mistralai/Voxtral-Small-24B-2507 · Hugging Face Voxtral Realtime WebGPU - a Hugging Face Space by mistralai Voxtral TTS - docs.mistral.ai</a></li>

</ul>
</details>

**Discussion**: Developers who tested the model praise its accuracy but consider latency the decisive factor, with one saying Soniox STT v5 remains the best for real-time translation. Others mention that Voxtral Mini 3b is a satisfying local model, while some users note the model can over-simplify precise wording and that the documentation for its function-calling feature is confusing.

**Tags**: `#speech-to-text`, `#Google`, `#AI models`, `#transcription`, `#machine learning`

---

<a id="item-5"></a>
## [Microduck: Open-Source Biped Robot Platform from Pollen Robotics](https://pollen-robotics.com/microduck/) ⭐️ 8.0/10

Pollen Robotics has unveiled Microduck, an open-source biped robot platform hosted on GitHub. The 25 cm robot features 15 motors, a camera, a depth sensor, two IMUs, and an articulated beak, and it moves using reinforcement learning policies. Microduck lowers the barrier for experimenting with reinforcement learning on real hardware, making humanoid-style robot research more accessible to hobbyists and academics. Because Pollen Robotics is now part of Hugging Face, the project also highlights the growing overlap between the AI/ML ecosystem and physical robotics. The simulated version defaults to an AZERTY keyboard layout (ZQSD keys) because the company is French, which some users found surprising. The robot's reinforcement learning policies are trained in MuJoCo, the physics engine maintained by Google DeepMind, before deployment to the physical robot.

hackernews · robotswantdata · Aug 27, 10:57 · [Discussion](https://news.ycombinator.com/item?id=49462763)

**Background**: Pollen Robotics is a French robotics company founded in 2016 and now part of Hugging Face, known for building expressive, open-source interactive robots. Microduck is a small biped that uses reinforcement learning (RL), a machine learning method where an agent improves its behavior through trial and error in a simulated environment. MuJoCo (Multi-Joint dynamics with Contact) is a widely used physics engine for simulating robots and training RL policies. The project aims to let researchers and makers reproduce and extend the robot's capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://pollen-robotics.com/microduck/blog/introducing-microduck/">Meet Microduck | Pollen Robotics</a></li>
<li><a href="https://github.com/pollen-robotics/microduck">GitHub - pollen- robotics / microduck : A Tiny biped duck robot</a></li>
<li><a href="https://pollen-robotics.com/">Pollen Robotics - Robots for AI builders</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters responded enthusiastically, with 586 points and 199 comments. Critiques focused on the simulator's AZERTY keyboard layout, whether the full hardware part list is truly open, and suggestions of alternative open-source robots like F1TENTH/RoboRacer, Legolas, and Tinker. Several commenters also highlighted MuJoCo's central role in robot learning, adding useful technical context.

**Tags**: `#robotics`, `#open-source`, `#simulation`, `#hardware`, `#AI`

---

<a id="item-6"></a>
## [Judge Rules Trump Administration's Blacklisting of Anthropic Illegal](https://www.nytimes.com/2026/08/27/technology/anthropic-government-blacklisting-ruling.html) ⭐️ 8.0/10

A federal judge ruled on August 27, 2026, that the Trump administration's blacklisting of AI company Anthropic was illegal. The decision marks a legal check on executive authority to place AI companies on government blacklists. The ruling strengthens legal protections for AI companies facing government scrutiny and could set a precedent for how executive actions against technology firms are reviewed. It may also shape future AI regulation by clarifying that national security justifications must meet legal standards. The ruling does not necessarily eliminate the underlying national-security concerns, and the administration could appeal. Depending on the court's remedy, Anthropic may be entitled to restored access, damages, or other relief related to the blacklisting.

hackernews · jbegley · Aug 28, 02:03 · [Discussion](https://news.ycombinator.com/item?id=49473522)

**Background**: Blacklisting is a government practice that bars a company from certain contracts, licenses, or other official dealings, often for national security reasons. Anthropic is a major artificial intelligence company that was placed on such a list by the previous administration, prompting the legal challenge that led to this ruling.

**Discussion**: Commenters were largely skeptical about the ruling's real-world impact, questioning whether illegality matters to this administration and whether the law moves too slowly to address fast-moving tech issues. Others sarcastically suggested the episode was a strategic boost for sovereign AI and self-hosting, and doubted that major players would face any negative consequences.

**Tags**: `#AI policy`, `#law`, `#Anthropic`, `#regulation`, `#government`

---

<a id="item-7"></a>
## [Decompiling a Nintendo 64 Game in 84 Days](https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/) ⭐️ 8.0/10

A developer chronicles the 84-day process of fully decompiling the Nintendo 64 game Snowboard Kids, detailing the reverse-engineering workflow and tooling used. The write-up highlights how modern tools, including LLMs, accelerated the effort. This matters because full decompilation enables community-driven preservation, modding, and ports of classic games, breathing new life into neglected titles. It also showcases a reproducible workflow that could inspire similar projects across the retro gaming ecosystem. The project reportedly achieved a 1:1 recreation of the original game code in a higher-level language, a hallmark of modern decompilation efforts. The write-up also discusses the use of LLM-assisted coding and the legal nuances of translating copyrighted executable code into open-source representations.

hackernews · knackers · Aug 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49466006)

**Background**: Game decompilation is the reverse-engineering process of examining a compiled game binary and recreating its original source code, typically in a high-level language like C. For N64 games, this allows the community to build PC ports, improve graphics, and fix bugs. LLMs have recently been used to automate and accelerate parts of this process. The legal status of decompilation projects remains debated, with concepts like clean-room reimplementation historically relevant.

<details><summary>References</summary>
<ul>
<li><a href="https://readonlymemo.com/decompilation-projects-and-n64-recompiled-list/">Decompilation projects and N64 Recompiled PC ports (August 2026)</a></li>
<li><a href="https://arxiv.org/abs/2402.18659">[2402.18659] Large Language Models and Games: A Survey and ...</a></li>
<li><a href="https://tetracorp.github.io/tokimeki-memorial/methods/what-is-decompilation.html">Exploring Tokimeki Memorial: What is decompilation ?</a></li>

</ul>
</details>

**Discussion**: Commenters celebrate the feat and point to similar projects like the Legend of Dragoon recomp, while others debate the legal status of decompilation and express surprise that game companies don't capitalize on it. Some highlight how LLM-assisted workflows turn developers into 'machines' limited only by time and tokens. A few recommend related nostalgia-driven games.

**Tags**: `#decompilation`, `#reverse engineering`, `#Nintendo 64`, `#game preservation`, `#LLMs`

---

<a id="item-8"></a>
## [Google launches Gemini Omni 1.1 Flash with longer, 4K-capable video generation](https://blog.google/innovation-and-ai/technology/developers-tools/build-with-gemini-omni-1-1-flash/) ⭐️ 8.0/10

Google released Gemini Omni 1.1 Flash, an updated version of its multimodal video generation model, now offering 40-second scene extension, starting/ending keyframe control, 360p draft previews, and 1080p or 4K output. The model is available to developers through the Gemini API and Google AI Studio. This release strengthens Google's position in AI video generation, where it continues to invest heavily while competitors like OpenAI have stepped back from similar efforts. The new creative controls make the model more practical for production workflows, which could accelerate adoption in film, advertising, and content creation, and also raises questions about its broader impact on creative professionals. Scene extension can analyze up to ten seconds of existing video and extend it in 10-second increments to a cumulative total of 40 seconds, improving visual consistency compared to earlier versions. The model also supports specifying the first and last frames of a shot, generating quick 360p drafts for iteration, and outputting full-resolution video at 1080p or 4K.

hackernews · saretup · Aug 27, 17:06 · [Discussion](https://news.ycombinator.com/item?id=49467922)

**Background**: Gemini Omni Flash is a high-performance multimodal model from Google designed for video generation and editing, offering cinematic controls via the Gemini API and Google AI Studio. Scene extension lets models build on existing clips to length a shot, while keyframe control lets creators define the starting and ending frame of a shot. The 1.1 update expands these capabilities with longer extensions, draft previews, and higher-resolution output.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/omni">Generate and edit videos with Gemini Omni Flash | Gemini API | Google AI for Developers</a></li>
<li><a href="https://the-decoder.com/googles-gemini-omni-1-1-flash-makes-ai-video-generation-cheaper-and-more-flexible/">Google's Gemini Omni 1.1 Flash makes AI video generation cheaper and more flexible</a></li>

</ul>
</details>

**Discussion**: Commenters noted the potential impact on voice and screen actors, debated Google's continued video-generation investment versus OpenAI's pivot away from Sora, and joked about missing Gemini Pro updates. One developer expressed disappointment that the model cannot sync generated video to pre-existing audio for lip-syncing, saying they use Minimax H3 locally instead.

**Tags**: `#AI`, `#Google`, `#video-generation`, `#Gemini`, `#developer-tools`

---

<a id="item-9"></a>
## [Prompt injection attack breaks Claude Code auto mode with 80% success](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 8.0/10

Security researcher Johann Rehberger demonstrated a prompt injection attack against Claude Code's auto mode that succeeds roughly 80% of the time. The attack tricks the agent into downloading and unpacking a zip archive, then executing code that unknowingly imports a malicious local struct.py file via base64's internal dependency on struct. This matters because Anthropic recently made auto mode the default in Claude Code for Pro, Max, and Team plans, relying on its classifier to protect users from prompt injection. A credible researcher showing that the safety mechanism can be bypassed — and even block Claude's own cleanup attempts — raises serious concerns about the safety of autonomous AI coding agents. The attack uses Python module shadowing: a struct.py file extracted from the zip archive takes precedence over the standard library module when base64 imports struct. In several runs, auto mode noticed the compromise but blocked the agent's command to terminate the malware process, showing the classifier itself can become part of the failure.

rss · Simon Willison · Aug 27, 22:50

**Background**: Prompt injection is an attack where carefully crafted text is hidden inside content an LLM reads, causing the model to act on instructions it should not follow. Claude Code's auto mode is a permission mode that uses a classifier to approve or block tool calls, aiming to let agents run autonomously without routine prompts. Python module shadowing occurs when a local file shares the name of a standard library module, and Python imports the local version first because the current directory is searched before installed packages.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/auto-mode-config">Configure auto mode - Claude Code Docs</a></li>
<li><a href="https://claude.com/blog/auto-mode">Auto mode for Claude Code | Claude by Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#AI security`, `#Claude Code`, `#LLM agents`, `#cybersecurity`

---

<a id="item-10"></a>
## [New Benchmark HarnessOpt-Bench Tests AI's Ability to Improve Other AI](https://www.reddit.com/r/MachineLearning/comments/1w052xg/can_ai_improve_itself_rsi_might_be_the_answer_r/) ⭐️ 8.0/10

The paper introduces HarnessOpt-Bench, a benchmark that scores an LLM on how much it improves another agent's harness, with sandbox isolation that prevents cheating by construction. It reports results from 5 frontier models, 4 downstream tasks, and 111 runs. This is a novel empirical contribution to recursive self-improvement research, a topic with high impact and safety implications. It offers a standardized way to measure whether AI systems can genuinely improve other AI systems, which is central to debates about intelligence explosion. The isolation is guaranteed by construction, not by instruction: the held-out evaluator and permission control sit outside the evolution loop. Results show Claude Opus 5 under OpenCode tops 3 of 4 tasks, and opencode beats native harnesses (Claude Code, Codex, Kimi CLI) in 11 of 20 model-task pairs.

reddit · r/MachineLearning · /u/shehio · Aug 27, 20:13

**Background**: An agent harness is the software infrastructure around an LLM that enables it to act as an AI agent, managing tool use, memory, and feedback loops. Recursive self-improvement is the hypothesized process in which an AI system rewrites its own code, potentially leading to an intelligence explosion. HarnessOpt-Bench evaluates end-to-end harness optimization under expensive and stochastic evaluation conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.06301">[2608.06301] HarnessOpt-Bench: Evaluating LLMs at Harness ...</a></li>
<li><a href="https://labs.scale.com/papers/harnessopt-bench">HarnessOpt-Bench: Evaluating LLMs at Harness Optimization</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#recursive self-improvement`, `#LLM agents`, `#benchmark`, `#machine learning`

---

<a id="item-11"></a>
## [NVIDIA Q4 Revenue Hits $68.1B, Beats Estimates; Q1 Guidance Raised to $78B](https://t.me/zaihuapd/43450) ⭐️ 8.0/10

NVIDIA reported fiscal Q4 revenue of $68.1 billion, with data center revenue of $62.3 billion, both beating analyst expectations. The company guided Q1 FY2027 sales to $78 billion, above the $72.6 billion consensus, lifting after-hours shares by over 3%. This earnings beat and raised guidance confirm that demand for AI infrastructure remains exceptionally strong, a signal that ripples across the entire AI and semiconductor supply chain. It also suggests that hyperscalers and enterprises are still aggressively deploying GPUs despite concerns about OpenAI's funding capability and competitive pressures. The data center segment contributed $62.3 billion of the $68.1 billion total, while gaming and automotive revenue missed expectations. CEO Jensen Huang cited exponential growth in compute demand and said the company took strategic steps to secure inventory against supply chain pressure.

telegram · zaihuapd · Aug 27, 08:51

**Background**: NVIDIA is the dominant supplier of GPUs used for AI training and inference, making its quarterly results a key bellwether for AI infrastructure investment. The company designs its chips but outsources manufacturing, so supply chain constraints and inventory management are critical to meeting surging demand from cloud providers and enterprises.

**Tags**: `#NVIDIA`, `#earnings`, `#AI infrastructure`, `#data center`, `#GPUs`

---

<a id="item-12"></a>
## [OpenAI develops persistent Codex agent that runs until hibernated](https://www.wired.com/story/openai-is-developing-a-persistent-ai-agent/) ⭐️ 8.0/10

According to code reviewed by WIRED, OpenAI is adding a 'persistent mode' to its Codex CLI that lets the AI agent work continuously until it is hibernated, unlike the current mode that stops after minutes or hours. OpenAI confirmed it is testing the feature but has no near-term release plans. This marks a notable step toward long-running autonomous coding agents, potentially transforming software engineering workflows by enabling developers to delegate broader, multi-session tasks. It also signals that major AI labs are pushing agentic AI beyond single-shot interactions toward continuous, goal-driven operation. The persistent mode includes an 'initiative' setting that automatically creates follow-up tasks after completing a request, and can execute these across sessions based on its understanding of the user. Changes to anything outside the user's system still require prior approval, and the mode has no confirmed launch date.

telegram · zaihuapd · Aug 28, 02:47

**Background**: Codex is an AI coding agent developed by OpenAI for software engineering tasks such as writing code and fixing bugs, released in April 2025 as Codex CLI and available via ChatGPT, desktop apps, and IDE integrations. AI agents are artificial intelligence programs that can pursue goals, use tools, and autonomously perform multi-step tasks, typically driven by large language models. Persistent mode extends the common session-bound model of such agents, allowing them to run much longer and manage their own task queue.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI agents`, `#autonomous coding`, `#software engineering`

---

<a id="item-13"></a>
## [US Defense Department Blacklists Anthropic; Defense Firms Drop Claude](https://t.me/zaihuapd/43460) ⭐️ 8.0/10

The US Department of Defense has formally designated Anthropic as a supply chain risk, marking the first time a domestic US tech company has received this label. Following the move, multiple defense tech companies instructed employees to stop using Anthropic's Claude models and switch to alternative AI tools. This is a major policy shift that could restrict Anthropic's access to defense-related contracts and set a precedent for AI regulation in the US. It also signals growing government scrutiny of AI companies' ties to national security supply chains, potentially reshaping adoption of Claude in the defense sector. Anthropic is reportedly the first US-based company to be placed on the Pentagon's supply chain risk list. Anthropic has sued the Department of Defense over the designation, according to a March 10 report. The blacklisting comes under the Trump administration and was first reported by CNBC.

telegram · zaihuapd · Aug 28, 03:15

**Background**: Anthropic is an AI startup founded in 2021 by former OpenAI researchers Dario and Daniela Amodei, focused on building safe, interpretable AI systems. Its Claude models are trained using 'constitutional AI' principles aimed at making the assistant helpful, harmless, and honest. A 'supply chain risk' designation under US defense rules typically means a company's products are barred from use in defense supply chains due to national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Anthropic">Anthropic - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.winzheng.com/article/pentagon-labels-anthropic-supply-chain-risk">官方确认：五角大楼将Anthropic列为 供 应 链 风 险 ，美 国 首家 | 赢政天下</a></li>
<li><a href="https://www.tmtpost.com/nictation/7906725.html">Anthropic就“ 供 应 链 风 险 ”认定起诉美 国 国 防 部</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI regulation`, `#national security`, `#defense technology`, `#supply chain risk`

---