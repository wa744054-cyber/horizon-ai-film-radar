---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 43 items, 14 important content pieces were selected

---

1. [MIRA: 5B Parameter World Model for Rocket League Released](#item-1) ⭐️ 9.0/10
2. [Januscape KVM Escape: 16-Year-Old Flaw Affects Intel and AMD](#item-2) ⭐️ 9.0/10
3. [DeepSeek developing own AI inference chips to reduce reliance on NVIDIA and Huawei](#item-3) ⭐️ 9.0/10
4. [Tenda Firmware Hidden Backdoor Grants Admin Access](#item-4) ⭐️ 8.0/10
5. [EU Chat Control Proposals Threaten End-to-End Encryption](#item-5) ⭐️ 8.0/10
6. [EU Mandates Driver Monitoring Cameras in All New Cars](#item-6) ⭐️ 8.0/10
7. [sqlite-utils 4.0 Released with Schema Migrations](#item-7) ⭐️ 8.0/10
8. [Differentiable Ray Tracing for Radio Propagation Thesis](#item-8) ⭐️ 8.0/10
9. [Trusted LoRA adapter subspace blocks malicious fine-tuning updates](#item-9) ⭐️ 8.0/10
10. [US Makes NVIDIA Blackwell Wafers, But Taiwan Still Packages Them](#item-10) ⭐️ 8.0/10
11. [China Weighs Export Controls on Top AI Models](#item-11) ⭐️ 8.0/10
12. [China's humanoid robot output to exceed 100k units by 2026](#item-12) ⭐️ 8.0/10
13. [Claude Cowork Launches: AI Autonomously Completes Complex Tasks](#item-13) ⭐️ 8.0/10
14. [Alibaba Orders Employees to Uninstall Claude by July 10](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MIRA: 5B Parameter World Model for Rocket League Released](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 9.0/10

MIRA is a 5-billion-parameter interactive world model trained on 10,000 hours of synthetic Rocket League data, capable of running 4-player simulations at 20 fps on a single NVIDIA B200 GPU. The developers released a playable online demo, a technical report, and a 1,000-hour 4-player gameplay dataset. This marks a significant milestone in multi-agent world modeling, demonstrating that large-scale interactive simulations can be trained and run efficiently on current hardware. It opens up new possibilities for AI research in multi-agent planning, simulation, and game AI, and the open-source release enables broader community exploration. The model has 5 billion parameters and runs 4-player simulations at 20 fps on a single B200 GPU using the Blackwell architecture. The dataset consists of 1,000 hours of 4-player Rocket League gameplay, and the technical report provides in-depth methodology details.

reddit · r/MachineLearning · /u/MasterScrat · Jul 7, 07:59

**Background**: A world model is an AI system that learns an internal representation of an environment and predicts how it evolves in response to actions. World models are used for planning, simulation, and reinforcement learning, enabling agents to reason about future outcomes without constant interaction with the real environment. This work applies world models to a complex multiplayer video game, showcasing their potential for multi-agent scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/dgx-b200/">DGX B200: The Foundation for Your AI Factory | NVIDIA</a></li>

</ul>
</details>

**Tags**: `#world models`, `#deep learning`, `#reinforcement learning`, `#video game AI`, `#multi-agent`

---

<a id="item-2"></a>
## [Januscape KVM Escape: 16-Year-Old Flaw Affects Intel and AMD](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

Security researchers disclosed Januscape (CVE-2026-53359), the first cross-platform KVM/x86 virtual machine escape vulnerability affecting both Intel and AMD platforms, with a published proof-of-concept exploit. This vulnerability breaks the isolation boundary between guest VMs and the host kernel, posing a severe threat to multi-tenant cloud environments and any KVM-based virtualization deployments. The flaw is a use-after-free bug in the shadow MMU emulation, allowing a guest to corrupt the host kernel's shadow page tables through internal operations, causing a host kernel panic.

telegram · zaihuapd · Jul 7, 10:14

**Background**: KVM (Kernel-based Virtual Machine) is a Linux kernel module that allows the host to run multiple virtual machines. The shadow MMU is a component used for managing memory virtualization when hardware support is unavailable or insufficient. This vulnerability has been present in the Linux kernel from 2010 to June 2026, spanning 16 years.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://docs.kernel.org/virt/kvm/x86/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://security.googleblog.com/2024/06/virtual-escape-real-reward-introducing.html">Virtual Escape; Real Reward: Introducing Google’s kvmCTF</a></li>

</ul>
</details>

**Tags**: `#security`, `#virtualization`, `#KVM`, `#vulnerability`, `#Linux kernel`

---

<a id="item-3"></a>
## [DeepSeek developing own AI inference chips to reduce reliance on NVIDIA and Huawei](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 9.0/10

DeepSeek has been developing its own AI inference chips for about a year, aiming to reduce dependency on NVIDIA and Huawei chips amid US export controls. The chip focuses on inference, not training, and the company has begun hiring chip designers and contacting foundries. This move signals a strategic shift in the AI hardware supply chain, as a major Chinese AI company seeks independence from Western and sanctioned chip suppliers. If successful, it could reduce the impact of US export controls on China's AI industry. The chip is in early stages, designed specifically for inference workloads. DeepSeek previously relied on NVIDIA H800 and Huawei Ascend chips, and founder Liang Wenfeng acknowledged chip restrictions as a challenge in a rare 2024 interview.

telegram · zaihuapd · Jul 7, 11:08

**Background**: DeepSeek is a Chinese AI company known for large language models. US export controls restrict the sale of advanced AI chips like NVIDIA's H100 to China, pushing companies to develop alternatives. Huawei also produces Ascend AI chips, but they are less powerful than top NVIDIA offerings. Recent Huawei roadmap reveals Ascend 950PR, an inference chip with 1.56 PFLOPs, challenging NVIDIA's H20.

<details><summary>References</summary>
<ul>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>
<li><a href="https://www.huaweicentral.com/huawei-reveals-3-year-ascend-ai-chip-roadmap-950-coming-in-2026/">Huawei reveals 3-year Ascend AI chip roadmap, 950 coming in 2026</a></li>
<li><a href="https://laweconcenter.org/resources/us-export-controls-on-ai-and-semiconductors/">US Export Controls on AI and Semiconductors - International ...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#DeepSeek`, `#chip design`, `#export controls`

---

<a id="item-4"></a>
## [Tenda Firmware Hidden Backdoor Grants Admin Access](https://kb.cert.org/vuls/id/213560) ⭐️ 8.0/10

Multiple versions of Tenda firmware contain an undocumented authentication backdoor (CVE-2026-11405) using a hardcoded password 'rzadmin', allowing an attacker to gain full administrative access to the device's web management panel. This vulnerability affects a wide range of Tenda network devices, including routers and switches, potentially compromising home and business networks. It highlights ongoing security risks in IoT devices with hardcoded credentials. The backdoor is found in the /bin/httpd web server binary within the login() function. Five specific firmware builds are confirmed vulnerable, including versions for AC10, AC15, and BE12Pro models.

hackernews · miniBill · Jul 8, 00:08 · [Discussion](https://news.ycombinator.com/item?id=48825749)

**Background**: A hardcoded password is a plain-text password embedded in source code, bypassing normal authentication. In IoT devices, such backdoors can be exploited remotely without user interaction. This vulnerability was first detailed in a 2022 write-up and has now been assigned CVE-2026-11405.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hidden-backdoor-in-tenda-router-firmware-grants-admin-access/">Hidden backdoor in Tenda router firmware grants admin access</a></li>
<li><a href="https://thehackernews.com/2026/07/certcc-warns-of-hidden-admin-backdoor.html">CERT/CC Warns of Hidden Admin Backdoor in Tenda Router Firmware</a></li>
<li><a href="https://kb.cert.org/vuls/id/213560">VU#213560 - Tenda firmware (multiple versions) contains ...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the hardcoded password 'rzadmin' was disclosed in a 2022 blog post, and recent firmware is encrypted, complicating analysis. Some attribute the issue to incompetence rather than malice, but advise avoiding Tenda products.

**Tags**: `#security`, `#backdoor`, `#Tenda`, `#IoT`, `#hardcoded credentials`

---

<a id="item-5"></a>
## [EU Chat Control Proposals Threaten End-to-End Encryption](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

The European Union has proposed 'Chat Control' regulations (version 1.0 and 2.0) that would require platforms to scan all private messages, including end-to-end encrypted ones, for child sexual abuse material. Critics argue this effectively breaks encryption and creates mass surveillance infrastructure. If enacted, Chat Control would fundamentally undermine end-to-end encryption, impacting the privacy and security of hundreds of millions of EU citizens. It sets a dangerous global precedent for government-mandated surveillance of private communications. Chat Control 1.0 expired in April 2026, but negotiations for Chat Control 2.0 continue with trilogues scheduled. The proposal relies on client-side scanning, which analyzes content on the user's device before encryption, raising technical and legal concerns about backdoors and reduced security.

hackernews · gasull · Jul 7, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48818311)

**Background**: Chat Control refers to a set of EU regulations aimed at combating child sexual abuse material (CSAM) online. The proposals require digital platforms to detect and report CSAM, potentially by scanning all messages. Client-side scanning is a controversial method that inspects data on the device before it is encrypted and sent, which could be exploited for broader surveillance and weaken trust in encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://fightchatcontrol.eu/chat-control-overview">Chat Control 1.0 vs 2.0 - Fight Chat Control</a></li>
<li><a href="https://www.internetsociety.org/resources/doc/2020/fact-sheet-client-side-scanning/">Fact Sheet: Client-Side Scanning - Internet Society</a></li>

</ul>
</details>

**Discussion**: The community comments express strong opposition to the proposals, with users calling it a 'dictatorial power' grab and a 'creepy surveillance state.' Technical questions are raised about how scanning encrypted messages would work, referencing either government backdoors or on-device scanning like Apple's CSAM scanner, and concerns about false positives affecting innocent users.

**Tags**: `#privacy`, `#encryption`, `#EU legislation`, `#surveillance`, `#technology policy`

---

<a id="item-6"></a>
## [EU Mandates Driver Monitoring Cameras in All New Cars](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

Starting from a recent EU regulation, all new cars sold in the European Union must include a driver monitoring camera system to detect drowsiness and distraction. This mandate significantly impacts automotive safety and privacy norms across Europe, affecting millions of drivers and manufacturers, and sparks debate on the balance between safety technology and personal privacy. The regulation specifically requires Driver Drowsiness and Attention Warning (DDAW) systems, which use infrared cameras and AI to monitor eye movement, head position, and other cues, as part of the EU General Safety Regulation (EU) 2019/2144.

hackernews · nickslaughter02 · Jul 7, 20:50 · [Discussion](https://news.ycombinator.com/item?id=48823557)

**Background**: Driver monitoring systems (DMS) use in-cabin cameras and sensors to track driver behavior, such as eye gaze and head pose, to detect distraction or drowsiness. They are already used in some luxury vehicles and are now being mandated by regulators in the EU and US to improve road safety.

<details><summary>References</summary>
<ul>
<li><a href="https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=PI_COM:C(2023)4523">Advanced Drivers Distraction Warning (ADDW) - EUR-Lex</a></li>
<li><a href="https://spyro-soft.com/blog/automotive/driver-monitoring-systems-to-become-mandatory-under-new-eu-and-us-road-safety-regulations">Driver Monitoring Systems to become mandatory under new EU and US road safety regulations</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed sentiments: many users report frustration with false positives, such as unwanted brake applications or beeping, while others acknowledge the systems can be accurate and potentially life-saving, with comparisons to airplane alarm overload highlighting concerns about design and user experience.

**Tags**: `#regulation`, `#privacy`, `#automotive`, `#driver monitoring`, `#EU`

---

<a id="item-7"></a>
## [sqlite-utils 4.0 Released with Schema Migrations](https://simonwillison.net/2026/Jul/7/sqlite-utils/#atom-everything) ⭐️ 8.0/10

Simon Willison released sqlite-utils 4.0, a major version that adds built-in support for database schema migrations, allowing developers to version-control and apply incremental changes to SQLite database schemas. Schema migrations are a critical feature for managing evolving databases in production; this release makes sqlite-utils a more complete tool for SQLite-based projects, particularly for developers who rely on Python and CLI workflows. The release includes support for both applying and rolling back migrations, and is available as both a Python library and a command-line tool. Two weeks prior, a release candidate (4.0rc1) was published that introduced migrations and nested transactions.

rss · Simon Willison · Jul 7, 15:42

**Background**: sqlite-utils is a Python library and CLI utility created by Simon Willison for manipulating SQLite databases. It provides higher-level operations on top of Python's sqlite3 module. Database schema migrations are a way to manage version-controlled, incremental changes to database schemas, commonly used in DevOps and software development.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>

</ul>
</details>

**Tags**: `#sqlite-utils`, `#SQLite`, `#Python`, `#database`, `#migrations`

---

<a id="item-8"></a>
## [Differentiable Ray Tracing for Radio Propagation Thesis](https://www.reddit.com/r/MachineLearning/comments/1upvkp5/phd_thesis_on_differentiable_ray_tracing_for/) ⭐️ 8.0/10

A Ph.D. thesis introduces a differentiable ray tracing framework for radio propagation modeling, using JAX for automatic differentiation to compute exact gradients through physical environments for inverse problems and ML training. This work bridges wireless communications and differentiable simulation, enabling gradient-based optimization for channel modeling, localization, and material calibration. Its open-source release (DiffeRT) makes these techniques accessible for next-generation wireless design. The thesis is split into three parts covering physics fundamentals, GPU-accelerated path tracing with discontinuity smoothing, and practical applications. It also open-sources DiffeRT2d, a 2D differentiable ray tracing toolbox built on JAX.

reddit · r/MachineLearning · /u/jeertmans · Jul 7, 13:45

**Background**: Ray tracing simulates the path of rays through an environment to model wave propagation. Differentiable ray tracing extends this by allowing gradients to be computed with respect to scene parameters, enabling optimization. Radio propagation models predict how radio waves travel, crucial for wireless network planning. This thesis merges these fields.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Radio_propagation">Radio propagation - Wikipedia</a></li>
<li><a href="https://github.com/jeertmans/DiffeRT2d">GitHub - jeertmans/DiffeRT2d: 2D Toolbox for Differentiable ...</a></li>
<li><a href="https://people.csail.mit.edu/tzumao/diffrt/">Differentiable Monte Carlo Ray Tracing through Edge Sampling</a></li>

</ul>
</details>

**Discussion**: Commenters praised the thesis for its accessibility and open-source code, noting its potential impact on wireless communications and differentiable programming.

**Tags**: `#differentiable ray tracing`, `#radio propagation`, `#automatic differentiation`, `#machine learning`, `#wireless communications`

---

<a id="item-9"></a>
## [Trusted LoRA adapter subspace blocks malicious fine-tuning updates](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

A new paper proposes constraining fine-tuning to a subspace learned from trusted LoRA adapters, preventing models from learning malicious updates. The approach was tested on 196 public LoRA adapters and against adaptive attacks, showing attack success drops sharply while useful adaptation is largely preserved. This offers a novel defense against fine-tuning poisoning that does not require detecting poisoned data, potentially improving AI safety in scenarios like on-device adaptation or user-generated data fine-tuning. It could shift the focus from detection to prevention by restricting the space of learnable behaviors. The method relies on a trusted pool of LoRA adapters to define a subspace that preserves useful adaptations while making malicious directions geometrically unreachable. The evaluation included adaptive attacks specifically designed to bypass the defense, and the paper provides public code and experiments for reproducibility.

reddit · r/MachineLearning · /u/Bright_Warning_8406 · Jul 7, 20:00

**Background**: LoRA (Low-Rank Adaptation) is a technique for efficiently fine-tuning large models by adding small, trainable adapter modules while keeping the base model frozen. Fine-tuning poisoning involves injecting malicious data into the training set to induce hidden behaviors like backdoors. Traditional defenses focus on detecting or filtering poisoned data, but this work takes a different approach by restricting the model's learning capacity to a subspace of trusted behaviors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://www.paloaltonetworks.com/cyberpedia/what-is-data-poisoning">What Is Data Poisoning? [Examples & Prevention] - Palo Alto Networks</a></li>
<li><a href="https://www.ibm.com/think/topics/lora">What is LoRA (Low-Rank Adaption)? | IBM</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#AI safety`, `#fine-tuning`, `#LoRA`, `#adversarial robustness`

---

<a id="item-10"></a>
## [US Makes NVIDIA Blackwell Wafers, But Taiwan Still Packages Them](https://www.tomshardware.com/tech-industry/nvidia-and-intel-tout-chips-built-in-america-but-every-arizona-made-blackwell-die-is-still-packaged-in-taiwan) ⭐️ 8.0/10

NVIDIA's Blackwell wafers are now mass-produced at TSMC's Arizona Fab 21 using the custom 4NP process, but the dies must be shipped to Taiwan for CoWoS-L advanced packaging and HBM integration. This highlights that the US can now produce leading-edge logic chips but remains dependent on Taiwan for advanced packaging, a critical bottleneck in AI chip supply chains with geopolitical implications. Advanced packaging requires CoWoS-L technology and HBM memory stacking, neither of which has mass production facilities in the US yet; facilities from Amkor, TSMC, and SK Hynix are under construction and expected to be ready by 2028-2029.

telegram · zaihuapd · Jul 7, 09:47

**Background**: NVIDIA's Blackwell architecture uses 208 billion transistors on TSMC's custom 4NP process. CoWoS-L (Chip-on-Wafer-on-Substrate with interposer) is a TSMC advanced packaging technology that integrates logic dies and HBM stacks side by side. Intel's 18A process is also mentioned as another advanced node in Arizona.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm">CoWoS® - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.intel.com/content/www/us/en/foundry/process/18a.html">Intel 18A | See Our Biggest Process Innovation</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#NVIDIA`, `#supply chain`, `#manufacturing`, `#Blackwell`

---

<a id="item-11"></a>
## [China Weighs Export Controls on Top AI Models](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 8.0/10

China's Ministry of Commerce has held meetings with Alibaba, ByteDance, and Zhipu AI to discuss restricting overseas access to the country's most advanced artificial intelligence models, including unreleased ones. This policy could reshape the global AI landscape by limiting the availability of leading Chinese models, potentially affecting open-source distribution and intensifying tech decoupling between the US and China. The restrictions may apply only to future models, and the final scope is still under discussion. Officials have also considered categorizing AI core technology leakage as a national security crime and limiting foreign investment in Chinese AI startups.

telegram · zaihuapd · Jul 7, 11:42

**Background**: China has developed a strong domestic AI ecosystem, with companies like Zhipu AI (rebranded internationally as Z.ai) producing open-weight models such as the GLM series. Zhipu AI was placed on the US Entity List in January 2025. The proposed export controls would affect both closed-weight and open-weight models, potentially impacting developers worldwide who rely on these models.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/beijing-china-ai-model-export-restrictions-070726">China weighs restrictions on overseas access to its most ...</a></li>
<li><a href="https://worldview.ranenetwork.com/content/situational-report/2026-07-07/china-beijing-explores-potential-export-restrictions-on-advanced-ai-models">China: Beijing Explores Potential Export Restrictions on ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zhipu_AI">Zhipu AI</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#China`, `#technology policy`, `#export controls`, `#national security`

---

<a id="item-12"></a>
## [China's humanoid robot output to exceed 100k units by 2026](https://www.news.cn/tech/20260707/1e0c79e82bb94a97a1488ebe3984834d/c.html) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology announced that the country's humanoid robot production is expected to surpass 100,000 units in 2026, and the AI application adoption rate among industrial enterprises above a designated size has exceeded 30%. This milestone reflects China's rapid progress in integrating AI and robotics into manufacturing, potentially strengthening its global leadership in industrial automation and accelerating economic transformation. Nearly 200 AI-related key standards have been developed domestically, and the AtomGit open-source community has registered over 11 million users. The 2026 World AI Conference in Shanghai will feature 1,100+ enterprises and 3,000+ exhibits, with over 300 products making global debuts.

telegram · zaihuapd · Jul 8, 02:25

**Background**: Humanoid robots are designed to mimic human form and movement, often powered by large AI models and intelligent agents. The 'above designated size' refers to enterprises with annual revenue above a certain threshold. AtomGit is a Chinese open-source platform that supports code hosting and community collaboration, akin to GitHub.

<details><summary>References</summary>
<ul>
<li><a href="https://gitcode.com/">AtomGit - 全球开发者的开源社区,开源代码托管平台</a></li>
<li><a href="https://github.com/atomgit-atomcode/atomcode">GitHub - atomgit-atomcode/atomcode: An open-source ...</a></li>

</ul>
</details>

**Tags**: `#humanoid robots`, `#AI adoption`, `#industrial AI`, `#China`, `#robotics`

---

<a id="item-13"></a>
## [Claude Cowork Launches: AI Autonomously Completes Complex Tasks](https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork) ⭐️ 8.0/10

Anthropic has launched Claude Cowork for paid users (Pro, Max, Team, Enterprise), enabling the AI to autonomously execute multi-step complex tasks in the background across desktop, web, and mobile platforms. This marks a significant advancement in AI assistant capabilities, as tasks like file organization, spreadsheet creation, and report generation can now run independently without constant user attention, greatly enhancing productivity across platforms. Tasks run remotely on Anthropic servers and continue even when the user's computer is turned off; desktop support includes direct local file read/write and browser operations, with scheduled automation and project-based task grouping.

telegram · zaihuapd · Jul 8, 03:50

**Background**: Claude is a family of large language models developed by Anthropic, first released in March 2023 and trained using constitutional AI for safety. Claude Cowork is an AI agent designed for non-technical office tasks, capable of accessing user folders on macOS to read, edit, create files, and perform asynchronous work.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://grokipedia.com/page/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#automation`, `#productivity`, `#Claude`

---

<a id="item-14"></a>
## [Alibaba Orders Employees to Uninstall Claude by July 10](https://t.me/zaihuapd/42424) ⭐️ 8.0/10

Alibaba has internally announced a reverse ban on Claude and other Anthropic products, requiring all employees to uninstall them by July 10, 2025. This follows accusations from Anthropic that Alibaba used approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5, 2025. This marks a significant corporate policy shift by a major Chinese tech company, potentially impacting how Chinese firms use foreign AI tools and intensifying competition in the AI industry. It also highlights growing tensions between US-based AI companies like Anthropic and Chinese enterprises over account abuse and security concerns. The ban affects Anthropic products including the Sonnet, Opus, and Fable models, as well as agent products like Claude Code. Prior to this, Alibaba had reimbursed employees for using external AI models such as Claude, GPT, and Gemini.

telegram · zaihuapd · Jul 8, 06:09

**Background**: Claude is a series of large language models developed by American company Anthropic, first released as an AI chatbot in March 2023. It uses constitutional AI for ethical alignment and includes models like Haiku, Sonnet, Opus, and Fable. Claude Code is an AI-assisted software development tool. Alibaba is a Chinese multinational conglomerate specializing in e-commerce, cloud computing, and AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model: Haiku, Sonnet, Opus, or Fable</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Alibaba`, `#Claude`, `#Anthropic`, `#corporate policy`

---