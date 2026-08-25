---
layout: default
title: "Horizon Summary: 2026-08-25 (ZH)"
date: 2026-08-25
lang: zh
---

> 从 39 条内容中筛选出 13 条重要资讯。

---

1. [苹果发布 M6 与 M5 Ultra 芯片，性能与 AI 算力大幅跃升](#item-1) ⭐️ 9.0/10
2. [OpenAI 自研芯片 Jalapeño 据称超越 Nvidia Blackwell](#item-2) ⭐️ 9.0/10
3. [英伟达首次测试 Vera Rubin NVL72：吞吐提升 30 倍，成本降低 35 倍](#item-3) ⭐️ 9.0/10
4. [FDA 批准首款可穿戴设备，持续监测酮体和血糖](#item-4) ⭐️ 8.0/10
5. [苹果发布搭载 M5 Max 和 M5 Ultra 的全新 Mac Studio](#item-5) ⭐️ 8.0/10
6. [Nitter 收到停止函后关闭所有实例](#item-6) ⭐️ 8.0/10
7. [Firefox 157 默认启用 JPEG XL，覆盖所有平台](#item-7) ⭐️ 8.0/10
8. [SpaceX 正式公布路易斯安那州 Starbase LA 发射场，投资规模达千亿美元](#item-8) ⭐️ 8.0/10
9. [在开放权重模型上持续学习实现前沿性能，助力主权 AI](#item-9) ⭐️ 8.0/10
10. [SpaceX 计划将英伟达 Vera Rubin NVL72 送入轨道，测试太空 AI 计算](#item-10) ⭐️ 8.0/10
11. [Qwen 预告 8 月 26 日开源 Qwen3.8-Flash-Next，基于 Qwen4 架构](#item-11) ⭐️ 8.0/10
12. [特斯拉监督版 FSD 在中国正式可用](#item-12) ⭐️ 8.0/10
13. [Anthropic 第二季营收超 115 亿美元，同比增长逾 14 倍](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [苹果发布 M6 与 M5 Ultra 芯片，性能与 AI 算力大幅跃升](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/) ⭐️ 9.0/10

苹果发布了首款采用 2 纳米制程的 M6 芯片，配备 12 核 CPU、12 核 GPU 和双 16 核神经引擎；同时推出采用四芯片架构的 M5 Ultra，这是苹果迄今最强大的芯片。 这一发布标志着 Mac 在性能和端侧 AI 算力上的重大飞跃，加剧了与 PC 对手的竞争，并扩展了本地运行大语言模型的可能性。同时也强化了苹果通过先进芯片设计和神经引擎实现硬件差异化的策略。 M6 是苹果首款 2 纳米制程芯片；M5 Ultra 通过 UltraFusion 连接两颗双芯片 M5 Max，形成四芯片架构，芯片间带宽超过 4.4TB/s，连接密度提升 6 倍以上。价格仍然偏高，顶配 Mac Studio 配置估计超过 2 万美元。

hackernews · interpol_p · 8月25日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49433292)

**背景**: 自 2020 年以来，苹果一直将 Mac 从 Intel 过渡到自研的基于 ARM 架构的芯片，采用统一内存架构和神经引擎来加速 AI。M1 Ultra 首次引入 UltraFusion 封装技术将两颗芯片组合，M5 Ultra 则扩展为四芯片配置。制程工艺逐代缩小，2 纳米的 M6 因此成为制造上的重要里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M 6 and M5 Ultra for a big leap in... - Apple</a></li>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M 5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>
<li><a href="https://petapixel.com/2026/08/25/apple-unveils-m6-its-first-2-nanometer-chip-and-the-extremely-powerful-m5-ultra/">Apple Unveils M 6 , its First 2-Nanometer Chip , and the... | PetaPixel</a></li>

</ul>
</details>

**社区讨论**: 评论者对性能提升印象深刻，一位 M1 Pro 用户表示在商店短暂测试中 M5 Pro 明显更快；还有人幽默地将其比作 90 年代末的芯片大战。然而，一些用户质疑高价是否值得用于本地大语言模型，因为云模型性能仍优于本地模型；另一些人则指出当前价格经通胀调整后大致相当于 80 年代末 Mac 的水平。

**标签**: `#Apple`, `#hardware`, `#AI`, `#M5 Ultra`, `#M6`

---

<a id="item-2"></a>
## [OpenAI 自研芯片 Jalapeño 据称超越 Nvidia Blackwell](https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia) ⭐️ 9.0/10

OpenAI 公布了与博通合作的首款自研推理芯片 Jalapeño 的初步测试数据。该芯片据称在 GPT-OSS 120B、DeepSeek R1 670B 和 Kimi K2.5 1T 等模型上，单位功耗吞吐量比英伟达 GB300 高 1.5 至 1.9 倍，端到端延迟低 1.7 至 3.6 倍，高交互场景性能高 2.1 至 4.1 倍。 如果结果属实，定制 ASIC 可能在快速增长的推理市场中成为英伟达 GPU 的有力竞争对手，可能削弱英伟达的定价权，并加速大型 AI 实验室自研芯片的趋势。这也意味着随着推理硬件更便宜、更高效，token 价格将继续下降。 该芯片额定功耗为 700 瓦，实测持续功耗不高于 550 瓦。基准测试对比的是英伟达 GB300，而非刚开始出货的 Vera Rubin，而且该芯片不用于模型训练；OpenAI 计划年底前在自有算力设施中部署，第二代已深入开发，第三代正在设计。

hackernews · Semianalysis · 8月25日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=49434378)

**背景**: ASIC（专用集成电路）是为特定任务定制的芯片，而非通用处理器，因此在速度、能效和硅片利用率上通常优于 GPU。AI 推理是指用训练好的模型对新数据做出预测，随着大型语言模型被广泛部署，推理已成为主要成本来源。英伟达的 Blackwell 架构（包括对比中使用的 GB300）目前主导着 AI 基础设施。OpenAI 设计定制推理芯片，旨在减少对英伟达的依赖，并改善大规模模型服务的经济性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-inference">What is AI Inference? - Machine learning</a></li>

</ul>
</details>

**社区讨论**: 评论者热情但持谨慎态度：有人认为定制推理芯片正像是早期 3dfx/Riva/PowerVR 格局的重现，并预计 token 价格会继续暴跌；也有人指出对比并未包含英伟达最新的 Vera Rubin，并质疑针对特定模型的芯片能否在模型迭代中保持价值。还有评论者设想直接把大模型权重烧录进芯片，也有人赞赏 SemiAnalysis 独立、接地气的分析风格。

**标签**: `#OpenAI`, `#AI chips`, `#Nvidia`, `#hardware`, `#inference`

---

<a id="item-3"></a>
## [英伟达首次测试 Vera Rubin NVL72：吞吐提升 30 倍，成本降低 35 倍](https://blogs.nvidia.com/blog/vera-rubin-nvl72-efficiency-ai-agents/) ⭐️ 9.0/10

英伟达首次公布了新一代机柜级系统 Vera Rubin NVL72 的片上实测数据。用 DeepSeek-V4-Pro 运行智能体编码任务时，每兆瓦吞吐量较 GB300 最高提升 30 倍，每百万 Token 成本最高下降 35 倍。 这是 AI 基础设施的一个重要里程碑，表明智能体工作负载的效率和成本呈数量级改善。它可能加速机柜级架构的采用，并重塑大规模 AI 推理的经济形态。 Vera Rubin NVL72 在一个液冷机柜中集成了 72 个 Rubin GPU、36 个 Vera CPU、NVLink 6 交换器、ConnectX-9 SuperNIC 和 BlueField-4 DPU。英伟达还宣布推理加速器 Groq 3 LPX 进入全面量产（在 Gemma 4 31B 上输出 3400 Token/秒），SpaceXAI 计划在 2028 年将 Vera CPU 部署到太空。

telegram · zaihuapd · 8月25日 14:48

**背景**: Vera Rubin NVL72 是英伟达继 GB300（Blackwell Ultra）之后的下一代机柜级超级计算机。与传统 GPU 卡不同，它将整个机柜视作一个巨型 GPU，针对大上下文智能体工作负载进行优化。Groq 3 LPX 是与 Rubin 平台协同设计的异构推理加速器，Vera CPU 则是面向智能体的专用处理器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/the-yoda-scrolls_nvidia-vera-rubin-nvl72-activity-7414932954453422080-kXDa">NVIDIA Unveils Vera Rubin NVL 72 Rack-Scale... | LinkedIn</a></li>
<li><a href="https://benquan.hk/article-vera-rubin-nvl72.html">NVIDIA Vera Rubin NVL 72 Deep Dive 2026 | BENQUAN Global</a></li>
<li><a href="https://developer.nvidia.com/blog/inside-nvidia-groq-3-lpx-the-low-latency-inference-accelerator-for-the-nvidia-vera-rubin-platform/">Inside NVIDIA Groq 3 LPX: The Low-Latency Inference Accelerator for the NVIDIA Vera Rubin Platform | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 未提供社区评论。

**标签**: `#NVIDIA`, `#Vera Rubin`, `#AI hardware`, `#inference`, `#DeepSeek`

---

<a id="item-4"></a>
## [FDA 批准首款可穿戴设备，持续监测酮体和血糖](https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar) ⭐️ 8.0/10

美国食品药品监督管理局（FDA）已批准 Libre Duo 10 Day——首款可穿戴设备，可持续监测组织间液中的酮体和葡萄糖水平，并每分钟通过无线方式将读数发送到智能手机。 这一批准标志着糖尿病和代谢健康管理领域的重大进步，为糖尿病患者提供了单一传感器，可实时检测危险的酮体堆积（糖尿病酮症酸中毒）和血糖波动，可能有助于早期干预并减少并发症。 这款名为 Libre Duo 10 Day 的设备可佩戴长达 10 天，每分钟测量皮肤下组织间液中的生物标志物，并通过无线方式将数据发送到兼容的智能手机。FDA 的公告强调，该授权填补了以往仅能通过指尖采血或尿液检测来测量酮体水平的空白，但未明确说明预期的患者群体。

hackernews · sunnynagra · 8月25日 19:07 · [社区讨论](https://news.ycombinator.com/item?id=49439017)

**背景**: 酮体是身体在无法利用葡萄糖时转而分解脂肪产生的酸性物质，其积聚可能导致糖尿病酮症酸中毒（DKA），这是 1 型糖尿病患者最常见的危及生命的并发症。传统上，酮体需通过血液或尿液检测来测量，而血糖则需通过连续血糖监测仪（CGM）单独监测。这款新设备将这两项测量整合到一个可穿戴传感器中，简化了糖尿病患者的日常管理。持续酮体监测是一个新兴研究领域，Abbott 等公司和多家初创企业也在开发类似的双传感器生物可穿戴设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar">FDA Authorizes First Wearable Device That Continuously Monitors Both Ketone Levels and Blood Sugar | FDA</a></li>
<li><a href="https://www.abbott.com/en-us/corpnewsroom/strategy-and-strength/abbotts-biowearable-one-sensor-for-glucose-ketones">Abbott's Biowearable: One Sensor for Glucose, Ketones | Newsroom</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8258504/">Continuous Ketone Monitoring : A New Paradigm for Physiologic...</a></li>

</ul>
</details>

**社区讨论**: 评论者们对自动化血糖控制和可及性的未来表示期待，同时也对无创传感的准确性以及酮体监测对普通糖尿病患者的实际有用性提出了怀疑。一位用户分享了朋友因糖尿病酮症酸中毒去世的个人故事，感叹这一进步的意义；另一些人则询问这项底层技术已存在多久。

**标签**: `#FDA`, `#wearable`, `#diabetes`, `#health tech`, `#medical devices`

---

<a id="item-5"></a>
## [苹果发布搭载 M5 Max 和 M5 Ultra 的全新 Mac Studio](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/) ⭐️ 8.0/10

苹果发布了搭载 M5 Max 和 M5 Ultra 芯片的全新 Mac Studio，强调了其本地 AI 能力和高内存带宽。新闻稿突出 M5 Ultra 最高可达 1.2 TB/s 的内存带宽，并将其定位为苹果迄今最强大的 Mac。 本次发布意义重大，因为它大幅提升了端侧 AI 性能，可能让用户更轻松地在本地运行大型语言模型，而不依赖云端。同时，它也引发了社区关于定价、内存容量以及该设备是否能满足未来更大模型需求的讨论。 M5 Ultra 由两颗 M5 Max 芯片通过片间互连结构连接而成，总内存带宽达到 1.2 TB/s（每颗芯片 614 GB/s）。内存配置最高可达 256GB，售价约 1 万美元，512GB 版本预计稍后推出；Thunderbolt 5 提供 120Gb/s 的外部 I/O 带宽。

hackernews · interpol_p · 8月25日 13:03 · [社区讨论](https://news.ycombinator.com/item?id=49433316)

**背景**: 本地 AI 是指在 Mac 等设备上直接运行人工智能模型，而不是将数据发送到云端服务器。内存带宽是指数据从内存中读取或存储到内存中的速率，对于大型模型而言是关键的瓶颈，因为权重和激活值需要快速移动。苹果的统一内存架构允许 CPU 和 GPU 共享同一内存池，这也是为什么带宽数字对评估 AI 性能至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Memory_bandwidth">Memory bandwidth</a></li>
<li><a href="https://localai.io/">LocalAI · Make AI run on every machine</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人称赞苹果押注本地 AI，并希望其能预装经过优化的前沿开放权重模型；另一些人则批评新闻稿中大量使用“最高达”的说法，以及高内存配置的高昂价格。技术型用户分析了带宽数据，估计 M5 Ultra 在运行 Deepseek V4 等模型时，预填充（prefill）速度可达每秒 1000+ token，生成速度可达每秒 50+ token，但对超过 1 万亿参数模型是否“未来可期”提出了质疑。

**标签**: `#Apple`, `#Mac Studio`, `#M5`, `#Local AI`, `#Hardware`

---

<a id="item-6"></a>
## [Nitter 收到停止函后关闭所有实例](https://github.com/zedeus/nitter/issues/1442) ⭐️ 8.0/10

Nitter 已收到停止函（cease and desist），导致所有公开实例在可预见的未来内下线，项目方正在等待法律建议。该公告发布在项目的 GitHub issue 页面上。 这一法律行动威胁到了一个广泛使用的隐私工具，该工具让用户无需广告、JavaScript 或跟踪即可阅读 X（Twitter）内容。同时，它也引发了对开源项目因违反服务条款而面临停止函威胁的脆弱性的担忧。 停止函的具体发送方尚未披露，项目法律团队目前正在评估应对方案。社区成员确认，包括 xcancel.com 在内的常用实例也已下线。

hackernews · Banditoz · 8月25日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=49437283)

**背景**: Nitter 是一个免费开源、用 Nim 编写的 Twitter/X 替代前端，所有请求通过其后端转发，从而提供无 JavaScript、无广告、无跟踪的快速轻量浏览体验。对于注重隐私的用户以及不想登录即可阅读推文的人来说，它是一个颇受欢迎的工具。该项目受 Invidious（一个类似的 YouTube 隐私前端）启发。此次法律行动可能为其他替代前端项目开创先例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nlnet.nl/project/Nitter/">NLnet; Nitter</a></li>
<li><a href="https://alternativeto.net/software/nitter/about/">Nitter : Free and open-source front-end mirror of Twitter... | AlternativeTo</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了失望和担忧，有人指出 X 仍被当地议会等组织用于发布官方信息，因此 Nitter 是重要的访问途径。其他人则思考了企业利用服务条款声明来关闭社区项目的更广泛趋势，还有人分享了其他平台（如 Hacker News）如何对待克隆项目的经验教训。

**标签**: `#Nitter`, `#Twitter`, `#Legal`, `#Open Source`, `#Privacy`

---

<a id="item-7"></a>
## [Firefox 157 默认启用 JPEG XL，覆盖所有平台](https://groups.google.com/a/mozilla.org/g/dev-platform/c/3YMV4MS34KA?pli=1) ⭐️ 8.0/10

Mozilla 宣布 Firefox 157 将在所有平台上默认启用 JPEG XL 支持。Chromium 也正在采用 JPEG XL，这标志着该图像格式在 Web 上的应用迈出了重要一步。 这意义重大，因为 Gecko 和 Blink 两大主流浏览器引擎都将默认支持 JPEG XL，使其有可能成为传统 JPEG 和 PNG 的实际替代品。这可能推动更高效的图像格式在网络上的广泛应用，并影响开发者和用户。 Firefox 和 Chromium 都使用基于 Rust 的 jxl-rs 库来支持 JPEG XL。苹果此前已在自家平台中使用了 libjxl（C++），但其未来计划尚不明朗，关于内存安全和性能对比也存在待解答的问题。

hackernews · yboris · 8月25日 17:55 · [社区讨论](https://news.ycombinator.com/item?id=49437946)

**背景**: JPEG XL 是一种由 JPEG 委员会、Google 和 Cloudinary 开发的现代图像格式，支持有损和无损压缩，效率优于 JPEG 和 PNG。它是由 ISO/IEC 18181 定义的自由开放标准，被设计为 JPEG 的长期继任者。浏览器支持进展缓慢；Firefox 此前仅在实验标志后面提供 JPEG XL，而 Chromium 曾一度移除了它。这一消息标志着该格式的采用重新获得动力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JPEG_XL">JPEG XL</a></li>
<li><a href="https://jpegxl.info/">JPEG XL : Superior Image Compression</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Firefox 和 Chromium 都依赖基于 Rust 的 jxl-rs 实现，并好奇苹果将如何处理其现有的 C++ libjxl 部署。还有人讨论了实际使用中的问题，例如将 JXL 图片上传到不支持的网站，以及是否支持 Windows 7/8 等旧操作系统。

**标签**: `#firefox`, `#jpeg-xl`, `#web standards`, `#browser`, `#image format`

---

<a id="item-8"></a>
## [SpaceX 正式公布路易斯安那州 Starbase LA 发射场，投资规模达千亿美元](https://www.spacex.com/sites/starbase-la) ⭐️ 8.0/10

2026 年 8 月 25 日，SpaceX 正式宣布将在路易斯安那州弗米利恩教区的佩肯岛湿地建造新的高密度发射场 Starbase LA。该场地将用于发射 Starship 火箭，运送 Starlink 卫星和轨道数据中心，据称投资规模达 1000 亿美元。 这标志着 SpaceX 的发射基础设施在得克萨斯州和佛罗里达州之外的重要扩展，可能为美国最贫困的沿海地区之一带来数十年的建设和航天就业机会。该场址的纬度还可能改善对太阳同步轨道的可达性，这对 Starlink 和轨道数据中心任务很有价值。 此次公告是在数月猜测之后发布的，当地房地产经纪人早在 5 月就曾提及该计划，Ars Technica 也在 8 月早些时候报道过相关传闻。社区成员指出，太阳同步轨道约 98 度的发射倾角是一项关键技术优势，同时也对 SpaceX 的时间表表示怀疑，并指出官方页面中存在几乎完全相同的段落，疑似由机器生成。

hackernews · bilsbie · 8月25日 16:37 · [社区讨论](https://news.ycombinator.com/item?id=49436822)

**背景**: 发射场纬度是轨道力学中的一个关键因素，因为它决定了火箭在不消耗额外燃料的情况下能达到的轨道倾角。靠近赤道的发射场可以利用地球自转为东向轨道获得额外速度，而较高纬度的场址通常更适合太阳同步轨道等高倾角轨道。SpaceX 已在得克萨斯州运营 Starbase 并拥有其他发射设施，Starship 的设计目标就是支持快速、高密度的重型货物发射。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.spacex.com/sites/starbase-la">SpaceX - Starbase , LA</a></li>
<li><a href="https://www.fox8live.com/2026/08/25/spacex-announces-plan-build-100-billion-starbase-louisiana-launch-facility/">SpaceX announces plan to build $100 billion ‘ Starbase Louisiana ...</a></li>
<li><a href="https://everydayastronaut.com/why-dont-they-just-launch-rockets-from-mountains-or-the-equator/">Why Don't They Just Launch Rockets From... | Everyday Astronaut</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对该地区的经济提振感到兴奋，有人预测路易斯安那沿海地区的焊工、混凝土工人和工匠将获得 10 到 20 年的稳定工作。也有人对美国境内雄心勃勃的实际工程项目表示谨慎乐观，但一些人怀疑马斯克的时间表，还有用户嘲讽官网文案逐字重复整句话，另有人指出埃隆此前曾否定火焰沟槽的设计。

**标签**: `#SpaceX`, `#aerospace`, `#engineering`, `#orbital mechanics`

---

<a id="item-9"></a>
## [在开放权重模型上持续学习实现前沿性能，助力主权 AI](https://www.reddit.com/r/MachineLearning/comments/1vxvzju/continual_learning_of_frontier_models_for/) ⭐️ 8.0/10

一份新的技术报告提出，各类机构可通过在现成开放权重模型上进行持续学习来实现前沿级 AI 性能。该报告发布了 Thomson，一个专注于法律、税务、安全和多语言等高风险专业工作的开放权重通用前沿模型。 这挑战了“只有少数资金雄厚的实验室才能构建前沿模型”的普遍假设，有望缩小 AI 开发者与用户之间在信息、经济和权力上的不对称。如果该方法得到验证，它可能使主权 AI——即独立构建、部署和治理 AI 的能力——对更多组织、政府和社区成为现实。 该持续学习方法引入了在每个训练阶段同时保持可塑性与稳定性的防护机制，并且只对参数进行极少量高影响干预。据报道，Thomson 展现出独特的π形能力提升模式：在广泛能力上获得提升的同时几乎完全消除了灾难性遗忘，并且所用计算资源和人员预算远低于常规前沿模型开发。

reddit · r/MachineLearning · /u/Forsaken_Scientist · 8月25日 10:30

**背景**: 持续学习，也称为终身学习，使机器学习模型能够随时间适应新数据，同时保留已学到的知识。开放权重模型公开训练好的神经网络权重，允许他人使用和微调，这与仅通过 API 提供的封闭模型不同。主权 AI 指国家、联邦或社区开发、部署或治理符合其法律、价值观和公共利益的 AI 系统的能力。这项工作将上述概念结合起来，为少数大公司之外的主体提出了拥有前沿 AI 能力的可行路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/continual-learning">What is Continual Learning? | IBM</a></li>
<li><a href="https://medium.com/lets-code-future/open-weight-ai-models-what-they-are-and-why-openais-next-move-matters-f86fe481973a">Open - Weight AI Models : What They Are , and Why... | Medium</a></li>
<li><a href="https://www.selfdriven.ai/research/sovereignity">Sovereignity - Research - selfdrivenAI — selfdrivenAI</a></li>

</ul>
</details>

**标签**: `#continual learning`, `#sovereign AI`, `#open-weight models`, `#frontier models`, `#AI governance`

---

<a id="item-10"></a>
## [SpaceX 计划将英伟达 Vera Rubin NVL72 送入轨道，测试太空 AI 计算](https://www.theregister.com/off-prem/2026/08/25/spacex-claims-it-will-put-a-vera-rubin-nvl72-rack-scale-system-into-orbit-next-year/5292067) ⭐️ 8.0/10

SpaceX 已宣布计划在 2027 年前将一套英伟达 Vera Rubin NVL72 机架级 AI 系统发射入轨，以测试太空环境下的 AI 计算。该公司尚未公布具体的发射日期、轨道高度以及供电和冷却方案。 这一举措可能标志着向轨道数据中心和天基 AI 基础设施迈出的重要一步，有望改变大规模计算的部署方式。不过，由于目前只是初步计划且缺乏技术细节，其可行性和影响仍有待验证。 Vera Rubin NVL72 将 72 颗 Rubin GPU 和 36 颗 Vera CPU 集成到一个液冷机架级系统中，功耗超过 100 千瓦。将其送入轨道需要解决发电、散热、辐射防护和通信等方面的挑战。

telegram · zaihuapd · 8月25日 08:03

**背景**: 机架级 AI 系统将 GPU、CPU、内存和网络集成到一个机箱中，可作为一个大型计算机进行管理，旨在高效运行大规模 AI 工作负载。英伟达的 Vera Rubin 平台是继 Hopper 和 Blackwell 之后的下一代架构，其中 NVL72 充当机架级超级计算机。轨道数据中心是一个未来概念，即将高性能计算基础设施部署在地球轨道上，可能提供无限太阳能和全球覆盖等优势，但该想法仍处于早期阶段且存在争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/rubin/">Infrastructure for Scalable AI Reasoning | NVIDIA Vera Rubin Platform</a></li>
<li><a href="https://win.ai/resources/blog/27-vera-rubin-nvl72-what-next-gen-training-infra-means">Vera Rubin NVL 72 cost and operational trade offs</a></li>
<li><a href="https://shaam.blog/articles/orbital-ai-data-centers-hype-vs-reality">Orbital AI Data Centers : Hype or the Future of Computing?</a></li>

</ul>
</details>

**标签**: `#Space computing`, `#AI hardware`, `#Nvidia`, `#SpaceX`, `#Orbital data center`

---

<a id="item-11"></a>
## [Qwen 预告 8 月 26 日开源 Qwen3.8-Flash-Next，基于 Qwen4 架构](https://www.modelscope.cn/models/Qwen/Qwen3.8-Flash-Next) ⭐️ 8.0/10

Qwen 在魔搭社区上线了 Qwen3.8-Flash-Next 的预告页，这是一款多模态 MoE 模型，预计于 2026 年 8 月 26 日 23:00（UTC+8）开放下载，提供标准版和 FP8 两个版本。官方表示该模型基于下一代 Qwen4 架构，提前开源是为社区迎接 Qwen4 系列做准备。 该事件意义重大，因为它首次公开预览了 Qwen4 架构，让开发者在完整版 Qwen4 发布前提前了解阿里巴巴下一代模型设计。开源 MoE 的开发路线也表明，在竞争激烈的 AI 生态中，团队仍将坚持以社区为中心的模型发展模式。 本次发布将包含标准版和 FP8 量化版两个版本，模型为多模态 MoE 架构。在 Hugging Face 上，该项目被描述为“Qwen 4 架构预览”，并列出了计划发布的模型文件 Qwen/Qwen3.8-Flash-Next。

telegram · zaihuapd · 8月25日 12:59

**背景**: 混合专家（MoE）是一种将模型拆分为多个专用子网络（即“专家”）、每次输入只激活其中一部分的架构，可提高效率并降低计算成本。FP8 是一种 8 位浮点格式，能降低内存占用并加速推理，通常只带来很小精度损失。Qwen3.8-Flash-Next 被定位为 Qwen4 的早期预览，让社区在完整版 Qwen4 系列发布前提前体验阿里巴巴下一代模型架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen/Qwen3.8-Flash-Next · Upcoming release · Hugging Face</a></li>
<li><a href="https://www.linkedin.com/pulse/mixture-experts-moearchitecture-padmashri-suresh-o5nqc">Mixture of Experts ( MoE ) architecture</a></li>
<li><a href="https://buttondown.com/justincormack/archive/ignore-previous-directions-6-floating-points/">Ignore previous directions 6: floating points • Buttondown</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#MoE`, `#AI`, `#open-source`, `#model-release`

---

<a id="item-12"></a>
## [特斯拉监督版 FSD 在中国正式可用](https://t.me/zaihuapd/43397) ⭐️ 8.0/10

2026 年 5 月 21 日，特斯拉通过 X 平台发文宣布，监督版全自动驾驶（FSD）现可在中国的使用。这标志着该系统正式进入全球最大的汽车市场之一。 该发布使特斯拉在全球竞争激烈的电动汽车和自动驾驶市场——包括比亚迪、华为等本土厂商全力推进高阶智驾功能——获得了战略立足点。同时，这也是对特斯拉纯视觉 FSD 在中国复杂路况及严格数据监管框架下实际表现的一次重要考验。 报道称，特斯拉此前已对国内 24 款车型开放过 FSD V13 的小范围测试，参与的测试车主约 5000 人。特斯拉上海数据中心已实现境内数据全留存，位于临港的 AI 训练中心已于 2026 年 2 月投入运营，并与百度地图合作使用合规高精地图。

telegram · zaihuapd · 8月25日 13:42

**背景**: 全自动驾驶（监督版）是特斯拉最先进的消费者辅助驾驶产品，可在驾驶员主动监督下完成导航、转向、变道和泊车等操作，并非完全自动驾驶。在中国，自动驾驶功能受到严格监管，包括数据本地化和地图资质要求，特斯拉通过上海数据中心、本地 AI 训练中心以及与百度地图的合作来满足这些合规要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://post.smzdm.com/p/a825z5e7/">中国被 特 斯 拉 移出 FSD ...</a></li>
<li><a href="https://www.ithome.com/0/992/918.htm">特 斯 拉 官网更新： 监 督 版 FSD 支持地区不再包含中国 - IT之家</a></li>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving ( Supervised ) | Tesla</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#FSD`, `#autonomous driving`, `#AI`, `#China`

---

<a id="item-13"></a>
## [Anthropic 第二季营收超 115 亿美元，同比增长逾 14 倍](https://t.me/zaihuapd/43403) ⭐️ 8.0/10

据彭博社援引文件报道，Anthropic 第二季初步营收超过 115 亿美元，同比增长逾 14 倍。当季调整后营业利润也实现转正。 这标志着这家领先 AI 实验室在商业化上取得重大里程碑，显示其 AI 模型的变现速度极快。随着可能在今秋启动大型 IPO，这些业绩很可能深刻影响 AI 行业的投资格局。 初步数据仍可能调整；相比之下，去年同期营收为 7.87 亿美元，2026 年第一季为 47.3 亿美元。据报道，Anthropic 正筹备可能在今秋启动的大型 IPO。

telegram · zaihuapd · 8月25日 17:32

**背景**: Anthropic 是一家由前 OpenAI 研究人员创立的 AI 安全与研究公司，以 Claude 系列大语言模型闻名。营收高速增长表明企业对其 AI 产品的需求不断上升；若启动 IPO，将为公开市场投资者提供一个重要的纯 AI 投资标的。

**标签**: `#Anthropic`, `#AI`, `#IPO`, `#revenue`, `#business`

---