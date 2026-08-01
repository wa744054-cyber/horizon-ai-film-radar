---
layout: default
title: "Horizon Summary: 2026-08-01 (EN)"
date: 2026-08-01
lang: en
---

> From 38 items, 8 important content pieces were selected

---

1. [Elevator Algorithm Deep Dive: Inefficiencies and Real-World Insights](#item-1) ⭐️ 8.0/10
2. [YC Open-Sources qm, a Multiplayer Agent Harness for Work](#item-2) ⭐️ 8.0/10
3. [Getting 25 Gbps Thunderbolt Ethernet on a Mac Studio: A Practical Guide](#item-3) ⭐️ 8.0/10
4. [Tailscale details Hugging Face intrusion via leaked reusable auth key](#item-4) ⭐️ 8.0/10
5. [Is AI Reasoning Right for the Wrong Reasons?](#item-5) ⭐️ 8.0/10
6. [DeepSeek V4 Flash: 304B model offers best value per intelligence](#item-6) ⭐️ 8.0/10
7. [MCP 2.0 Stateless Spec Reignites Interest, Sparks New Tools](#item-7) ⭐️ 8.0/10
8. [Google Confirms Paid/Free Tiers for Android 16 Developer Verification](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Elevator Algorithm Deep Dive: Inefficiencies and Real-World Insights](https://john.fun/elevators) ⭐️ 8.0/10

A new technical analysis on john.fun examines the inefficiencies of common elevator scheduling algorithms, and was widely discussed on Hacker News (1,185 points, 282 comments). The discussion expanded the analysis to parallels with disk scheduling algorithms such as SCAN. This matters because elevator scheduling is a classic real-world example of algorithm design that affects millions of people daily, and the discussion bridges to OS disk scheduling, showing how everyday systems can inform systems design. The strong community engagement also validates practical algorithm analysis as a valuable topic. The article reportedly points out inefficiencies in common elevator strategies; commenters highlight that destination dispatch can be worse, while noting that 99% of usage involves ground-floor trips. A commenter also links the SCAN algorithm to elevator behavior and mentions HDD disk scheduling.

hackernews · Jrh0203 · Jul 31, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49124218)

**Background**: The SCAN algorithm, also called the elevator algorithm, is a disk-scheduling technique where the disk arm moves in one direction, servicing requests until it reaches the end, then reverses — just like an elevator traveling up and down a shaft. In real buildings, most elevator traffic consists of trips to or from the ground floor, which can make sophisticated scheduling less beneficial than expected. Destination dispatch groups passengers by destination to reduce stops, but may perform worse under random traffic simulations, as commenters observed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/dsa/scan-elevator-disk-scheduling-algorithms/">SCAN (Elevator) Disk Scheduling Algorithms - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences: one simulated elevator algorithms in high school and noted that HDDs are like a long elevator wrapped around a spindle, while another staying in a 60-floor tower reported frequently saturated elevators. Some questioned the article's random-destination assumption, arguing that real buildings mostly see traffic to and from the ground floor. A link to the Elevator Saga game was also shared for hands-on experimentation.

**Tags**: `#elevator-algorithms`, `#disk-scheduling`, `#systems-design`, `#algorithms`, `#hackernews`

---

<a id="item-2"></a>
## [YC Open-Sources qm, a Multiplayer Agent Harness for Work](https://github.com/yc-software/qm) ⭐️ 8.0/10

Y Combinator has open-sourced QM, a multiplayer AI agent harness it uses internally for work tasks, under the MIT license. QM introduces per-person scopes and shared rooms to coordinate AI agents and humans in collaborative environments. This matters because QM offers a production-tested harness for coordinating fleets of agents across an organization, directly addressing scoping and context-sharing problems that many multi-agent systems struggle with. It could accelerate the adoption of multi-agent collaboration for real work in startups and enterprises. QM is designed for work-related tasks such as accounting, legal, and engineering at YC, and every employee or project can get an agent as needed. It is built on YC's earlier experiments with agent harnesses, uses OpenClaw-like agents, and even ships an 'anti-slop' taste skill for frontend design work.

hackernews · tosh · Jul 31, 18:04 · [Discussion](https://news.ycombinator.com/item?id=49126604)

**Background**: An AI agent harness is the software layer between a large language model and the real world: the model does the reasoning, while the harness handles orchestration, tools, memory, state, errors, identity, verification, and guardrails. YC has experimented with several harnesses over time, and QM is the result of those learnings. By open-sourcing it, YC is sharing the internal tooling it uses to run its own operations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work</a></li>
<li><a href="https://qm.ycombinator.com/index.html">QM — Open-Source Agent Harness from YC</a></li>
<li><a href="https://startupfortune.com/y-combinator-open-sources-qm-the-ai-agent-harness-it-uses-to-run-itself/">Y Combinator Open-Sources QM, the AI Agent Harness It Uses to ...</a></li>

</ul>
</details>

**Discussion**: Community reactions are largely positive but raise practical concerns. One commenter argues that a multiplayer agent harness is only useful when context and AI output do not overwhelm the team space and work asynchronously, otherwise it risks becoming a boring job scheduler. Others praise the per-person scopes and shared rooms, while noting that a true multiplayer harness needs to support other agents and MCP clients such as Cowork.

**Tags**: `#AI agents`, `#multiplayer`, `#harness`, `#collaboration`, `#open source`

---

<a id="item-3"></a>
## [Getting 25 Gbps Thunderbolt Ethernet on a Mac Studio: A Practical Guide](https://www.jeffgeerling.com/blog/2026/getting-25g-ethernet-mac-thunderbolt/) ⭐️ 8.0/10

The author published a detailed guide on achieving 25 Gbps Ethernet on a Mac Studio using Thunderbolt adapters, with practical test results and community feedback. It highlights the hardware options and performance benchmarks. This matters because high-speed networking is a bottleneck for many creative and data-intensive workflows on Macs. The guide provides a viable path for users who need faster-than-10GbE connectivity, and the community discussion reflects broader concerns about cost and macOS networking limitations. The tests used Thunderbolt-to-25GbE adapters such as Sonnet's Twin25G T5, achieving over 25 Gbps bidirectional throughput in some cases. A key limitation is macOS's lack of SMB Direct (RDMA) support, which may affect performance in certain NAS workloads.

hackernews · speckx · Jul 31, 16:15 · [Discussion](https://news.ycombinator.com/item?id=49125034)

**Background**: Thunderbolt is a high-bandwidth interface that can carry network traffic, and Macs can use Thunderbolt Bridge for networking. 25 Gigabit Ethernet (25GbE) is a fast networking standard commonly used in data centers, and adapters that connect via Thunderbolt allow Macs to use it without built-in 25GbE ports.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sonnettech.com/product/twin25gt5/overview.html">Twin25G T5 Thunderbolt 5 Adapter - SONNETTECH</a></li>
<li><a href="https://support.apple.com/guide/mac-help/ip-thunderbolt-connect-mac-computers-mchld53dd2f5/mac">Use IP over Thunderbolt to connect Mac computers - Apple Support</a></li>
<li><a href="https://astropad.com/blog/thunderbolt-bridge/">What is Thunderbolt Bridge ? A Complete Guide [2026] - Astropad</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed experiences: one praised the Sonnet adapter for work but noted the 15W upstream power limitation, while others suggested cheaper DIY alternatives like a used eGPU enclosure. There was also curiosity about whether a $400 adapter would suffice, and a suggestion that the performance issue might be due to missing RDMA support in macOS.

**Tags**: `#Thunderbolt`, `#Ethernet`, `#Mac Studio`, `#Networking`, `#Hardware`

---

<a id="item-4"></a>
## [Tailscale details Hugging Face intrusion via leaked reusable auth key](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 8.0/10

In a new blog post, Tailscale disclosed that an attacker exploited a reusable auth key leaked in Hugging Face's CI environment to enroll 181 rogue nodes into Hugging Face's tailnet. Tailscale said no vulnerability in Tailscale itself was found or exploited. The incident demonstrates that even a secure mesh VPN cannot protect an organization if long-lived credentials are mishandled. It also highlights the need for better alerting and tighter auth key controls, making it a valuable case study for security teams using Tailscale or similar tools. Among 136 credentials found in the CI environment, one reusable Tailscale auth key was used over several days to enroll nodes carrying a CI identity tag. Commenters noted that the key was not bound to origin or destination machines and that such activity should have triggered an alert.

hackernews · bluehatbrit · Jul 31, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49127306)

**Background**: Tailscale is a mesh VPN that creates a private network, called a tailnet, of devices and nodes. Auth keys are used to authenticate new nodes to a tailnet; they can be set as reusable, and Tailscale's documentation recommends using one-off keys or handling reusable keys securely to reduce risk. In CI environments, dynamically provisioned nodes often rely on such keys, making credential hygiene and key expiry critical for security.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys">Auth keys · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys/how-to/secure-auth-keys">Securely handle an auth key · Tailscale Docs</a></li>

</ul>
</details>

**Discussion**: Commenters were largely appreciative of Tailscale's transparency, though some viewed the post as effective marketing that also highlighted Hugging Face's mistake. Others called for a security checkup feature and pointed out that long-lived credentials should be scoped and bound to specific origins, arguing the intrusion was an alerting and config-hygiene failure.

**Tags**: `#security`, `#tailscale`, `#auth-keys`, `#incident-response`, `#vpn`

---

<a id="item-5"></a>
## [Is AI Reasoning Right for the Wrong Reasons?](https://www.quantamagazine.org/is-ai-reasoning-right-for-the-wrong-reasons-20260731/) ⭐️ 8.0/10

A Quanta Magazine feature investigates whether AI reasoning models genuinely reason or just pattern-match, highlighting a dispute over recent papers that critique LLM reasoning and a rebuttal from OpenAI's Sébastien Bubeck. This debate determines how we evaluate and trust AI systems in high-stakes domains like science and mathematics. If reasoning is just pattern-matching, the reliability of these models for complex tasks remains questionable. The article includes community commentary with technical perspectives, such as transformers lacking recursion and being limited by fixed network depth, which constrains reasoning. Sébastien Bubeck dismissed earlier Apple results as due to a training quirk in obsolete models.

hackernews · retupmoc01 · Jul 31, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49124358)

**Background**: AI reasoning models are a recent class of large language models designed to think step-by-step, often using chain-of-thought prompting, which instructs the model to generate intermediate reasoning steps before answering. The distinction between genuine reasoning and pattern matching is central in AI research: LLMs excel at recognizing patterns in data, but whether they truly reason, rather than reproduce reasoning-like sequences, remains contested. This article sits within that broader debate.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/chain-of-thoughts">What is chain of thought (CoT) prompting? - IBM</a></li>
<li><a href="https://forwardfuture.com/newsletter/daily/2024-11-04/can-ai-truly-reason-exploring-the-limits-of-pattern-recognition-in-llms">Can AI Truly Reason ? Exploring the Limits of Pattern ... | Forward Future</a></li>
<li><a href="https://solutiongigs.in/blog/ai-reasoning-models-explained">AI Reasoning Models Explained: When to Use... | SolutionGigs Blog</a></li>

</ul>
</details>

**Discussion**: The comments reflect several viewpoints: one user dismisses the debate as semantic navel-gazing, citing Dijkstra's analogy about submarines swimming; another criticizes Bubeck's dismissive tone toward critics; a third offers a technical explanation that transformers lack recursion and fixed depth limits reasoning, making chain-of-thought a way to emulate deeper recursion. Overall sentiment is mixed, with some seeing the debate as unproductive and others engaging in technical critique.

**Tags**: `#AI reasoning`, `#LLMs`, `#cognition`, `#semantics`, `#machine learning`

---

<a id="item-6"></a>
## [DeepSeek V4 Flash: 304B model offers best value per intelligence](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released DeepSeek-V4-Flash-0731, a 304-billion-parameter model with substantially enhanced agentic capabilities, priced at $0.14 per million input tokens and $0.27 per million output tokens. The model is now available on Hugging Face and via OpenRouter. At $0.14/$0.27 per million tokens, V4 Flash may currently be the best value-per-intelligence model on the market, ranking ahead of MiniMax M3 (428B) on the Artificial Analysis Intelligence Index. This shows that smaller, cheaper models can compete with much larger ones, potentially reshaping how developers choose models for cost-sensitive applications. The 304B-parameter model is 167GB on Hugging Face and appears to punch well above its weight. However, output quality varies heavily with reasoning effort: the default reasoning level produced a poorly drawn pelican, while setting reasoning_effort to high yielded much better results.

rss · Simon Willison · Jul 31, 23:59

**Background**: The Artificial Analysis Intelligence Index is a composite benchmark score that combines reasoning, knowledge, maths, programming, and agentic tasks, scaled from 0 to 100. Agentic capabilities refer to an LLM's ability to reason, act, and interact in dynamic environments, enabling automation of complex workflows. Value-per-intelligence is a cost-efficiency metric that divides the Intelligence Index by the cost per task, helping users compare models beyond raw benchmark scores.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://artificialanalysis.ai/models">Comparison of AI Models across Intelligence , Performance, and Price</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#AI model release`, `#Artificial Analysis`, `#Agentic AI`

---

<a id="item-7"></a>
## [MCP 2.0 Stateless Spec Reignites Interest, Sparks New Tools](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

The Model Context Protocol 2.0 (the 2026-07-28 specification), also known as Stateless MCP, was rolled out on Tuesday and marked the most significant change to the spec since its launch. Simon Willison built two new tools—mcp-explorer and datasette-mcp—to explore the simplified stateless workflow. This update greatly reduces the complexity of implementing both MCP clients and servers, making it easier to build scalable web applications without managing session state. It also rekindles interest in MCP as a safer, more auditable alternative to giving agents a full shell environment, which can be risky. The new stateless protocol replaces the legacy two-request flow (initialize + session ID, then tools/call) with a single HTTP request using headers like MCP-Protocol-Version, Mcp-Method, and Mcp-Name. mcp-explorer is a stateless Python CLI tool that can be run via uvx without installation, and Willison plans to integrate MCP into Datasette Agent and llm-coding-agent.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP is an open standard introduced by Anthropic in November 2024 to standardise how AI systems connect to external tools and data sources. Interest surged in 2025 but was partially eclipsed by Anthropic's 'Skills' feature, since an agent with terminal and curl could already do much of what MCP offered. The new stateless specification—the first major milestone since MCP was donated to the Agentic AI Foundation—removes session state and adds routing headers, making it easier to implement and scale.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/31/stateless-mcp/">Stateless MCP has recaptured my interest (and inspired mcp - explorer ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://www.solo.io/blog/mcp-stateless-spec-changes-the-engineering-details">MCP Stateless Spec Changes: The Engineering Details | Solo.io</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#AI`, `#protocol`, `#LLM`, `#developer tools`

---

<a id="item-8"></a>
## [Google Confirms Paid/Free Tiers for Android 16 Developer Verification](https://t.me/zaihuapd/42911) ⭐️ 8.0/10

Google confirmed that Android 16 will introduce a developer verification system for sideloaded apps, with a free tier requiring only email registration and a $25 paid tier matching Google Play's registration fee. The system will not publicly disclose the list of sideloading developers, but it will collect their personal information. This change alters how Android users sideload apps and could disrupt open-source stores like F-Droid that rely on unverified distribution. It also raises privacy and censorship concerns because Google will collect developer personal data without disclosing who has been verified. All sideloading developers must register their app package names and signing keys with Google. Verification is performed in the cloud and may require network connectivity; the free tier imposes install limits, while the paid tier removes them.

telegram · zaihuapd · Aug 1, 03:08

**Background**: Sideloading on Android means installing APK files outside the Google Play Store, a common way to get apps not listed there. F-Droid is a well-known open-source app repository that only distributes free and open-source software, so mandatory developer verification could disrupt how it operates. Android package names and signing keys are used to identify and validate the source of an app.

<details><summary>References</summary>
<ul>
<li><a href="https://android-developers.googleblog.com/2026/03/android-developer-verification.html">Android Developers Blog: Android developer verification: Balancing openness and choice with safety</a></li>
<li><a href="https://www.androidauthority.com/android-developer-verification-rollout-sideloading-flow-3653395/">Android's new developer verification rollout begins, sideloading changes are next</a></li>
<li><a href="https://en.wikipedia.org/wiki/F-Droid">F - Droid - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Android`, `#developer verification`, `#sideloading`, `#privacy`, `#F-Droid`

---