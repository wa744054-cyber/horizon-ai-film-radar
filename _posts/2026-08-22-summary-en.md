---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 29 items, 6 important content pieces were selected

---

1. [Open-Source Roguelike DelveRL Built for Training Game Agents](#item-1) ⭐️ 8.0/10
2. [Evaluation Resolution Alters Which Learning Rule Looks Most Brain-Like at V1](#item-2) ⭐️ 8.0/10
3. [Nintendo Wipes Out 400+ Switch Emulator Repos in Single-Day GitHub Sweep](#item-3) ⭐️ 8.0/10
4. [Tesla Announces Supervised Full Self-Driving Now Available in China](#item-4) ⭐️ 8.0/10
5. [SemiAnalysis: Open Models Catch Up Twice as Fast Each Generation](#item-5) ⭐️ 8.0/10
6. [Amazon Accused of Buying, Scanning, Destroying Books for AI Training](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Open-Source Roguelike DelveRL Built for Training Game Agents](https://www.reddit.com/r/MachineLearning/comments/1vvii1j/i_built_an_opensource_roguelike_specifically_for/) ⭐️ 8.0/10

The developer released DelveRL, a purpose-built open-source turn-based roguelike environment for reinforcement learning, with deterministic simulation, procedural levels, partial observability, and batched renderer-free environments. It includes a recurrent PPO baseline that reaches a median floor of 18 and extended runs to floor 33. DelveRL addresses a real gap in RL research by providing a human-playable game with a structured API that is easy to integrate with agent harnesses, unlike many existing games. This could make roguelike environments more accessible for testing agent exploration, risk management, and long-horizon planning. The environment is fully local, features deterministic simulation for reproducibility, and offers procedural levels, partial observability, and strategic depth. The project includes game code, training code, a checkpoint, bridge documentation, and raw benchmarks, all open source.

reddit · r/MachineLearning · /u/SnyderConsulting · Aug 22, 17:32

**Background**: Reinforcement learning (RL) involves an agent learning to make decisions by interacting with an environment and receiving rewards. Games like roguelikes offer rich, partially observable, procedurally generated scenarios useful for testing RL algorithms, but many existing games are difficult to integrate with agent harnesses. Recurrent PPO is an extension of the Proximal Policy Optimization algorithm that uses LSTM networks to handle partial observability and memory.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/SnyderConsulting/DelveRL/tree/main/docs">DelveRL/docs at main · SnyderConsulting/DelveRL · GitHub</a></li>
<li><a href="https://sb3-contrib.readthedocs.io/en/master/modules/ppo_recurrent.html">Recurrent PPO — Stable Baselines3 - Contrib 2.9.0 documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning">Reinforcement learning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#RL environment`, `#roguelike`, `#open-source`, `#game agents`

---

<a id="item-2"></a>
## [Evaluation Resolution Alters Which Learning Rule Looks Most Brain-Like at V1](https://www.reddit.com/r/MachineLearning/comments/1vvdxwt/the_evaluation_resolution_has_been_shown_to_have/) ⭐️ 8.0/10

This study shows that the resolution at which CNN representations are evaluated strongly affects which learning rule appears most brain-like at V1. The common finding that untrained CNNs match trained ones vanishes at higher resolutions, where trained models clearly outperform untrained ones. This finding is important because model-brain comparisons using RSA are widely used in computational neuroscience, and evaluation resolution has been largely ignored as a confound. It challenges past claims that untrained CNNs are as brain-like as trained ones, which could reshape how researchers interpret such comparisons. The study used a small CNN trained on a CIFAR-10 subset at 32 px and evaluated it on THINGS-fMRI stimuli across six resolutions (32 to 224 px) while keeping weights and normalization fixed. Five learning rules were compared, and the authors ruled out several confounds, including batch-norm miscalibration and low-level pixel structure; a backprop advantage at lateral occipital complex (LOC) persisted at all resolutions.

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · Aug 22, 14:30

**Background**: Representational Similarity Analysis (RSA) is a technique that compares how a model and a brain represent stimuli by correlating their pairwise similarity matrices. V1 is the first cortical region for visual processing, and CNNs are often used as models of biological vision. Learning rules such as backpropagation, feedback alignment, and spike-timing-dependent plasticity (STDP) define how networks update their weights during training. Previous work suggested that random untrained CNNs can match trained CNNs in V1, but this study indicates that this conclusion depends on the evaluation resolution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/systems-neuroscience/articles/10.3389/neuro.06.004.2008/full">Frontiers | Representational similarity analysis - connecting the...</a></li>
<li><a href="https://towardsdatascience.com/feedback-alignment-methods-7e6c41446e36/">Feedback Alignment Methods | Towards Data Science</a></li>
<li><a href="https://homo-deus.com/lab/neuromorphic-computing/stdp-learning/">STDP Simulator: Spike - Timing - Dependent Plasticity Learning Rule</a></li>

</ul>
</details>

**Tags**: `#computational neuroscience`, `#CNN`, `#learning rules`, `#model-brain comparison`, `#evaluation resolution`

---

<a id="item-3"></a>
## [Nintendo Wipes Out 400+ Switch Emulator Repos in Single-Day GitHub Sweep](https://torrentfreak.com/nintendo-wipes-out-400-switch-emulator-repos-in-single-day-github-sweep/) ⭐️ 8.0/10

Nintendo filed seven DMCA anti-circumvention notices with GitHub in a single day, resulting in the takedown of over 400 Switch emulator repositories, including 311 suyu forks and 29 Skyline repositories. The notices allege the emulators use unauthorized keys to decrypt games. This is one of the largest coordinated DMCA enforcement actions against open-source emulator projects, affecting hundreds of repositories and potentially chilling future Switch emulation development. It also highlights the ongoing legal tension between emulation, anti-circumvention law, and open-source software distribution. The DMCA notices are anti-circumvention claims under Section 1201, targeting the use of decryption keys rather than direct copyright infringement. Both the Yuzu and Suyu cases were resolved by settlement without a final court ruling, so the legal precedent remains unsettled.

telegram · zaihuapd · Aug 22, 00:28

**Background**: Switch emulators such as Yuzu, Suyu, and Skyline let users play Nintendo Switch games on PCs or Android devices by mimicking console hardware and using decryption keys obtained from real consoles. In March 2024, Yuzu settled with Nintendo for $2.4 million and shut down; Suyu is a community fork of Yuzu, while Skyline was an Android-focused emulator that stopped development in 2023. DMCA Section 1201 prohibits the circumvention of technological protection measures, which is the legal basis for Nintendo's takedown requests.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yuzu_(emulator)">Yuzu (emulator) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Skyline_(emulator)">Skyline (emulator)</a></li>

</ul>
</details>

**Tags**: `#Nintendo`, `#DMCA`, `#Emulation`, `#GitHub`, `#Legal`

---

<a id="item-4"></a>
## [Tesla Announces Supervised Full Self-Driving Now Available in China](https://t.me/zaihuapd/43321) ⭐️ 8.0/10

Tesla announced on X that its supervised Full Self-Driving (FSD) feature is now available in China, marking the latest expansion of its advanced driver-assistance system. The announcement did not provide an exact launch date or detailed rollout plans. This is a significant regulatory and market milestone because China is one of the world's largest auto markets and a highly competitive arena for autonomous driving. It could pressure domestic rivals like BYD, Huawei-backed brands, and Xpeng to accelerate their own assisted-driving offerings. Tesla's FSD (Supervised) remains a Level 2 driver-assistance system that still requires an attentive driver behind the wheel, and Tesla notes it does not make the vehicle autonomous. The company claims FSD (Supervised) results in 7x fewer major and minor collisions and 5x fewer off-highway collisions, although these figures require active driver supervision.

telegram · zaihuapd · Aug 22, 01:56

**Background**: Full Self-Driving (Supervised) is Tesla's optional Level 2 advanced driver-assistance system, as defined by SAE International, available on vehicles produced since April 2019. It provides automatic steering, traffic-aware cruise control, and road navigation, but unlike fully autonomous driving, it requires active driver supervision. The expansion into China is a notable development for the autonomous-driving industry in the country.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot">Tesla Autopilot - Wikipedia</a></li>
<li><a href="https://www.tesla.com/support/fsd">Full Self-Driving (Supervised) | Tesla Support</a></li>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving (Supervised) | Tesla</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#FSD`, `#Autonomous Driving`, `#China`, `#AI`

---

<a id="item-5"></a>
## [SemiAnalysis: Open Models Catch Up Twice as Fast Each Generation](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis's latest analysis finds that open-source models are closing the capability gap with closed-source frontier models faster with each generation. In the agent era, Kimi K2.6 surpassed Opus 4.5 in 4.8 months, and GLM-5.2 overtook GPT-5.2 in 6 months. This raises concerns about model-layer commoditization, as open-source models like GLM 5.3 and Kimi K3 can now handle many coding and agent tasks that helped Anthropic reach over $65 billion in annualized revenue. It suggests that pure model capability may become less of a differentiator, pushing value to productization and distribution. The analysis divides AI model history into three eras—early scaling, reasoning, and agent—and finds catch-up times halve each generation. However, it cautions that benchmarks are not everything and that Anthropic's productization strengths remain a key advantage.

telegram · zaihuapd · Aug 22, 08:26

**Background**: SemiAnalysis is an independent research firm specializing in semiconductors and artificial intelligence, known for institutional-grade industry analysis. The AI industry is increasingly debating whether open-source models will commoditize the model layer, as seen in discussions about generative AI commoditization and the shift toward agent-based workflows. The 'agent era' refers to the current phase where AI assistants move from chatting to executing tasks, which is exactly where open-source models are converging quickly.

<details><summary>References</summary>
<ul>
<li><a href="https://startedbywomen.com/companies/semianalysis">SemiAnalysis | Started by Women</a></li>
<li><a href="https://baike.baidu.com/item/智能体时代/68091644">智能体时代（人工智能代理时代）_百度百科</a></li>
<li><a href="https://www.jxxy.net/ai/articles/aiwhisperx-coding-agent-24b-arr/">写在Coding Agent 240亿时刻：大模型进入挤兑阶段｜觉醒AI</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#AI models`, `#industry analysis`, `#SemiAnalysis`, `#agent era`

---

<a id="item-6"></a>
## [Amazon Accused of Buying, Scanning, Destroying Books for AI Training](https://t.me/zaihuapd/43331) ⭐️ 8.0/10

404 Media's investigation reveals Amazon has been buying physical books, scanning them to train AI models, and then destroying the original copies. The researchers traced a rare book to an Amazon warehouse in Las Vegas, where employees said they cut off bindings to speed up scanning and then discarded the pages. This practice raises serious ethical and legal concerns about copyright infringement and the destruction of cultural artifacts. It highlights an emerging industry trend where tech companies harvest printed works for AI training, which could affect authors, publishers, and the preservation of rare or out-of-print books. The investigation placed tracking devices inside a rare book and followed it to an Amazon facility in Las Vegas, Nevada. According to warehouse staff, large volumes of printed books are received, their bindings are cut off to accelerate scanning, and the pages are then destroyed.

telegram · zaihuapd · Aug 22, 15:40

**Background**: AI companies need massive amounts of text data to train large language models, and books are considered valuable high-quality sources. Similar practices were previously reported with Anthropic. Authors and publishers have increasingly raised copyright objections to such unlicensed use of their works, and the additional destruction of physical books amplifies concerns about loss of irreplaceable printed materials.

**Tags**: `#AI training`, `#Amazon`, `#copyright`, `#data ethics`, `#investigative report`

---