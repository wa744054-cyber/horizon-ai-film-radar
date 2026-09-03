---
layout: default
title: "Horizon Summary: 2026-09-03 (EN)"
date: 2026-09-03
lang: en
---

> From 33 items, 7 important content pieces were selected

---

1. [OpenAI unveils GPT-6 Astra with near-perfect ARC-AGI-3 score](#item-1) ⭐️ 9.0/10
2. [ICANN and Verisign Propose Terminating Third-Level .name Domains](#item-2) ⭐️ 8.0/10
3. [1993 Amiga Assembly Game Ported to Godot With an LLM in One Evening](#item-3) ⭐️ 8.0/10
4. [Go Grandmaster Shin Jinseo Beats AI KataGo with Two-Stone Handicap](#item-4) ⭐️ 8.0/10
5. [Audacity 4.0 Launches With Qt6 UI, Drawing Praise and Criticism](#item-5) ⭐️ 8.0/10
6. [Polars 2.0 pre-release removes legacy constraints, changes defaults](#item-6) ⭐️ 8.0/10
7. [Microsoft to Enable Memory Integrity by Default on Windows 11 in October 2026](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI unveils GPT-6 Astra with near-perfect ARC-AGI-3 score](https://openai.com/index/gpt-6-astra/) ⭐️ 9.0/10

OpenAI has officially announced GPT-6 Astra, a new frontier model that reportedly scores 99.9% on the ARC-AGI-3 benchmark and makes major gains on the Artificial Analysis Coding Agent Index. The system card is publicly available at deploymentsafety.openai.com. GPT-6 Astra's near-perfect ARC-AGI-3 result is significant because that benchmark is designed to measure an agent's ability to learn novel skills interactively, a capability long associated with general intelligence. The release also raises the competitive bar for coding-agent performance and reignites the debate over whether such scores reflect real progress toward AGI or merely broader benchmark coverage. The ARC-AGI-3 result depends heavily on the harness used; with the responses API harness, GPT-5.6 Sol is estimated to score about 30%, while the leaderboard shows 7.8% under a different standard. GPT-6 Astra's 99.9% comes from a specific harness configuration, and the full system card is available at deploymentsafety.openai.com.

hackernews · kibae · Sep 3, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49554643)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark from ARC Prize that evaluates whether an AI agent can learn in novel environments through exploration, goal inference, and planning without explicit instructions; earlier frontier models often scored below 1% while humans solved it completely. GPT-6 Astra is OpenAI's successor to GPT-5 and arrives amid intense competition on coding-agent leaderboards such as the Artificial Analysis Coding Agent Index.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC Prize - Leaderboard ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3: The New Interactive Reasoning Benchmark GitHub - arcprize/arc-agi-3-benchmarking</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**Discussion**: Commenters raised concerns that the ARC-AGI-3 scorecard is misleading, noting that GPT-5.6 Sol would score roughly 30% if measured with the same responses API harness used for GPT-6 Astra. Others pointed out that despite the near-perfect ARC-AGI-3 score, improvements on other benchmarks look incremental, echoing François Chollet's critique that most frontier-model progress remains skill-acquisition and coverage-driven. Some also noticed an overrepresentation of autonomous shopping in the demos.

**Tags**: `#AI`, `#GPT-6`, `#OpenAI`, `#LLM`, `#AGI`

---

<a id="item-2"></a>
## [ICANN and Verisign Propose Terminating Third-Level .name Domains](https://neil.fraser.name/news/2026/09/03/) ⭐️ 8.0/10

ICANN and Verisign have proposed terminating all existing third-level .name domain registrations (e.g., user.surname.name) and releasing the underlying second-level domains for new registration. The proposal would invalidate long-held personal-name domains rather than simply closing them to new registrations. This policy shift undermines the stability and security of existing domain registrations, contradicting ICANN's mission to ensure the stable, secure operation of the Internet's unique identifier systems. Affected registrants risk losing their online identities, while released second-level domains could be scooped up by third parties, enabling impersonation and domain squatting. The proposal targets third-level .name registrations, where the registrant controls the leftmost label (e.g., 'neil' in neil.fraser.name), and the corresponding second-level domain (fraser.name) currently remains unavailable to others. Once the third-level domains are terminated, the now-vacant second-level domains are expected to become available, without a stated reservation period for existing holders.

hackernews · pavel_lishin · Sep 3, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49550772)

**Background**: .name is a top-level domain created for personal names, and it originally allowed registrations at the third level, such as john.smith.name, alongside second-level registrations like smith.name. In the DNS hierarchy, a second-level domain sits directly below a top-level domain, and a third-level domain is one level further down. ICANN coordinates the domain name system and contracts with registry operators like Verisign, which administers the .name TLD. The proposal reflects the registry's effort to phase out an older, less-used registration structure, but it raises concerns about contract stability and registrant protections.

<details><summary>References</summary>
<ul>
<li><a href="https://neil.fraser.name/news/2026/09/03/">Neil Fraser: News: . name Termination</a></li>
<li><a href="https://support.opensrs.com/support/solutions/articles/201000063568--name-domain-policies">A Domain Resellers Guide to . NAME Domain Policies : OpenSRS...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Second-level_domain">Second-level domain - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly critical, with one suggesting that new registrations should be stopped while existing third-level domains are honored. Another argued that the arbitrary termination contradicts ICANN's own mission of stability and security and would enable name hijacking. Some clarified that second-level domain owners like dvt.name are not affected, while others noted that leases can disappear, making reliance on such domains risky.

**Tags**: `#dns`, `#icann`, `#domain-policy`, `#web-infrastructure`, `#security`

---

<a id="item-3"></a>
## [1993 Amiga Assembly Game Ported to Godot With an LLM in One Evening](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

The developer ported his original 1993 Amiga game, written in MC68000 assembly and created in Baghdad, to the Godot engine using Claude Fable 5, an LLM that decoded the legacy assembly code. The initial working port was completed in a single evening, with a few more weekends spent fine-tuning and shipping the game. This demonstrates a practical use of LLMs to salvage and modernize decades-old hand-written assembly code, significantly lowering the barrier to retro game preservation and porting. It also showcases AI-assisted reverse engineering as a viable workflow for the retro-computing community. The LLM repeatedly assembled the code with vasm on the author's Mac until the resulting binary was byte-identical to the original shipped files. A residual 108-byte mismatch was explained by the original files being memory snapshots taken after the game had run inside AsmOne, not clean assembler output.

hackernews · rabahs · Sep 3, 14:28 · [Discussion](https://news.ycombinator.com/item?id=49550375)

**Background**: The Amiga was a line of home computers popular in the late 1980s and early 1990s, famed for custom graphics and sound hardware; many games were written in Motorola 68000 assembly to maximize performance. AsmOne was a popular Amiga development environment that assembled code in memory, so saved binaries could include runtime changes. vasm is a modern portable assembler that can rebuild 68000 code byte-for-byte. This context explains the 108-byte mismatch the LLM encountered: the original files were memory snapshots, not clean assembler output.

<details><summary>References</summary>
<ul>
<li><a href="http://sun.hasenbraten.de/vasm/">vasm portable and retargetable assembler</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_programming_languages">Amiga programming languages - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Motorola_68000">Motorola 68000 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic and nostalgic. One shared a similar successful experiment: asking Claude to build a Go version from a ZX81 memory dump. Others praised the original 1993 assembly achievement, wondered about debugging stories, commented on the game's resemblance to 'Gods: Into the Wonderful', and said they plan to apply the same approach to other forgotten games.

**Tags**: `#LLM`, `#Godot`, `#Amiga`, `#assembly`, `#retro-gaming`

---

<a id="item-4"></a>
## [Go Grandmaster Shin Jinseo Beats AI KataGo with Two-Stone Handicap](https://www.kedglobal.com/artificial-intelligence/newsView/ked202607210007) ⭐️ 8.0/10

Shin Jinseo, the world's top-ranked Go player, defeated the AI engine KataGo in a game in which he received a two-stone handicap. The result was reported by KED Global and drew attention as one of the few human wins against a top Go AI under handicap conditions. This matters because Shin is widely considered the strongest human Go player in history, yet even he needs a two-stone handicap to overcome leading AI engines. The game shows how AI has reshaped professional Go, while also demonstrating that human creativity in complex joseki can still create winning opportunities. The victory reportedly came from Shin playing out a complex variation of the 'flying knife' joseki, a long exchange that can run for over 50 moves, steering the game to a favorable position. A two-stone handicap means Shin was treated as the far weaker player, and community estimates agree that in an even game no human could currently beat KataGo.

hackernews · gmays · Sep 3, 01:11 · [Discussion](https://news.ycombinator.com/item?id=49544762)

**Background**: KataGo is a free, open-source computer Go program developed by David Wu and first released in February 2019; it is one of the strongest AI engines and is capable of beating top human players. In Go, a handicap is given by the stronger player placing extra stones before starting, in order to offset the difference in strength; for two stones, the stones are usually placed on corner points. Handicaps are commonly used in Go, and a player's rating or grade can be expressed directly in terms of stones of handicap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Handicapping_in_Go">Handicapping in Go - Wikipedia</a></li>
<li><a href="https://www.britgo.org/about/rating">Ratings, Grades and Handicaps | British Go Association</a></li>

</ul>
</details>

**Discussion**: Commenters emphasized that Shin is exceptional even among professionals, with an Elo-like rating around 3850, about 120 points ahead of the next-best player and far above Ke Jie's peak of 3755. Several clarified that the headline could mislead, because the handicap means Shin was considered the weaker player and no human could beat KataGo in an even game. Others praised Shin's decision to build the board according to his own style rather than imitating AI moves.

**Tags**: `#Artificial Intelligence`, `#Go`, `#KataGo`, `#Human-AI Competition`, `#Games`

---

<a id="item-5"></a>
## [Audacity 4.0 Launches With Qt6 UI, Drawing Praise and Criticism](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

Audacity 4.0, the latest major release of the open-source audio editor, has been published on GitHub with a redesigned Qt6-based user interface. The release is part of a modernisation effort led by Muse Group, which now oversees Audacity's development. This is a significant milestone for one of the most widely used open-source audio editors, and it shows that the project is still actively evolving after years of community debate over its direction. The update affects a huge user base, including musicians, podcasters, and hobbyist audio engineers, many of whom rely on Audacity for free multi-track editing. The new UI is built on Qt6 rather than the older wxWidgets toolkit, a major architectural shift that affects how the application looks and behaves across Windows, macOS, and Linux. Community members note that the changelog does not appear to address long-standing complaints about JACK/Pipewire integration, such as the lack of a persistent JACK client.

hackernews · ClydeN · Sep 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=49548395)

**Background**: Audacity is a free, open-source program for recording and editing audio, popular for tasks such as trimming podcasts, removing noise, and mixing tracks. In 2021, Audacity was acquired by Muse Group, and later releases introduced online services and telemetry, prompting controversy and leading some users to create forks such as Tenacity and Sneedacity. Qt is a cross-platform C++ framework used to build native graphical interfaces; Qt6 is the latest major generation of that framework.

<details><summary>References</summary>
<ul>
<li><a href="https://ru.wikipedia.org/wiki/Qt">Qt — Википедия</a></li>
<li><a href="https://www.pythonguis.com/pyqt6-tutorial/">PyQt6 Tutorial 2026, Create Python GUIs with Qt</a></li>

</ul>
</details>

**Discussion**: Comments show a split response: some users welcome the new momentum and recommend a presentation by Muse’s Head of Software, while others remain skeptical because their technical complaints, such as weak Pipewire/JACK support, appear unaddressed. There is also continued concern about telemetry and the push toward audio.com services, and one user asks what happened to post-telemetry forks like Tenacity and Sneedacity.

**Tags**: `#audacity`, `#audio-editing`, `#open-source`, `#release`, `#qt`

---

<a id="item-6"></a>
## [Polars 2.0 pre-release removes legacy constraints, changes defaults](https://pola.rs/posts/announcing-polars-2/) ⭐️ 8.0/10

The Polars team has announced the 2.0 pre-release, positioning it as a deliberately 'boring' major version rather than a feature release. The release focuses on removing legacy design constraints and flipping defaults such as maintain_order=False. As one of the fastest-growing DataFrame libraries, Polars' major-version philosophy sets an example for semantic versioning in open-source data tools. The default changes could require pipeline updates in production and scientific computing environments that previously relied on implicit row-order preservation. In Polars 2.0, operations such as sort, join, and unique gain or keep a maintain_order parameter, with the default False because order preservation is more expensive and can block the streaming engine. The upgrade guide also notes that before 2.0, some checks were performed by lossily coercing operands to Float64, which the new release removes.

hackernews · komape · Sep 3, 06:59 · [Discussion](https://news.ycombinator.com/item?id=49546753)

**Background**: Polars is an analytical query engine for DataFrames written in Rust, designed for multi-threaded, vectorized execution and very high performance. Many users compare it with pandas, which is more notebook-oriented but pushes edge cases to runtime. Earlier Polars engines often preserved row order by default as a natural side effect, but the new streaming engine makes guaranteed ordering expensive. A maintain_order parameter lets users choose order-preserving semantics explicitly when needed.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/75748777/does-polars-preserve-row-order-in-a-left-join">python - Does polars preserve row order in a left join ...</a></li>
<li><a href="https://docs.pola.rs/releases/upgrade/2/">Version 2 . 0 -rc - Polars user guide</a></li>
<li><a href="https://github.com/pola-rs/polars">GitHub - pola - rs / polars : Extremely fast Query Engine for DataFrames...</a></li>

</ul>
</details>

**Discussion**: Commenters generally welcomed the team's serious approach to semantic versioning, with one describing the deliberate 'boring' major release as exactly how version bumps should be done. Others praised Polars for production stability, while a scientist questioned whether changing maintain_order to False by default could introduce non-deterministic behavior into scientific pipelines. Another developer highlighted streaming and out-of-core progress, reporting strong results when using Polars as a backend for graph queries.

**Tags**: `#polars`, `#dataframe`, `#data-engineering`, `#software-release`, `#rust`

---

<a id="item-7"></a>
## [Microsoft to Enable Memory Integrity by Default on Windows 11 in October 2026](https://techcommunity.microsoft.com/blog/windows-itpro-blog/expanding-memory-integrity-protection-across-windows-devices/4551984) ⭐️ 8.0/10

Microsoft announced it will automatically enable Memory Integrity (HVCI) on eligible Windows 11 devices starting October 13, 2026. The change will use hardware virtualization to allow only trusted kernel-mode drivers and code to run. This security default change significantly reduces the driver-based attack surface across a large number of Windows 11 devices. It may also affect system performance and driver compatibility, making it important for consumers and enterprise administrators. Eligible devices must support hardware virtualization, UEFI, and Secure Boot. The rollout starts with the October 13 Patch Tuesday update, and incompatible or older drivers may prevent enablement, with rare cases causing blue screens.

telegram · zaihuapd · Sep 3, 06:09

**Background**: Memory Integrity, also called Hypervisor-protected Code Integrity (HVCI), is a Windows security feature built on Virtualization-Based Security (VBS). It uses hardware virtualization to create an isolated environment that verifies kernel-mode code and drivers before they run. This helps prevent malicious software from exploiting low-level drivers to take over the system. Microsoft previously enabled VBS by default on Windows 11, and now it is expanding default Memory Integrity coverage to eligible devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/997/293.htm">微软称符合条件 Win11 设备 10 月默认启用内存完整性保护，拦截恶意驱...</a></li>
<li><a href="https://www.cnblogs.com/suv789/p/18819875">启用 内核完整性保护（HVCI） 和 受控文件夹访问（CFA） 是 Windows ...</a></li>
<li><a href="https://www.gamersky.com/news/202609/2202013.shtml">Win 11 ...</a></li>

</ul>
</details>

**Tags**: `#Windows 11`, `#Security`, `#HVCI`, `#Memory Integrity`, `#Microsoft`

---