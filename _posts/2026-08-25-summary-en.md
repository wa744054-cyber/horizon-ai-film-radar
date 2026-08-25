---
layout: default
title: "Horizon Summary: 2026-08-25 (EN)"
date: 2026-08-25
lang: en
---

> From 39 items, 13 important content pieces were selected

---

1. [Apple Unveils M6 and M5 Ultra Chips with Major AI Compute Leap](#item-1) ⭐️ 9.0/10
2. [OpenAI's Jalapeño Chip Reportedly Beats Nvidia Blackwell](#item-2) ⭐️ 9.0/10
3. [NVIDIA's First Vera Rubin NVL72 Benchmarks: 30x Throughput, 35x Cost Cut](#item-3) ⭐️ 9.0/10
4. [FDA authorizes first wearable for continuous ketone and glucose monitoring](#item-4) ⭐️ 8.0/10
5. [Apple Unveils Mac Studio with M5 Max and M5 Ultra](#item-5) ⭐️ 8.0/10
6. [Nitter Shuts Down All Instances After Cease and Desist](#item-6) ⭐️ 8.0/10
7. [Firefox 157 Enables JPEG XL by Default on All Platforms](#item-7) ⭐️ 8.0/10
8. [SpaceX Announces Starbase LA, a $100B Louisiana Launch Facility](#item-8) ⭐️ 8.0/10
9. [Frontier Performance via Continual Learning on Open-Weight Models for Sovereign AI](#item-9) ⭐️ 8.0/10
10. [SpaceX Plans Orbital Launch of Nvidia Vera Rubin NVL72 AI System](#item-10) ⭐️ 8.0/10
11. [Qwen teases Qwen3.8-Flash-Next MoE open source, previews Qwen4 architecture](#item-11) ⭐️ 8.0/10
12. [Tesla Supervised FSD Now Available in China](#item-12) ⭐️ 8.0/10
13. [Anthropic Q2 Revenue Surpasses $11.5B, Up 14x Year-Over-Year](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Apple Unveils M6 and M5 Ultra Chips with Major AI Compute Leap](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/) ⭐️ 9.0/10

Apple introduced the M6, its first 2nm chip with a 12-core CPU, 12-core GPU, and dual 16-core Neural Engine, alongside the M5 Ultra, which uses a quad-die architecture to become Apple's most powerful chip ever. The announcement signals a major leap in performance and on-device AI compute for Macs, intensifying competition with PC rivals and expanding possibilities for running large language models locally. It also reinforces Apple's push to differentiate its hardware through advanced chip design and neural engines. The M6 is Apple's first 2nm chip, while the M5 Ultra uses UltraFusion to connect two dual-die M5 Max chips, creating a quad-die architecture with inter-die bandwidth over 4.4TB/s and over 6x connection density. Pricing remains high, with a maxed-out Mac Studio configuration estimated at over $20,000.

hackernews · interpol_p · Aug 25, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49433292)

**Background**: Apple has been transitioning its Macs from Intel to its own ARM-based silicon since 2020, using a unified memory architecture and Neural Engine for AI acceleration. The M1 Ultra introduced Apple's UltraFusion packaging technology to combine two dies, and the M5 Ultra now extends this to a quad-die configuration. Process nodes have shrunk with each generation, making the 2nm M6 a significant manufacturing milestone.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M 6 and M5 Ultra for a big leap in... - Apple</a></li>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M 5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>
<li><a href="https://petapixel.com/2026/08/25/apple-unveils-m6-its-first-2-nanometer-chip-and-the-extremely-powerful-m5-ultra/">Apple Unveils M 6 , its First 2-Nanometer Chip , and the... | PetaPixel</a></li>

</ul>
</details>

**Discussion**: Commenters are impressed by the performance gains, with one M1 Pro owner noting the M5 Pro felt significantly quicker in a brief store test, and another drawing a humorous comparison to late-90s chip wars. However, several users question whether the high price is justified for local LLM use, since cloud models still outperform local ones, while others point out that current prices are roughly inflation-adjusted to late-1980s Mac levels.

**Tags**: `#Apple`, `#hardware`, `#AI`, `#M5 Ultra`, `#M6`

---

<a id="item-2"></a>
## [OpenAI's Jalapeño Chip Reportedly Beats Nvidia Blackwell](https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia) ⭐️ 9.0/10

OpenAI has published the first benchmark results for 'Jalapeño', its self-designed inference ASIC developed with Broadcom. The chip reportedly delivers 1.5–1.9x higher throughput per watt, 1.7–3.6x lower latency, and 2.1–4.1x higher interactive performance than Nvidia's GB300 on models such as GPT-OSS 120B, DeepSeek R1 670B, and Kimi K2.5 1T. If the results hold up, custom ASICs could become a serious competitor to Nvidia GPUs for the fast-growing inference market, potentially disrupting Nvidia's pricing power and accelerating the trend of large AI labs designing their own silicon. It also suggests token prices will keep falling as inference hardware becomes cheaper and more efficient. The chip has a rated power of 700W but sustained draw of no more than 550W in tests. It was benchmarked against Nvidia's GB300, not the just-shipping Vera Rubin, and it is not intended for model training; OpenAI plans to deploy it in its own compute facilities by the end of the year, with a second generation in advanced development and a third being designed.

hackernews · Semianalysis · Aug 25, 14:06 · [Discussion](https://news.ycombinator.com/item?id=49434378)

**Background**: An ASIC (application-specific integrated circuit) is a chip customized for a particular task rather than general-purpose use, offering better speed, power efficiency, and silicon utilization than GPUs. AI inference is using a trained model to make predictions on new data, and it has become a major cost driver as large language models are deployed widely. Nvidia's Blackwell architecture, including the GB300 processor used in the comparison, currently dominates AI infrastructure. By designing a custom inference ASIC, OpenAI aims to reduce its reliance on Nvidia and improve the economics of serving large models at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-inference">What is AI Inference? - Machine learning</a></li>

</ul>
</details>

**Discussion**: Commenters are enthusiastic but measured: some see custom inference chips following the early 3dfx/Riva/PowerVR era and expect token prices to keep plummeting, while others point out that the comparison excluded Nvidia's newest Vera Rubin and wonder if a model-specific chip will remain useful as models evolve. One commenter speculates about baking LLM weights directly into silicon, and several praise SemiAnalysis's hands-on, independent style.

**Tags**: `#OpenAI`, `#AI chips`, `#Nvidia`, `#hardware`, `#inference`

---

<a id="item-3"></a>
## [NVIDIA's First Vera Rubin NVL72 Benchmarks: 30x Throughput, 35x Cost Cut](https://blogs.nvidia.com/blog/vera-rubin-nvl72-efficiency-ai-agents/) ⭐️ 9.0/10

NVIDIA announced the first on-chip benchmark results for its Vera Rubin NVL72 rack-scale system. Using DeepSeek-V4-Pro for agentic coding tasks, throughput per megawatt improved by up to 30x and cost per million tokens dropped by up to 35x compared to GB300. This is a major milestone for AI infrastructure, showing order-of-magnitude gains in efficiency and cost for agentic workloads. It could accelerate adoption of rack-scale architectures and reshape the economics of large-scale AI inference. The Vera Rubin NVL72 combines 72 Rubin GPUs, 36 Vera CPUs, NVLink 6 switching, ConnectX-9 SuperNICs, and BlueField-4 DPUs in a liquid-cooled rack. NVIDIA also announced that the Groq 3 LPX inference accelerator is entering full production (3400 tokens/s on Gemma 4 31B), and SpaceXAI plans to deploy Vera CPUs in space by 2028.

telegram · zaihuapd · Aug 25, 14:48

**Background**: Vera Rubin NVL72 is NVIDIA's next-generation rack-scale supercomputer, following the GB300 (Blackwell Ultra). Unlike traditional GPU cards, it treats the entire rack as a single giant GPU, optimized for large-context agentic workloads. Groq 3 LPX is a co-designed heterogeneous inference accelerator for the Rubin platform, and the Vera CPU is an agent-specific processor.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/the-yoda-scrolls_nvidia-vera-rubin-nvl72-activity-7414932954453422080-kXDa">NVIDIA Unveils Vera Rubin NVL 72 Rack-Scale... | LinkedIn</a></li>
<li><a href="https://benquan.hk/article-vera-rubin-nvl72.html">NVIDIA Vera Rubin NVL 72 Deep Dive 2026 | BENQUAN Global</a></li>
<li><a href="https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/">Inside NVIDIA Groq 3 LPX: The Low-Latency Inference Accelerator for the NVIDIA Vera Rubin Platform | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: No community comments were provided.

**Tags**: `#NVIDIA`, `#Vera Rubin`, `#AI hardware`, `#inference`, `#DeepSeek`

---

<a id="item-4"></a>
## [FDA authorizes first wearable for continuous ketone and glucose monitoring](https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar) ⭐️ 8.0/10

The U.S. Food and Drug Administration has authorized the Libre Duo 10 Day, the first wearable device that continuously monitors both ketone and glucose levels in interstitial fluid, transmitting readings wirelessly to a smartphone every minute, day and night. This authorization marks a significant advancement in diabetes and metabolic health management, offering people with diabetes a single sensor to detect both dangerous ketone buildup (diabetic ketoacidosis) and glucose fluctuations in real time, potentially improving early intervention and reducing complications. The device, called the Libre Duo 10 Day, is worn for up to 10 days and measures biomarkers in the interstitial fluid just beneath the skin every minute, sending data wirelessly to a compatible smartphone. The FDA's announcement highlights that the authorization addresses a gap where ketone levels are typically only measured via fingerstick or urine tests, but it does not specify the intended patient population.

hackernews · sunnynagra · Aug 25, 19:07 · [Discussion](https://news.ycombinator.com/item?id=49439017)

**Background**: Ketones are acids produced when the body breaks down fat for energy instead of glucose, and their buildup can lead to diabetic ketoacidosis (DKA), a life-threatening complication most common in type 1 diabetes. Traditionally, ketone levels are measured through blood or urine tests, and glucose is monitored separately via continuous glucose monitors (CGMs). This new device combines both measurements into a single wearable, simplifying daily management for people with diabetes. Continuous ketone monitoring is an emerging area of research, with companies like Abbott and startups developing similar dual-sensor biowearables.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar">FDA Authorizes First Wearable Device That Continuously Monitors Both Ketone Levels and Blood Sugar | FDA</a></li>
<li><a href="https://www.abbott.com/en-us/corpnewsroom/strategy-and-strength/abbotts-biowearable-one-sensor-for-glucose-ketones">Abbott's Biowearable: One Sensor for Glucose, Ketones | Newsroom</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8258504/">Continuous Ketone Monitoring : A New Paradigm for Physiologic...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed hope about the future of automated glucose control and accessibility, while also voicing skepticism about the accuracy of noninvasive sensing and the practical usefulness of ketone monitoring for average diabetics. One user shared a personal story about a friend who died of diabetic ketoacidosis, reflecting on the significance of the advancement, while another asked how long the underlying technology has existed.

**Tags**: `#FDA`, `#wearable`, `#diabetes`, `#health tech`, `#medical devices`

---

<a id="item-5"></a>
## [Apple Unveils Mac Studio with M5 Max and M5 Ultra](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/) ⭐️ 8.0/10

Apple has announced new Mac Studio models powered by the M5 Max and M5 Ultra chips, highlighting their capabilities for local AI and high memory bandwidth. The press release emphasizes 'up to' 1.2 TB/s memory bandwidth on the M5 Ultra, positioning the machine as Apple's most powerful Mac yet. This release matters because it significantly boosts on-device AI performance, potentially making it easier to run large language models locally without cloud dependence. It also sparks community debate about pricing, memory capacity, and whether the machine is future-proof for larger models. The M5 Ultra is built from two M5 Max dies connected by an inter-die fabric, achieving 1.2 TB/s total memory bandwidth (614 GB/s per die). Memory configurations go up to 256GB at roughly $10,000, with a 512GB option expected later; Thunderbolt 5 provides 120Gb/s external I/O.

hackernews · interpol_p · Aug 25, 13:03 · [Discussion](https://news.ycombinator.com/item?id=49433316)

**Background**: Local AI refers to running artificial intelligence models directly on a device, such as a Mac, rather than sending data to cloud servers. Memory bandwidth is the rate at which data can be read from or stored into memory, and it is a critical bottleneck for large models because the weights and activations must be moved quickly. Apple's unified memory architecture allows the CPU and GPU to share the same memory pool, which is why bandwidth figures are central to assessing AI performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Memory_bandwidth">Memory bandwidth</a></li>
<li><a href="https://localai.io/">LocalAI · Make AI run on every machine</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise Apple for leaning into local AI and hope for optimized frontier open-weight models to ship included, while others criticize the heavy use of 'up to' in the press release and the high cost of high-memory configurations. Technical users analyze bandwidth numbers, estimating that the M5 Ultra could deliver around 1000+ tokens per second prefill and 50+ tokens per second generation for models like Deepseek V4, but they question 'future-proofing' for models exceeding 1 trillion parameters.

**Tags**: `#Apple`, `#Mac Studio`, `#M5`, `#Local AI`, `#Hardware`

---

<a id="item-6"></a>
## [Nitter Shuts Down All Instances After Cease and Desist](https://github.com/zedeus/nitter/issues/1442) ⭐️ 8.0/10

Nitter has received cease and desist letters, prompting all public instances to go down for the foreseeable future while the project awaits legal advice. The announcement was made on the project's GitHub issue tracker. This legal action threatens a widely used privacy tool that lets people read X (Twitter) content without ads, JavaScript, or tracking. It also raises concerns about the vulnerability of open-source projects to cease-and-desist threats based on terms-of-service violations. The exact sender of the cease and desist letters has not been disclosed, and the project's legal team is currently evaluating options. Community members confirmed that popular instances such as xcancel.com are also down.

hackernews · Banditoz · Aug 25, 17:08 · [Discussion](https://news.ycombinator.com/item?id=49437283)

**Background**: Nitter is a free and open-source alternative front-end for Twitter/X, written in Nim, that routes requests through its backend to provide a fast, lightweight browsing experience without JavaScript, ads, or tracking. It has been a popular tool for privacy-conscious users and for those who want to read tweets without logging in. The project was inspired by Invidious, a similar privacy front-end for YouTube. This legal action could set a precedent for other alternative front-end projects.

<details><summary>References</summary>
<ul>
<li><a href="https://nlnet.nl/project/Nitter/">NLnet; Nitter</a></li>
<li><a href="https://alternativeto.net/software/nitter/about/">Nitter : Free and open-source front-end mirror of Twitter... | AlternativeTo</a></li>

</ul>
</details>

**Discussion**: Commenters expressed disappointment and concern, with some noting that X is still used by organizations like local councils for official updates, making Nitter an important access point. Others reflected on the broader trend of companies using ToS claims to shut down community projects, and a few shared lessons from how other platforms handle clones, like Hacker News.

**Tags**: `#Nitter`, `#Twitter`, `#Legal`, `#Open Source`, `#Privacy`

---

<a id="item-7"></a>
## [Firefox 157 Enables JPEG XL by Default on All Platforms](https://groups.google.com/a/mozilla.org/g/dev-platform/c/3YMV4MS34KA?pli=1) ⭐️ 8.0/10

Mozilla announced that Firefox 157 will ship JPEG XL support enabled by default on all platforms. Chromium is also adopting JPEG XL, making this a major step for the image format's adoption on the web. This is significant because both major browser engines, Gecko and Blink, will support JPEG XL out of the box, potentially making it a practical replacement for legacy JPEG and PNG. It could drive broader adoption of a more efficient image format across the web and impact developers and users alike. Both Firefox and Chromium are using the Rust-based jxl-rs library for JPEG XL support. Apple previously shipped libjxl (C++) in its platforms, but its future plans remain unclear, and there are open questions about memory safety and performance comparisons.

hackernews · yboris · Aug 25, 17:55 · [Discussion](https://news.ycombinator.com/item?id=49437946)

**Background**: JPEG XL is a modern image format developed by the JPEG committee, Google, and Cloudinary, supporting both lossy and lossless compression with better efficiency than JPEG and PNG. It is a free and open standard defined by ISO/IEC 18181, designed as a long-term successor to JPEG. Browser support has been slow to arrive; Firefox previously offered JPEG XL behind a flag, while Chromium at one point removed it. This news marks renewed momentum for the format's adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JPEG_XL">JPEG XL</a></li>
<li><a href="https://jpegxl.info/">JPEG XL : Superior Image Compression</a></li>

</ul>
</details>

**Discussion**: Commenters noted that both Firefox and Chromium rely on the Rust-based jxl-rs implementation and wondered what Apple will do with its existing C++ libjxl deployment. Others discussed practical concerns, such as uploading JXL images to sites that don't support them, and whether older operating systems like Windows 7/8 will be supported.

**Tags**: `#firefox`, `#jpeg-xl`, `#web standards`, `#browser`, `#image format`

---

<a id="item-8"></a>
## [SpaceX Announces Starbase LA, a $100B Louisiana Launch Facility](https://www.spacex.com/sites/starbase-la) ⭐️ 8.0/10

On August 25, 2026, SpaceX officially announced Starbase LA, a new high-cadence launch facility to be built on marshland at Pecan Island in Vermillion Parish, Louisiana. The site is intended to launch Starship rockets carrying Starlink satellites and orbital data centers, with a reported investment of $100 billion. This marks a major expansion of SpaceX's launch infrastructure beyond Texas and Florida, potentially bringing decades of construction and aerospace jobs to one of the poorest coastal regions in the United States. The site's latitude may also improve access to sun-synchronous orbits, which are valuable for Starlink and orbital data center missions. The announcement follows months of speculation, with local realtors calling the plan as early as May and Ars Technica covering rumors earlier in August. Community members noted the sun-synchronous orbit launch angle of about 98 degrees as a key technical benefit, while also raising doubts about SpaceX's timeline and pointing out that the official page contains near-identical paragraphs that appear machine-generated.

hackernews · bilsbie · Aug 25, 16:37 · [Discussion](https://news.ycombinator.com/item?id=49436822)

**Background**: Launch site latitude is a critical factor in orbital mechanics because it determines the orbital inclination a rocket can reach without extra fuel. Launches near the equator gain extra speed from Earth's rotation for easterly orbits, while higher-latitude sites are often better suited for high-inclination orbits such as sun-synchronous orbits. SpaceX already operates Starbase in Texas and other launch facilities, and Starship is designed to support rapid, high-cadence launches of heavy cargo.

<details><summary>References</summary>
<ul>
<li><a href="https://www.spacex.com/sites/starbase-la">SpaceX - Starbase , LA</a></li>
<li><a href="https://www.fox8live.com/2026/08/25/spacex-announces-plan-build-100-billion-starbase-louisiana-launch-facility/">SpaceX announces plan to build $100 billion ‘ Starbase Louisiana ...</a></li>
<li><a href="https://everydayastronaut.com/why-dont-they-just-launch-rockets-from-mountains-or-the-equator/">Why Don't They Just Launch Rockets From... | Everyday Astronaut</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly enthusiastic about the regional economic boost, with one predicting 10 to 20 years of solid work for welders, concrete workers, and tradespeople in coastal Louisiana. Others expressed cautious optimism about ambitious real-world projects, but several were skeptical of Musk's timelines, and one user mocked the website copy for repeating entire sentences verbatim and another noted Elon had previously dismissed flame trenches.

**Tags**: `#SpaceX`, `#aerospace`, `#engineering`, `#orbital mechanics`

---

<a id="item-9"></a>
## [Frontier Performance via Continual Learning on Open-Weight Models for Sovereign AI](https://www.reddit.com/r/MachineLearning/comments/1vxvzju/continual_learning_of_frontier_models_for/) ⭐️ 8.0/10

A new technical report argues that frontier-level AI performance can be achieved by a wide range of institutions through continual learning on readily available open-weight models. The report introduces Thomson, an open-weights general-purpose frontier model focused on high-stakes professional work such as legal, tax, safety, and multilingual tasks. This challenges the common assumption that only a few heavily funded labs can build frontier models, potentially reducing the information, economic, and power asymmetry between AI developers and users. If validated, the approach could make sovereign AI—independent building, deployment, and governance of AI—viable for many more organizations, governments, and communities. The continual learning approach introduces safeguards that preserve both plasticity and stability at each training stage, while making only a minimal number of high-impact parameter interventions. Thomson reportedly shows a distinctive π-shaped improvement pattern, gaining across many capabilities with almost no catastrophic forgetting, and achieves these results with compute and personnel budgets substantially lower than typical frontier development.

reddit · r/MachineLearning · /u/Forsaken_Scientist · Aug 25, 10:30

**Background**: Continual learning, also called lifelong learning, allows machine learning models to adapt to new data over time while retaining previously learned knowledge. Open-weight models publish the trained neural network weights, enabling others to use and fine-tune them, unlike closed API-only models. Sovereign AI refers to the capacity of a state, federation, or community to develop, deploy, or govern AI systems aligned with its laws, values, and public interest. This work combines these ideas to propose a practical path toward frontier AI ownership beyond a few large companies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/continual-learning">What is Continual Learning? | IBM</a></li>
<li><a href="https://medium.com/lets-code-future/open-weight-ai-models-what-they-are-and-why-openais-next-move-matters-f86fe481973a">Open - Weight AI Models : What They Are , and Why... | Medium</a></li>
<li><a href="https://www.selfdriven.ai/research/sovereignity">Sovereignity - Research - selfdrivenAI — selfdrivenAI</a></li>

</ul>
</details>

**Tags**: `#continual learning`, `#sovereign AI`, `#open-weight models`, `#frontier models`, `#AI governance`

---

<a id="item-10"></a>
## [SpaceX Plans Orbital Launch of Nvidia Vera Rubin NVL72 AI System](https://www.theregister.com/off-prem/2026/08/25/spacex-claims-it-will-put-a-vera-rubin-nvl72-rack-scale-system-into-orbit-next-year/5292067) ⭐️ 8.0/10

SpaceX has announced plans to launch an Nvidia Vera Rubin NVL72 rack-scale AI system into orbit by 2027 to test AI computing in space. The company has not yet disclosed specific launch dates, orbital altitude, or power and cooling solutions. This initiative could mark a significant step toward orbital data centers and space-based AI infrastructure, potentially shifting how large-scale compute is deployed. However, as a preliminary plan without technical details, its feasibility and impact remain to be demonstrated. The Vera Rubin NVL72 combines 72 Rubin GPUs and 36 Vera CPUs into a single liquid-cooled rack-scale system, consuming over 100 kilowatts of power. Launching it into orbit requires solving challenges related to power generation, thermal management, radiation shielding, and communications.

telegram · zaihuapd · Aug 25, 08:03

**Background**: A rack-scale AI system integrates GPUs, CPUs, memory, and networking into a single chassis that can be managed as one large computer, designed to run large-scale AI workloads efficiently. Nvidia's Vera Rubin platform is the next-generation architecture following Hopper and Blackwell, with the NVL72 acting as a rack-scale supercomputer. Orbital data centers are a futuristic concept where high-performance computing infrastructure is placed in Earth's orbit, potentially offering advantages such as unlimited solar power and global coverage, though the idea remains controversial and early-stage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/rubin/">Infrastructure for Scalable AI Reasoning | NVIDIA Vera Rubin Platform</a></li>
<li><a href="https://win.ai/resources/blog/27-vera-rubin-nvl72-what-next-gen-training-infra-means">Vera Rubin NVL 72 cost and operational trade offs</a></li>
<li><a href="https://shaam.blog/articles/orbital-ai-data-centers-hype-vs-reality">Orbital AI Data Centers : Hype or the Future of Computing?</a></li>

</ul>
</details>

**Tags**: `#Space computing`, `#AI hardware`, `#Nvidia`, `#SpaceX`, `#Orbital data center`

---

<a id="item-11"></a>
## [Qwen teases Qwen3.8-Flash-Next MoE open source, previews Qwen4 architecture](https://www.modelscope.cn/models/Qwen/Qwen3.8-Flash-Next) ⭐️ 8.0/10

Qwen has published a preview page on ModelScope for Qwen3.8-Flash-Next, a multimodal MoE model expected to be released on August 26, 2026 at 23:00 UTC+8, in standard and FP8 versions. The model is built on the upcoming Qwen4 architecture and is open-sourced early to prepare the community for the Qwen4 series. This is significant because it marks the first public preview of the Qwen4 architecture, giving developers an early look at Alibaba's next-generation model design before the full Qwen4 release. The open-source MoE approach also signals continued community-centered model development in the competitive AI landscape. The release will include both a standard version and an FP8 quantized version, and the model is a multimodal MoE. On Hugging Face, the project is described as "A Preview of the Qwen 4 Architecture" and lists Qwen/Qwen3.8-Flash-Next as the planned artifact.

telegram · zaihuapd · Aug 25, 12:59

**Background**: Mixture of Experts (MoE) is an architecture that divides a model into multiple specialized subnetworks, or "experts," and activates only a subset of them for each input, improving efficiency and reducing compute costs. FP8 is an 8-bit floating-point format that lowers memory usage and speeds up inference, often with minimal accuracy loss. Qwen3.8-Flash-Next is positioned as an early preview of Qwen4, Alibaba's next-generation AI model architecture, ahead of the full Qwen4 series launch.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen/Qwen3.8-Flash-Next · Upcoming release · Hugging Face</a></li>
<li><a href="https://www.linkedin.com/pulse/mixture-experts-moearchitecture-padmashri-suresh-o5nqc">Mixture of Experts ( MoE ) architecture</a></li>
<li><a href="https://buttondown.com/justincormack/archive/ignore-previous-directions-6-floating-points/">Ignore previous directions 6: floating points • Buttondown</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#MoE`, `#AI`, `#open-source`, `#model-release`

---

<a id="item-12"></a>
## [Tesla Supervised FSD Now Available in China](https://t.me/zaihuapd/43397) ⭐️ 8.0/10

On May 21, 2026, Tesla announced via a post on X that its supervised Full Self-Driving (FSD) system can now be used in China. This marks the official entry of the system into one of the world's largest automotive markets. The launch gives Tesla a strategic foothold in China's competitive EV and autonomous-driving market, where local players like BYD and Huawei are pushing advanced driver-assistance features. It also tests how Tesla's vision-based FSD performs under China's complex traffic conditions and strict data-regulation framework. According to reports, Tesla had previously run small-scale tests of FSD V13 on 24 domestic models with about 5,000 owners. Tesla's Shanghai data center retains all in-country data, its Lingang AI training center entered operation in February 2026, and it cooperates with Baidu Maps to use compliant high-definition maps.

telegram · zaihuapd · Aug 25, 13:42

**Background**: Full Self-Driving (Supervised) is Tesla's most advanced consumer driver-assistance product, capable of navigating, steering, changing lanes, and parking under active driver supervision; it is not fully autonomous. In China, autonomous-driving features face strict regulatory requirements, including data localization and map licensing, which Tesla has addressed through its Shanghai data center, local AI training hub, and Baidu Maps partnership.

<details><summary>References</summary>
<ul>
<li><a href="https://post.smzdm.com/p/a825z5e7/">中国被 特 斯 拉 移出 FSD ...</a></li>
<li><a href="https://www.ithome.com/0/992/918.htm">特 斯 拉 官网更新： 监 督 版 FSD 支持地区不再包含中国 - IT之家</a></li>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving ( Supervised ) | Tesla</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#FSD`, `#autonomous driving`, `#AI`, `#China`

---

<a id="item-13"></a>
## [Anthropic Q2 Revenue Surpasses $11.5B, Up 14x Year-Over-Year](https://t.me/zaihuapd/43403) ⭐️ 8.0/10

Bloomberg reports, citing documents, that Anthropic's preliminary Q2 revenue exceeded $11.5 billion, a more than 14-fold increase year-over-year. The company also turned an adjusted operating profit for the quarter. This marks a major business milestone for one of the leading AI labs, showing rapid commercialization of its AI models. With a possible large IPO in the fall, the results could significantly shape the AI industry's investment landscape. The preliminary figures remain subject to adjustment, and they compare with $787 million in the same quarter a year earlier and $4.73 billion in Q1 2026. Anthropic is reportedly preparing for a large IPO that could launch this fall.

telegram · zaihuapd · Aug 25, 17:32

**Background**: Anthropic is an AI safety and research company founded by former OpenAI researchers, known for its Claude series of large language models. Strong revenue growth suggests rising enterprise demand for its AI products, and an IPO would provide public market investors a major pure-play AI exposure.

**Tags**: `#Anthropic`, `#AI`, `#IPO`, `#revenue`, `#business`

---