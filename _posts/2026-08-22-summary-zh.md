---
layout: default
title: "Horizon Summary: 2026-08-22 (ZH)"
date: 2026-08-22
lang: zh
---

> 从 29 条内容中筛选出 6 条重要资讯。

---

1. [为训练游戏代理打造的开源 Roguelike 环境 DelveRL](#item-1) ⭐️ 8.0/10
2. [评估分辨率改变哪种学习规则在 V1 中最像大脑](#item-2) ⭐️ 8.0/10
3. [任天堂单日下架 400 余个 Switch 模拟器仓库，suyu 占 311 个](#item-3) ⭐️ 8.0/10
4. [特斯拉宣布监督版 FSD 在中国可用](#item-4) ⭐️ 8.0/10
5. [SemiAnalysis：开源模型每一代追平时间减半](#item-5) ⭐️ 8.0/10
6. [亚马逊被曝购买并销毁纸质书以训练 AI](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [为训练游戏代理打造的开源 Roguelike 环境 DelveRL](https://www.reddit.com/r/MachineLearning/comments/1vvii1j/i_built_an_opensource_roguelike_specifically_for/) ⭐️ 8.0/10

开发者发布了 DelveRL，这是一个专为强化学习设计的开源回合制 Roguelike 环境，具备确定性模拟、程序化关卡、部分可观测性以及无渲染器的批量环境。其中包含一个循环 PPO 基线，中位可到达 18 层，延长运行可达 33 层。 DelveRL 通过提供一个具有结构化 API、易于与代理框架集成的人类可玩游戏，解决了 RL 研究中的一个现实空白，这与许多现有游戏不同。这可能使 Roguelike 环境更容易用于测试代理的探索、风险管理和长程规划能力。 该环境完全本地运行，具有为可复现性而设的确定性模拟，并提供程序化关卡、部分可观测性和策略深度。项目包含游戏代码、训练代码、检查点、桥接文档和原始基准，全部开源。

reddit · r/MachineLearning · /u/SnyderConsulting · 8月22日 17:32

**背景**: 强化学习（RL）是让代理通过与环境的交互并根据奖励来学习决策。像 Roguelike 这样的游戏提供了丰富的、部分可观测的、程序化生成的场景，非常适合测试 RL 算法，但许多现有游戏难以与代理框架集成。循环 PPO 是近端策略优化算法的扩展，使用 LSTM 网络来处理部分可观测性和记忆问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/SnyderConsulting/DelveRL/tree/main/docs">DelveRL/docs at main · SnyderConsulting/DelveRL · GitHub</a></li>
<li><a href="https://sb3-contrib.readthedocs.io/en/master/modules/ppo_recurrent.html">Recurrent PPO — Stable Baselines3 - Contrib 2.9.0 documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning">Reinforcement learning - Wikipedia</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#RL environment`, `#roguelike`, `#open-source`, `#game agents`

---

<a id="item-2"></a>
## [评估分辨率改变哪种学习规则在 V1 中最像大脑](https://www.reddit.com/r/MachineLearning/comments/1vvdxwt/the_evaluation_resolution_has_been_shown_to_have/) ⭐️ 8.0/10

这项研究表明，评估 CNN 表征时的分辨率会显著影响哪种学习规则在 V1 上显得最像大脑。那种“未训练 CNN 与训练 CNN 在 V1 上一样好”的常见发现在高分辨率下消失，训练模型明显优于未训练模型。 这一发现很重要，因为使用 RSA 进行的模型-大脑比较在计算神经科学中广泛使用，而评估分辨率在很大程度上被忽略为一种混淆变量。它挑战了此前关于未训练 CNN 与训练 CNN 一样类脑的说法，这可能改变研究人员解读此类比较的方式。 该研究使用了一个在 CIFAR-10 子集上以 32 像素训练的小型 CNN，并在六种分辨率(32 至 224 像素)下对 THINGS-fMRI 刺激进行评估，同时保持权重和归一化不变。研究比较了五种学习规则，并排除了若干混杂因素，如批归一化校准不当和低层像素结构；在侧枕复合体(LOC)上反向传播的优势在所有分辨率下均存在。

reddit · r/MachineLearning · /u/ConfusionSpiritual19 · 8月22日 14:30

**背景**: 表征相似性分析(RSA)是一种通过关联模型与大脑的成对相似性矩阵来比较它们如何表征刺激的技术。V1 是视觉处理的第一个皮层区域，CNN 常被用作生物视觉的模型。反向传播、反馈对齐和脉冲时序依赖可塑性(STDP)等学习规则定义了网络在训练过程中如何更新权重。此前研究表明随机未训练的 CNN 可以在 V1 上与训练过的 CNN 相媲美，而本研究表明这一结论依赖于评估分辨率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/systems-neuroscience/articles/10.3389/neuro.06.004.2008/full">Frontiers | Representational similarity analysis - connecting the...</a></li>
<li><a href="https://towardsdatascience.com/feedback-alignment-methods-7e6c41446e36/">Feedback Alignment Methods | Towards Data Science</a></li>
<li><a href="https://homo-deus.com/lab/neuromorphic-computing/stdp-learning/">STDP Simulator: Spike - Timing - Dependent Plasticity Learning Rule</a></li>

</ul>
</details>

**标签**: `#computational neuroscience`, `#CNN`, `#learning rules`, `#model-brain comparison`, `#evaluation resolution`

---

<a id="item-3"></a>
## [任天堂单日下架 400 余个 Switch 模拟器仓库，suyu 占 311 个](https://torrentfreak.com/nintendo-wipes-out-400-switch-emulator-repos-in-single-day-github-sweep/) ⭐️ 8.0/10

任天堂在同一天向 GitHub 提交了 7 份 DMCA 反规避通知，导致 400 多个 Switch 模拟器仓库被下架，其中包括 suyu 的 311 个分支和 Skyline 的 29 个仓库。通知称这些模拟器使用未经授权的密钥解密游戏。 这是针对开源模拟器项目规模最大的 DMCA 执法行动之一，影响了数百个仓库，并可能对未来的 Switch 模拟开发产生寒蝉效应。它也凸显了模拟、反规避法律与开源软件分发之间长期存在的法律张力。 这些 DMCA 通知属于第 1201 条的反规避主张，针对的是使用解密密钥的行为，而非直接侵犯版权。Yuzu 和 Suyu 两案均以和解方式了结，未经法院最终裁定，因此法律先例仍未确定。

telegram · zaihuapd · 8月22日 00:28

**背景**: Yuzu、Suyu 和 Skyline 等 Switch 模拟器通过模拟主机硬件并使用从实体主机获取的解密密钥，让用户能在 PC 或 Android 设备上运行 Switch 游戏。2024 年 3 月，Yuzu 与任天堂达成 240 万美元和解并停止运营；Suyu 是 Yuzu 的社区分支，而 Skyline 是一款面向 Android 的模拟器，已于 2023 年停止开发。DMCA 第 1201 条禁止规避技术保护措施，这正是任天堂下架请求的法律依据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yuzu_(emulator)">Yuzu (emulator) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Skyline_(emulator)">Skyline (emulator)</a></li>

</ul>
</details>

**标签**: `#Nintendo`, `#DMCA`, `#Emulation`, `#GitHub`, `#Legal`

---

<a id="item-4"></a>
## [特斯拉宣布监督版 FSD 在中国可用](https://t.me/zaihuapd/43321) ⭐️ 8.0/10

特斯拉今天上午在社交媒体 X 发帖，宣布其监督版全自动驾驶（FSD）功能已可在中国的车辆上使用。这是特斯拉 FSD 在中国市场的重要一步，但官方没有公布具体的上线日期或更多细节。 这是一座重要的监管与市场里程碑，因为中国是全球最大的汽车市场之一，也是自动驾驶竞争最激烈的地区之一。这可能会给比亚迪、华为系品牌和小鹏等本土对手带来压力，推动它们加快自身辅助驾驶技术的落地。 特斯拉的 FSD（监督版）仍是一个 L2 级驾驶辅助系统，依然需要驾驶者手握方向盘并保持专注，官方也明确指出它并不会让车辆完全自动驾驶。特斯拉称 FSD（监督版）可将重大和轻微碰撞减少 7 倍、公路外碰撞减少 5 倍，但这些数据均以驾驶者主动监督为前提。

telegram · zaihuapd · 8月22日 01:56

**背景**: FSD（监督版）是特斯拉提供的可选 L2 级先进驾驶辅助系统，按 SAE International 的定义属于部分自动驾驶，2019 年 4 月后生产的特斯拉汽车基本都配备 Autopilot，并可选订阅 FSD（监督版）。它提供自动转向、交通感知巡航控制和道路导航等功能，但与完全自动驾驶不同，它要求驾驶员时刻保持监督。此次进入中国，是这一系统在重大海外市场的又一次拓展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot">Tesla Autopilot - Wikipedia</a></li>
<li><a href="https://www.tesla.com/support/fsd">Full Self-Driving (Supervised) | Tesla Support</a></li>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving (Supervised) | Tesla</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#FSD`, `#Autonomous Driving`, `#China`, `#AI`

---

<a id="item-5"></a>
## [SemiAnalysis：开源模型每一代追平时间减半](https://newsletter.semianalysis.com/p/are-open-models-catching-up) ⭐️ 8.0/10

SemiAnalysis 最新分析发现，开源模型正以每一代更快的速度缩小与闭源前沿模型的能力差距。在智能体时代，Kimi K2.6 用了 4.8 个月超越 Opus 4.5，GLM-5.2 用了 6 个月超过 GPT-5.2。 这引发了模型层商品化的担忧，因为 GLM 5.3、Kimi K3 等开源模型如今已能胜任许多曾助 Anthropic 实现 650 亿美元以上年化收入的编程与智能体任务。这表明纯模型能力可能不再是一个重要的差异化因素，价值重心将转向产品化与分发渠道。 该分析将大模型历史分为早期扩展、推理和智能体三个时代，并发现每个时代的追平时间都在减半。不过文章也提醒，基准测试并非全部，Anthropic 的产品化能力仍然是其重要优势。

telegram · zaihuapd · 8月22日 08:26

**背景**: SemiAnalysis 是一家专注于半导体和人工智能的独立研究机构，以机构级行业分析著称。AI 行业越来越关注开源模型是否会使得模型层商品化，相关讨论涉及生成式 AI 的商品化趋势以及向智能体工作流的转变。所谓“智能体时代”指 AI 从“会聊天”进化为“能干活”的阶段，开源模型正是在这一领域快速逼近闭源前沿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://startedbywomen.com/companies/semianalysis">SemiAnalysis | Started by Women</a></li>
<li><a href="https://baike.baidu.com/item/智能体时代/68091644">智能体时代（人工智能代理时代）_百度百科</a></li>
<li><a href="https://www.jxxy.net/ai/articles/aiwhisperx-coding-agent-24b-arr/">写在Coding Agent 240亿时刻：大模型进入挤兑阶段｜觉醒AI</a></li>

</ul>
</details>

**标签**: `#open-source`, `#AI models`, `#industry analysis`, `#SemiAnalysis`, `#agent era`

---

<a id="item-6"></a>
## [亚马逊被曝购买并销毁纸质书以训练 AI](https://t.me/zaihuapd/43331) ⭐️ 8.0/10

404 Media 的调查显示，亚马逊一直在购买纸质书、扫描书籍内容用于训练 AI 模型，随后销毁原书。调查人员追踪一本稀有书至拉斯维加斯的亚马逊仓库，仓库员工称他们会剪掉装订以加快扫描，之后将书页丢弃。 这一做法引发了关于版权侵犯和销毁文化资产的严重伦理与法律问题。它揭示了科技公司为 AI 训练大量获取印刷作品的行业新趋势，并可能影响作者、出版商以及稀有或绝版书籍的保存。 调查人员在稀有书中放置了追踪装置，最终追踪到内华达州拉斯维加斯的亚马逊仓库。仓库员工表示，他们会接收大量印刷书籍，剪掉装订以加快扫描速度，书页随后被销毁。

telegram · zaihuapd · 8月22日 15:40

**背景**: AI 公司需要大量文本来训练大型语言模型，而书籍被视为高质量的数据来源。此前 Anthropic 也被曝出类似做法。图书作者和出版商越来越反对这种未经授权使用其作品的行为，而销毁原书进一步加剧了人们对不可替代纸质资料流失的担忧。

**标签**: `#AI training`, `#Amazon`, `#copyright`, `#data ethics`, `#investigative report`

---