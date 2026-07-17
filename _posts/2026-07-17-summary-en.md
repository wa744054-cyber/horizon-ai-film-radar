---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 42 items, 12 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Browser](#item-1) ⭐️ 9.0/10
2. [Linus Torvalds Declares Linux Not Anti-AI, Invites Fork](#item-2) ⭐️ 9.0/10
3. [Japan buys 27,500 Nvidia Rubin chips for sovereign robot AI](#item-3) ⭐️ 9.0/10
4. [Kimi K3: Open Frontier Intelligence](#item-4) ⭐️ 8.0/10
5. [LM Studio Bionic: AI Agent for Open Models](#item-5) ⭐️ 8.0/10
6. [Rust-to-Zig Compiler Rewrite: Incremental Builds & Memory Control](#item-6) ⭐️ 8.0/10
7. [GPT-5.6 Codex Bug Can Delete Files Without Sandboxing](#item-7) ⭐️ 8.0/10
8. [Inkling: An Open-Weights Multimodal MoE Model Released](#item-8) ⭐️ 8.0/10
9. [TSMC Invests $100B More in US, Q2 Profit Up 77%](#item-9) ⭐️ 8.0/10
10. [EU Proposes Mandating Android AI Assistant Access for Rivals](#item-10) ⭐️ 8.0/10
11. [1Password Integrates Claude for Secure AI Login](#item-11) ⭐️ 8.0/10
12. [Truth Social Sells Trump Post Access to Wall Street](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the Firefox browser to WebAssembly, enabling the entire browser to run inside another browser, such as Chrome, as a technical demonstration. This achievement showcases the power of WebAssembly to run complex native applications like a full browser within the browser, pushing the boundaries of web capabilities and demonstrating the potential of LLM-assisted compilation for large codebases. The project used an estimated $25,000 worth of Claude Opus and Fable tokens (though actual cost was much lower due to subscription plans) and relies on the Wisp protocol to proxy all network traffic over a WebSocket through Puter's servers. The demo supports end-to-end encryption.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a low-level binary instruction format that allows code written in other languages to run in web browsers at near-native speed. Compiling a full browser like Firefox to WASM requires overcoming significant technical challenges, including handling network access, which is typically restricted in browser sandboxes. The use of large language models (LLMs) like Claude Opus and Fable assisted in the compilation process, which is a novel approach to porting large codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#virtualization`, `#LLM`

---

<a id="item-2"></a>
## [Linus Torvalds Declares Linux Not Anti-AI, Invites Fork](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linus Torvalds, the creator and top maintainer of the Linux kernel, explicitly stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, inviting dissenters to fork the project or leave. This authoritative endorsement from Linux's top maintainer could shift community norms and encourage broader adoption of AI tools in kernel development, potentially accelerating innovation while also sparking debate about AI's role in open source. Torvalds made the remarks in a kernel mailing list post responding to criticism of AI usage, asserting that AI's utility is no longer in question and that those who disagree can fork or walk away.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is developed through a collaborative, community-driven process centered on the Linux Kernel Mailing List (LKML). Torvalds has final authority on what goes into the kernel, and his statements carry significant weight in shaping project direction and community norms.

<details><summary>References</summary>
<ul>
<li><a href="https://lore.kernel.org/">Lore Kernel - The Linux Kernel Archives</a></li>
<li><a href="https://en.wikipedia.org/wiki/Linux_kernel_mailing_list">Linux kernel mailing list - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#AI`, `#open source`, `#kernel`, `#Linus Torvalds`

---

<a id="item-3"></a>
## [Japan buys 27,500 Nvidia Rubin chips for sovereign robot AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 9.0/10

Japan announced a $2.4 billion investment to procure 27,500 Nvidia Rubin chips, led by the newly formed Noetra consortium, to build a sovereign AI foundation model for robotics, aiming to launch its first AI model by March 2027 and a robotics-specific version within a few years. This move positions Japan as a potential third AI power alongside the US and China, reducing its reliance on foreign AI technologies and aiming to capture over 30% of the global robotics market by 2040, with significant implications for the robotics and AI industries worldwide. Noetra is a consortium backed by SoftBank, Toyota-backed Preferred Networks, NEC, Sony, and Honda. The Rubin GPUs and Vera CPUs are part of Nvidia's next-generation Rubin architecture, with the Rubin Ultra variant expected in 2027.

telegram · zaihuapd · Jul 16, 10:59

**Background**: Sovereign AI refers to national efforts to build independent AI capabilities, reducing dependence on foreign providers. Japan's initiative focuses on physical AI for robots, leveraging the Rubin platform which is a multi-rack POD-scale system designed for agentic AI and AI reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/rubin/">Infrastructure for Scalable AI Reasoning | NVIDIA Vera Rubin Platform</a></li>
<li><a href="https://www.datamintelligence.com/news/japan-noetra-ai-robotics-plan-10-million-robots-by-2040">Japan Noetra AI Robotics Plan to Deploy 10... | Datam Intelligence</a></li>

</ul>
</details>

**Tags**: `#Nvidia Rubin`, `#sovereign AI`, `#Japan robotics`, `#government funding`, `#AI chips`

---

<a id="item-4"></a>
## [Kimi K3: Open Frontier Intelligence](https://www.kimi.com/blog/kimi-k3) ⭐️ 8.0/10

Moonshot AI released Kimi K3, an open-weight frontier model with 2.8 trillion parameters, priced at $3/$15 per million tokens (input/output), matching Anthropic's Sonnet pricing. As one of the largest open-weight models, Kimi K3 could accelerate the commoditization of AI, offering competitive performance at a price point comparable to leading closed models and challenging the dominance of US-based AI labs. Kimi K3 has a 1 million token context window, with cached tokens priced at $0.3 per million. Its 2.8 trillion parameter size makes it the largest open-weight model publicly available.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Open-weight models make their trained parameters publicly available, allowing download, fine-tuning, and local deployment. Frontier models are the most advanced general-purpose AI models, often requiring hundreds of millions of dollars to train. Moonshot AI is a Chinese company that has reportedly raised $500 million to develop Kimi K3.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Frontier_model">Frontier model</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights mixed views: some see Kimi K3 as a step toward AI commoditization, while others note that its pricing, though high, is justified if performance matches frontier models. Technical details such as the 13,000 reasoning tokens used in a sample render also draw attention.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#Moonshot AI`, `#frontier models`

---

<a id="item-5"></a>
## [LM Studio Bionic: AI Agent for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, a new Mac app that functions as an AI agent for open models, enabling coding and document creation tasks. The app uses an agentic harness to orchestrate language models with tools, memory, and state persistence. Bionic brings advanced agent functionality to locally run open models, combining data privacy with cost control. This release signals a shift toward practical, consumer-accessible AI agents that can operate without reliance on proprietary cloud services. Bionic supports voice input with local transcription, flexible model execution (local, LM Link, or cloud), and automatic checkpointing for document work. Users can point it to their existing LM Studio model library and run models like Qwen3.6 35B.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: An agentic harness is the software infrastructure that turns a stateless LLM into a multi-step agent by managing tool use, memory, and execution loops. LM Studio, previously a local LLM chat client, now extends into agent territory with Bionic. This concept was popularized in 2026 as 'Agent = Model + Harness'.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic: the AI agent for open models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic, a new AI agent app for open models - 9to5Mac</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>

</ul>
</details>

**Discussion**: Community response is largely positive; founder Yagil offered free credits to test with specific models. Early users praised the familiar UI and smooth setup, but requested features like system-wide file access, local web search, SSH support, and a loading indicator. Comparisons were drawn to other agent harnesses like OpenAI's Codex.

**Tags**: `#AI agents`, `#open models`, `#LM Studio`, `#local AI`, `#agentic harness`

---

<a id="item-6"></a>
## [Rust-to-Zig Compiler Rewrite: Incremental Builds & Memory Control](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The author details their experience rewriting a compiler from Rust to Zig, highlighting Zig's memory control and significantly faster incremental build times compared to Rust. This rewrite demonstrates practical trade-offs between Rust and Zig for systems programming, especially for compilers, and the debate over memory safety versus performance can influence language choice in performance-critical projects. The author notes that emitting machine code does not inherently require unsafe operations, challenging the post's assertion that compilers need memory-unsafe features, and Zig's ReleaseSafe mode catches use-after-free errors at runtime, but community members question its effectiveness for all use-after-free bugs.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Rust and Zig are modern systems programming languages. Rust emphasizes memory safety without garbage collection through ownership and borrowing, while Zig prioritizes control and simplicity with manual memory management and compile-time features. Rewriting a compiler is a substantial undertaking that highlights these language differences.

**Discussion**: Community members raised nuanced points: some argued that unsafe operations in compilers are mainly for hot patching, not general code generation; others questioned Zig's runtime safety checks for use-after-free. The discussion reflects deep engagement with the technical trade-offs.

**Tags**: `#Rust`, `#Zig`, `#compiler`, `#systems programming`, `#programming languages`

---

<a id="item-7"></a>
## [GPT-5.6 Codex Bug Can Delete Files Without Sandboxing](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI's GPT-5.6 Codex has a bug where it can accidentally delete user files when full access mode is enabled without sandboxing protections, as reported by Thibault Sottiaux. This bug poses serious safety risks for AI coding agents, potentially causing irreversible data loss and undermining trust in AI-assisted development. The bug occurs when the model attempts to override the $HOME environment variable to define a temporary directory but mistakenly deletes $HOME instead, and it is most common when auto review and sandboxing are disabled.

rss · Simon Willison · Jul 16, 17:45

**Background**: OpenAI Codex is an AI coding agent released in April 2025 that can generate and execute code. GPT-5.6 is OpenAI's latest model family, released in July 2026, with variants Luna, Terra, and Sol. Full access mode gives Codex unrestricted file system access, which combined with a lack of sandboxing can lead to dangerous behaviors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`

---

<a id="item-8"></a>
## [Inkling: An Open-Weights Multimodal MoE Model Released](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights multimodal Mixture-of-Experts model with 975B total parameters and 41B active parameters, licensed under Apache 2.0 and trained on 45 trillion tokens of text, images, audio, and video. This release strengthens the US open-weights ecosystem with a competitive multimodal base model, providing a viable alternative to models like NVIDIA Nemotron and Gemma 4, and enabling fine-tuning via the Tinker platform for customization. The model card and training data documentation are notably sparse, lacking technical depth, and the company admits Inkling is not a frontier model but rather a strong base for fine-tuning. A smaller variant, Inkling-Small (276B total, 12B active), is promised but not yet released.

rss · Simon Willison · Jul 16, 15:35

**Background**: A Mixture-of-Experts (MoE) model uses multiple specialized sub-networks (experts) and a routing mechanism to activate only a subset of parameters per input, improving efficiency without sacrificing capacity. Open-weights models allow users to download and customize the trained parameters, but typically do not include training code or full architecture details, offering more freedom than closed APIs but less than fully open-source models.

<details><summary>References</summary>
<ul>
<li><a href="https://datanorth.ai/blog/what-is-mixture-of-experts-moe-and-why-does-it-matter">What is mixture of experts (MoE) and why does it matter?</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#AI model release`

---

<a id="item-9"></a>
## [TSMC Invests $100B More in US, Q2 Profit Up 77%](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

TSMC announced an additional $100 billion investment in its Arizona factories, bringing total US investment to $265 billion. The company also reported a record Q2 net profit of $22 billion, up 77% year-over-year, driven by AI demand. This massive investment underscores TSMC's strategic shift to diversify manufacturing away from Taiwan, while the record profit highlights the explosive demand for AI chips. The move strengthens the US semiconductor supply chain and solidifies TSMC's dominance. TSMC raised its 2026 capital expenditure forecast to $60-$64 billion, and expects full-year revenue growth of slightly over 40%. Currently, eight factories are under construction or planned in Arizona, with up to four more possible.

telegram · zaihuapd · Jul 16, 12:29

**Background**: TSMC is the world's largest contract chipmaker, producing advanced processors for companies like Apple, Nvidia, and AMD. The US government has been encouraging semiconductor manufacturing on home soil through the CHIPS Act to reduce reliance on Asian supply chains.

**Tags**: `#TSMC`, `#semiconductor`, `#AI`, `#investment`, `#manufacturing`

---

<a id="item-10"></a>
## [EU Proposes Mandating Android AI Assistant Access for Rivals](https://t.me/zaihuapd/42615) ⭐️ 8.0/10

The European Union is drafting a regulation that would force Google to grant rival AI assistants, such as ChatGPT and Claude, the same system-level access on Android that Google's own Gemini receives. This regulation could significantly reshape competition in the mobile AI assistant market, potentially giving users more choice and reducing Google's dominance, but Google warns it may compromise security and privacy. The proposal is still in its draft stage and its release could be delayed, according to Bloomberg. Google has expressed concerns that opening up system access could allow malicious apps to misuse the privileges.

telegram · zaihuapd · Jul 16, 13:19

**Background**: Android is the world's most popular mobile operating system, and Google's services like the Google Assistant are deeply integrated. The EU has a history of antitrust actions against Google, including fines for tying its search and apps. This new regulation targets the emerging AI assistant space, aiming to ensure fair competition.

**Tags**: `#EU regulation`, `#Android`, `#AI assistants`, `#antitrust`, `#Google`

---

<a id="item-11"></a>
## [1Password Integrates Claude for Secure AI Login](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 8.0/10

1Password has launched an integration with Anthropic's Claude on Mac that allows the AI agent to log into websites on behalf of users, while passwords and 2FA codes are never exposed to Claude's context or memory. This integration bridges AI assistants with sensitive credential management, enabling automation without compromising security — a key step for broader AI adoption in private and enterprise workflows. Credentials are injected directly into target webpages via a secure channel, with biometric approval required per session; credentials are erased if auto-fill fails. The feature supports Mac business, family, and personal plans, and requires both 1Password and Claude desktop and browser extensions.

telegram · zaihuapd · Jul 16, 15:54

**Background**: 1Password is a popular password manager that stores credentials in an encrypted vault. Claude is an AI assistant developed by Anthropic that can perform tasks via a desktop app. Traditionally, AI agents would need to see passwords to log in, posing security risks. This integration solves that by keeping credentials out of the AI's context.

**Tags**: `#password management`, `#AI integration`, `#Claude`, `#security`, `#1Password`

---

<a id="item-12"></a>
## [Truth Social Sells Trump Post Access to Wall Street](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Trump Media and Technology Group (TMTG) announced the Truth API, a paid data service launching August 1, 2026, that provides millisecond-speed access to real-time posts from the top 10 accounts on Truth Social, primarily targeting high-frequency trading firms. This service could grant Wall Street traders an unfair information advantage by monetizing President Trump's policy announcements, raising concerns about market fairness and conflicts of interest between business and governance. The Truth API uses industry-standard delivery methods, offers 24/7 coverage, and includes a historical archive of posts dating back to 2022. Pricing has not been disclosed.

telegram · zaihuapd · Jul 17, 01:02

**Background**: High-frequency trading (HFT) firms use sophisticated natural language processing (NLP) algorithms to scan millions of social media posts per second for market-moving information. Trump has frequently used Truth Social to announce policy decisions, causing significant market volatility. Truth Social's move to sell this data follows broader trends of data monetization by social media platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.globenewswire.com/news-release/2026/07/16/3328489/0/en/Trump-Media-and-Technology-Group-Launches-Truth-API-a-New-Licensed-Data-Service-for-Financial-Services-Partners-That-Provides-the-Fastest-Access-to-Truth-Social-s-Most-Influential-.html">Trump Media and Technology Group Launches Truth API , a New</a></li>
<li><a href="https://www.oanda.com/us-en/skills-and-insights/education/fundamental-analysis/news-and-geopolitics/effect-news-social-media-trading/">Impact of social media on trading | News & geopolitics | OANDA | US</a></li>

</ul>
</details>

**Tags**: `#Data Monetization`, `#Financial Markets`, `#API`, `#Conflict of Interest`, `#Social Media`

---