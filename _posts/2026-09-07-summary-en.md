---
layout: default
title: "Horizon Summary: 2026-09-07 (EN)"
date: 2026-09-07
lang: en
---

> From 33 items, 6 important content pieces were selected

---

1. [Huawei launches Kirin 9050 Pro with 'logic folding' after six-year chip hiatus](#item-1) ⭐️ 9.0/10
2. [LG Smart TVs Caught Logging Audio and Snooping on Home Networks](#item-2) ⭐️ 8.0/10
3. [OpenAI RSI Day Report Reveals Surge in Coding Agent Use](#item-3) ⭐️ 8.0/10
4. [Google TPU Inference Externalization Advances, Challenging NVIDIA's CUDA Moat](#item-4) ⭐️ 8.0/10
5. [LLM-Guided Program Evolution Breaks 10 Circle-Packing Records](#item-5) ⭐️ 8.0/10
6. [China's Top Court Issues Judicial Interpretation on AI Disputes](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Huawei launches Kirin 9050 Pro with 'logic folding' after six-year chip hiatus](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 9.0/10

At the Mate XT 2 launch in Guangzhou on September 7, Huawei unveiled the Kirin 9050 Pro, its first new flagship chip in six years. It is the first high-performance chip to use Huawei's 'logic folding' architecture, which stacks logic units vertically within a single die. The release breaks Huawei's six-year gap in flagship chip launches caused by US export controls, signaling renewed competitiveness in high-end mobile silicon. The logic folding approach may offer an alternative path to continue transistor scaling as Moore's Law slows, potentially reshaping the semiconductor landscape. Logic folding arranges logic layers like a duplex, adding vertical interconnect channels similar to elevators, which shortens signal paths and lowers latency. Search reports indicate the technique can increase transistor density by around 53 percent and may offer yields comparable to traditional 2D designs.

telegram · zaihuapd · Sep 7, 08:20

**Background**: Huawei has been largely barred from cutting-edge chip manufacturing since US export controls took effect in 2020, forcing it to rely on inventory and older process nodes. Logic folding is a 3D chip architecture that stacks logic cells vertically instead of placing them side by side on a flat die. The approach aims to bypass traditional photolithography limits and extend chip performance gains without relying solely on more advanced EUV equipment, which Huawei cannot currently access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/huawei-logicfolding-architecture-everything-you-need-to-know/">Huawei LogicFolding Architecture: Everything you need to know</a></li>
<li><a href="https://www.geeky-gadgets.com/huawei-logic-folding-moores-law/">Huawei Logic Folding: A New Approach to Moore's Law - Geeky ...</a></li>
<li><a href="https://chinaresearchcollective.substack.com/p/huawei-kirin-2026-logicfolding-a">Huawei Kirin 2026: LogicFolding - A Deep Dive into the Future ...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#Kirin chip`, `#semiconductors`, `#chip architecture`, `#mobile hardware`

---

<a id="item-2"></a>
## [LG Smart TVs Caught Logging Audio and Snooping on Home Networks](https://www.youtube.com/watch?v=6IFVTcM28KA) ⭐️ 8.0/10

An investigation by Gamers Nexus, reported by NotebookCheck and other outlets, found that LG Smart TVs running webOS can capture audio through their microphones even when the screen is off, and actively scan the local network to map nearby phones and other devices. The findings affect an estimated 216 million LG Smart TVs worldwide. This raises serious privacy and consent concerns for hundreds of millions of households, since televisions sit in the most intimate room of the home and can capture voice and device data without clear user awareness. It also highlights broader industry problems with IoT data collection and the limitations of consent obtained through terms of service. Tests showed the TVs log audio with the screen off, and they sweep local networks to identify connected devices. LG's terms reportedly require owners to obtain consent from guests whose voices may be captured, but critics argue such contractual clauses do not override wiretapping laws.

hackernews · treve · Sep 7, 00:22 · [Discussion](https://news.ycombinator.com/item?id=49592375)

**Background**: Modern smart TVs are essentially computers with microphones and internet connections, and many manufacturers use Automatic Content Recognition (ACR) to identify viewing habits for advertising. In this case, LG's webOS-powered TVs were found going further by capturing audio in standby mode and actively probing the local network to enumerate other devices. Network scanning can reveal when people are home and what devices they use, and the resulting data may be shared with third parties for profiling and ad targeting. LG is not alone; similar data-collection practices have been documented across brands such as Samsung and Sony.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/privacy/up-to-200m-lg-smart-tvs-could-be-secretly-listening-in-on-conversations/">LG smart TVs may log voice commands and scan homes | Cybernews</a></li>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and ...</a></li>
<li><a href="https://cybersecuritynews.com/lg-smart-tvs-caught-scanning-networks/">LG Smart TVs Caught Scanning Networks and Logging Audio in ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage and vindication, with some noting they had disabled network functions or physically removed the Wi-Fi/BT module from their TVs the first day they owned them. Others pointed out that LG's terms attempt to shift the burden of obtaining consent onto owners, while questioning whether such snooping violates all-party wiretap laws. Several said they would avoid buying LG products in the future.

**Tags**: `#privacy`, `#internet-of-things`, `#security`, `#smart-tv`

---

<a id="item-3"></a>
## [OpenAI RSI Day Report Reveals Surge in Coding Agent Use](https://simonwillison.net/2026/Sep/6/research-acceleration-the-view-inside-openai/) ⭐️ 8.0/10

OpenAI published an RSI-day essay, 'Research acceleration: The view inside OpenAI', revealing internal data showing that median daily AI spend per researcher jumped from near zero in February 2026 to roughly $600 by late August 2026. Simon Willison speculates the sharp acceleration in late July may correspond to employees gaining access to the model later released as GPT-6 Astra. This is the first detailed look at how a leading AI lab integrates coding agents into its own research workflow, confirming that agentic engineering has become a major driver of productivity and spending. It also signals OpenAI's strategic focus on recursive self-improvement, a path toward AGI that could reshape the entire AI research ecosystem. The chart included in the piece marks the year 2026 as when agentic engineering took off inside OpenAI, with a steep upward climb beginning in late July. The essay itself does not expand the acronym RSI, and OpenAI's Chief Scientist Jakub Pachocki also published a companion essay titled 'An Alien Mind' on the same day.

rss · Simon Willison · Sep 6, 23:57

**Background**: Recursive self-improvement (RSI) is a hypothesized process in which an AGI system rewrites its own code or contributes to improving subsequent AI systems, potentially leading to an intelligence explosion. Coding agents—also called agentic engineering—are software development systems where AI agents autonomously plan, write, test, and evolve code under human-defined goals and oversight, a practice that matured rapidly during 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-engineering">What is Agentic Engineering? | IBM</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI research`, `#coding agents`, `#recursive self-improvement`

---

<a id="item-4"></a>
## [Google TPU Inference Externalization Advances, Challenging NVIDIA's CUDA Moat](https://newsletter.semianalysis.com/p/tpu-inferencex-full-steam) ⭐️ 8.0/10

SemiAnalysis reports that Google's externalized TPU inference service, InferenceX, is gaining customers and can offer up to 50% better performance per dollar than NVIDIA. The service leverages Google's recent TPU hardware, including Ironwood and TPUv8i, to serve open-weight models through familiar inference engines. This development directly threatens NVIDIA's CUDA moat by giving AI companies a viable alternative for inference workloads with better price-performance. If InferenceX scales, it could shift significant AI inference traffic from NVIDIA GPUs to Google Cloud and pressure NVIDIA to cut prices. SemiAnalysis claims the 50% price-performance advantage is achieved when serving open-weight models through mainstream inference engines, not just Google's proprietary tooling. Ironwood is Google's seventh-generation TPU built for inference with up to 4,614 TFLOP/s peak performance, while Google's eighth-generation TPU lineup, announced in April 2026, adds a dedicated inference chip, TPUv8i.

rss · Semianalysis · Sep 7, 20:00

**Background**: Google develops custom Tensor Processing Units (TPUs) for AI workloads and has offered them on Google Cloud for years. 'Externalization' here refers to Google packaging its internal inference stack—software, kernels, and serving infrastructure—into a product that external customers can use, rather than just offering raw TPU access. NVIDIA's CUDA moat refers to the years of developer mindshare and optimized libraries that lock AI workloads to NVIDIA GPUs. Google aims to compete by engineering a full inference stack that matches or beats NVIDIA's price-performance on open-weight models.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/tpu-inferencex-full-steam">TPU Inference Externalization Full Steam Ahead - InferenceX</a></li>
<li><a href="https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/ironwood-tpu-age-of-inference/">Ironwood: The first Google TPU for the age of inference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#TPU`, `#Inference`, `#Google`, `#AI Hardware`, `#CUDA Moat`

---

<a id="item-5"></a>
## [LLM-Guided Program Evolution Breaks 10 Circle-Packing Records](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

Researchers used Discovery Loop, an LLM-guided program evolution system, to improve the best-known sum-of-radii solutions on the Packomania csqv benchmark for N=101 to 114. The 2.4%–5.4% improvements were obtained in 15 iterations at an LLM cost of $27.72, and Packomania independently accepted the results. The result shows that LLMs can drive verifiable improvements on a long-standing benchmark through program evolution rather than by solving the problem directly. Because the approach is largely task-agnostic, it may generalize to other hard optimization problems, although the reported gains are limited to a narrow set of instances. Each candidate algorithm proposed by the LLM is evaluated by an independent verifier, so only improvements are kept and failed attempts are discarded. The paper is at arXiv:2609.05093, with code and solutions on GitHub; the author particularly seeks critique on the plateau-detection stopping rule.

reddit · r/MachineLearning · /u/SIGH_I_CALL · Sep 7, 16:54

**Background**: Circle packing is a classic geometry problem concerned with arranging circles in a container so that no two circles overlap and, in many variants, no circle can be enlarged without creating an overlap. Packomania is a well-known website that tracks best-known packing results for many types of instances, including its csqv benchmark, and accepts independently verified improvements. Discovery Loop is a program-evolution system: instead of asking an LLM to design a final packing directly, it asks the LLM to modify a working search program, guided by a scoreboard of results and a history of prior attempts. This iterative process lets the model discover incremental algorithmic improvements at very low compute cost.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.05093">[2609.05093] LLM-Guided Program Evolution for Circle Packing ...</a></li>
<li><a href="https://arxiv.org/html/2609.05093v1">LLM-Guided Program Evolution for Circle Packing:Breaking 10 ...</a></li>
<li><a href="https://packomania.com/">Packomania (52C17)</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#program evolution`, `#optimization`, `#circle packing`, `#benchmark`

---

<a id="item-6"></a>
## [China's Top Court Issues Judicial Interpretation on AI Disputes](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 8.0/10

On September 7, China's Supreme People's Court issued a judicial interpretation on artificial intelligence dispute cases, consisting of five parts and 24 articles. It clarifies liability for AI face-swapping, algorithm-based price discrimination, fake celebrity endorsements, autonomous driving, and intellectual property issues. This is the first comprehensive judicial framework in China for resolving AI-related disputes, giving courts concrete rules to handle emerging harms around algorithmic fairness, privacy, and personality rights. It will directly affect AI developers, internet platforms, and consumers, providing clearer legal expectations and remedies. The interpretation explicitly states that using AI to create identifiable faces or voices without consent may constitute infringement of personality rights. It also says algorithmic price discrimination that harms consumers' rights should be subject to liability, AI-impersonated endorsements that induce purchases may trigger punitive damages, and privacy violations through 'network doxxing' or 'human flesh search' are regulated.

telegram · zaihuapd · Sep 7, 09:32

**Background**: AI face-swapping uses deep-learning techniques to replace a person's face or voice in images and audio/video, enabling convincing fake content that can be used for fraud and reputational harm. 'Big-data price discrimination' refers to platforms using collected user data and algorithms to show different prices for the same product or service to different users, a longstanding source of consumer complaints. 'Network kaihe' is a newer form of online violence that involves obtaining and publicly exposing someone's personal information, often with harassment or abuse. Earlier laws such as the Personal Information Protection Law and the Algorithmic Recommendation Provisions banned certain algorithmic discrimination; this judicial interpretation turns those principles into concrete civil liability rules for AI cases.

<details><summary>References</summary>
<ul>
<li><a href="https://baike.baidu.com/item/大数据杀熟/22456755">大数据杀熟 - 百度百科 AI算法杀熟被明令禁止：那些年，你多花的每一分钱，都是"聪明"的代价 算法加持下大数据“杀熟”？ - 知乎 我们是如何被“大数据杀熟”的？|算法|计算机|大模型|人工智能_网易订阅 大数据杀熟的原理是什么？ - 知乎</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/338972125">从程序员的角度出发：大数据杀熟，到底是什么原理？怎么反制？</a></li>
<li><a href="https://huacheng.gz-cmc.com/pages/2025/03/21/cea2cf981c354f08a4cfbbe028c401ef.html">起底“ 开 盒 ”：一个普通人的隐私信息只值80元</a></li>

</ul>
</details>

**Tags**: `#AI治理`, `#法律`, `#算法公平`, `#隐私保护`, `#司法解释`

---