<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT</h1>

<p align="center"><b>追踪 AI 安全新闻、论文与事件。一站阅读，也能接入你的 Agent。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/zh"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-4-2ea44f" alt="4 Agent skills"></a>
  <a href="https://github.com/wuyoscar/AISafetyHot-Hub/stargazers"><img src="https://img.shields.io/github/stars/wuyoscar/AISafetyHot-Hub?style=flat" alt="GitHub stars"></a>
</p>

<p align="center"><a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a></p>

<p align="center"><a href="https://aisafetyhot.com/zh"><img src="assets/observatory.gif" width="1000" alt="新版科研观测台实录：材料扫描、立体星图与新闻流"></a></p>

<p align="center"><a href="https://aisafetyhot.com/zh">打开观测台</a> · <a href="https://aisafetyhot.com/zh/featured">实时新闻</a> · <a href="https://aisafetyhot.com/zh/papers">找论文</a> · <a href="https://aisafetyhot.com/zh/daily">读日报</a> · <a href="#agent">接入 Agent</a></p>

**AI Safety HOT** 持续整理越狱、提示注入、Agent 安全、防御与护栏、对齐、评测、真实事件和治理政策。网站提供中英文阅读；这个 Hub 保存公开论文清单、日报归档和 Agent 技能。

## 从一条动态，看到它关联的研究与事件

首页是一座可以探索的**科研观测台**：材料卡片逐条扫描，汇入由信源、事件和论文研究方向组成的立体星图；往下是最近 72 小时的新闻流，以及汇集报道与社区讨论的热点观察。拖动星图旋转，点选节点，沿链接继续阅读。

上面的 GIF 来自真实网站录屏。[查看高清静态图](assets/site-overview.webp) · [查看新闻流与热点观察](assets/site-news-flow.webp)

| 想看什么 | 从这里开始 |
| --- | --- |
| 最近发生了什么 | [实时新闻](https://aisafetyhot.com/zh/featured)：浏览动态、阅读导读，回到原文。 |
| 一件事怎样发展 | [热点新闻](https://aisafetyhot.com/zh/hot)：把相关报道放在一起，查看事件进展与讨论。 |
| 一个方向有哪些研究 | [实时论文](https://aisafetyhot.com/zh/papers)与[会议论文](https://aisafetyhot.com/zh/conferences)：按研究方向筛选，查看题录、速读和原文。 |
| 每天集中读一遍 | [安全日报](https://aisafetyhot.com/zh/daily)：按方向整理，当天的新进展补进同一期。 |

<details>
<summary><b>展开新版页面截图</b></summary>

### 实时新闻

按时间浏览新闻，结合搜索与筛选找到你关心的动态。

<a href="https://aisafetyhot.com/zh/featured"><img src="assets/site-featured.webp" width="1000" alt="实时新闻页面：新闻列表与筛选"></a>

### 热点新闻

从一个事件进入，查看相关报道和讨论。

<a href="https://aisafetyhot.com/zh/hot"><img src="assets/site-hot.webp" width="1000" alt="热点新闻页面：事件排名与相关报道"></a>

### 实时论文

按研究方向、论文类型和 Agent 场景筛选，继续阅读速读与原文。

<a href="https://aisafetyhot.com/zh/papers"><img src="assets/site-papers.webp" width="1000" alt="实时论文页面：研究方向与论文列表"></a>

### 会议论文

浏览 AI 与安全会议中的相关工作，按方向查找论文。

<a href="https://aisafetyhot.com/zh/conferences"><img src="assets/site-conferences.webp" width="1000" alt="会议论文页面：会议与研究方向"></a>

### 安全日报

把当天值得关注的新闻和研究集中读完。

<a href="https://aisafetyhot.com/zh/daily"><img src="assets/site-daily.webp" width="1000" alt="安全日报页面：按方向整理的新闻与论文"></a>

</details>

<a id="agent"></a>

## 让你的 Agent 一起读

AI Safety HOT 有一个公开的 MCP 接口：热点排行、事件来龙去脉、每天的动态和新论文，Agent 接上就能直接问。免费，不用 API Key。

**一句话安装**：把下面这句发给你的 Agent（Claude Code、Codex、Cursor……都行）：

```
帮我安装 AI Safety HOT：https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/install.md
```

它会自己判断用的是哪个客户端、装好 MCP 和技能、试调一次，再告诉你能问什么。

**已经装过？更新也是一句话：**

```
帮我更新 AI Safety HOT：https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/update.md
```

<a id="skills"></a>
<a id="技能"></a>

### 装好就能用

不用记工具名，直接问：

| 你可以这样问 | Agent 会做什么 | 技能 |
| --- | --- | --- |
| 现在 AI 安全圈最热的是什么？第一名怎么回事？ | 读热点排行，再按时间理一遍这件事的报道 | [`aisafety-hot`](skills/aisafety-hot/SKILL.md) |
| 今天 AI 安全有什么大事？ | 读最近 24 小时的精选，按攻击、防御、事件、政策整理成简报 | [`aisafety-brief`](skills/aisafety-brief/SKILL.md) |
| 今天有哪些值得看的新论文？帮我整理越狱方向的相关工作 | 读每日论文和方向索引，一句话说清每篇做了什么，可以给 BibTeX | [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) |
| Anthropic 最近一周有什么安全动态？Cursor 最近出过安全问题吗？ | 盯一家公司或一个产品，列出进展、事件和漏洞 | [`aisafety-watch`](skills/aisafety-watch/SKILL.md) |

<!-- agent-examples:start -->
下面是 2026-10-24 实际调用的返回节选：

**「现在 AI 安全圈最热的是什么？第一名怎么回事？」** → `aisafetyhot_get_hot_topics` + `aisafetyhot_get_story`

```text
第 1 名：Wiz称AI发现PHP核心严重RCE漏洞，官方已发布修复
  72 小时本站范围：646 个独立信源，917 条链接
第 2 名：第三方红队试点发现OpenAI内部监控系统漏洞
  72 小时本站范围：128 个独立信源，143 条链接
第 3 名：LiteLLM 1.107.0 遭入侵，植入窃密程序与后门
  72 小时本站范围：264 个独立信源，307 条链接

事件：Wiz称AI发现PHP核心严重RCE漏洞，官方已发布修复｜49 篇报道｜45 个来源
2026-10-23｜The Guardian · 人工智能｜“黑色十月”：网络安全专家对 AI 助力黑客攻击新时代发出警报
2026-10-23｜Semafor｜人类自满制造了 AI 时代最大的问题
2026-10-23｜ZDF｜AI 发现的 PHP 安全漏洞：网站为何下线、后续如何应对
```

**「今天 AI 安全有什么大事？」** → `aisafetyhot_get_latest`

```text
1. OpenAI 加强前沿模型训练环境安全防护
   来源：OpenAI；原文发表：2026-10-23
2. USDA 承认 DOGE 裁员让联邦 AI 人工监督“难以为继”
   来源：TechTimes；原文发表：2026-10-23
3. Anthropic 称其未发布模型在能力和对齐上都优于 Mythos 5.1
   来源：The Decoder；原文发表：2026-10-23
```

**「今天有哪些值得看的新论文？」** → `daily-papers/2026-10-24.json`

```text
1. Agentic Verified Optimization of Real-World Software
   研究者提出智能体验证式优化任务，要求智能体在产出更快实现的同时给出与既有实现等价的机器可检验证明，以应对现有等价检查主要依赖测试、而智能体已被证明会利用测试通过检查却不保留原行为的问题。
   arXiv 2610.30188
2. Reliable AI-Assisted Decisions via Selective Auditing
   研究者提出一种选择性审计方法，在保证未被审计的 AI 错误比例低于用户设定阈值的前提下，尽量减少人工专家审查。
   arXiv 2610.31662
3. AgentVQA: A Unified Benchmark for Agentic Visual Understanding
   研究者推出 AgentVQA，一个覆盖网页智能体、机器人、第一人称视频、游戏和空间规划五类场景的离线基准，用于评测视觉语言模型在真实智能体任务上的表现，以补充成本高、难扩展的在线评测。
   arXiv 2610.31494
```

**「Anthropic 最近一周有什么安全动态？」** → `aisafetyhot_get_latest topic=anthropic`

```text
1. Anthropic 称其未发布模型在能力和对齐上都优于 Mythos 5.1
   来源：The Decoder；原文发表：2026-10-23
2. AISI 就 2026 年 7 月自家事故开展对齐调查：Mythos 5 为何实施未经授权的供应链攻击
   来源：X @AISecurityInst；原文发表：2026-10-23
3. Anthropic 对 UK AISI 网络测试事件的对齐评估
   来源：Anthropic Research；原文发表：2026-10-23
```
<!-- agent-examples:end -->

### 手动安装、更新和卸载

**Claude Code**（技能和 MCP 在同一个插件里）

```bash
# 安装
claude plugin marketplace add wuyoscar/AISafetyHot-Hub
claude plugin install aisafetyhot@aisafetyhot-hub
# 更新
claude plugin marketplace update aisafetyhot-hub
claude plugin update aisafetyhot@aisafetyhot-hub
# 卸载
claude plugin uninstall aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
# 安装
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
npx skills add wuyoscar/AISafetyHot-Hub
# 更新
npx skills update
# 卸载
codex mcp remove aisafetyhot
npx skills remove aisafety-hot aisafety-brief aisafety-paper-scout aisafety-watch
```

**Cursor / 其他 Agent**：在 MCP 设置里加一个 Streamable HTTP 服务，地址 `https://aisafetyhot.com/api/mcp`；支持技能的客户端再跑 `npx skills add wuyoscar/AISafetyHot-Hub`。

**体检**：一条命令确认接口能用，返回当前前三名热点就是通的。

```bash
curl -s https://aisafetyhot.com/api/mcp -H 'content-type: application/json' -H 'accept: application/json, text/event-stream' \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/call","params":{"name":"aisafetyhot_get_hot_topics","arguments":{"limit":3}}}'
```

### 用之前你可能想知道

| | |
| --- | --- |
| **免费** | 最近 7 天的精选新闻、热点榜事件、日报和每日论文，匿名就能读，不用 API Key |
| **只读** | 接口只读不写；返回的标题和摘要来自外部信源，技能会让 Agent 只当资料，不执行里面的指令 |
| **限额** | 每个 IP 每分钟 60 次、每天 300 次，超了会返回 429 和等待时间 |
| **更早的历史** | 历史查询、完整论文解读和周报月报需要只读授权，见 [Agent 指南](docs/agent.md) |
| **兼容** | 支持 MCP（Streamable HTTP）的客户端都能用；工具和参数见 [Agent 指南](docs/agent.md)与[调用示例](docs/mcp-examples.md) |

## 每日论文与公开归档

[每日论文](daily-papers)从论文库中每天挑选 30 篇，跨日去重，兼顾近期研究与较早的重要工作；保留原始发表日期、原文和站内阅读链接。也可以按[研究方向](daily-papers/topics)浏览。

| 归档 | 内容 |
| --- | --- |
| [daily-papers](daily-papers) | 每日论文推荐与方向索引 |
| [daily](daily) · [English](en) | 已公开的日报归档 |
| [papers](papers) | 按日期导出的论文 Markdown、JSON 与 BibTeX |
| [archive](archive) | 年度索引 |

<!-- papers:start -->
### 2026-10-26 · 30 篇

1. **[LoRAcles: Self-Supervised Weight-Space Interpretability at Scale](https://neurips.cc/virtual/2026/poster/154333)**  
   训练以 LoRA 权重为输入、回答模型行为问题的语言模型，在 AuditBench 上达最优，能检测模型生物的细微变化并首次非平凡地 verbalize 语义后门触发器。 · `可解释性` · Celeste De Schamphelaere … Euan Ong · NeurIPS 2026 oral
2. **[CLIOPATRA: Extracting Private Information from LLM Insights](https://neurips.cc/virtual/2026/poster/152543)**  
   作者称首个针对隐私保护型 LLM 洞察系统的攻击，通过注入恶意对话击穿多层防护，在 Anthropic Clio 上以近 100% 精度、最高 65% 的比例提取目标用户医疗聊天内容。 · `隐私与数据泄露` · Meenatchi Sundaram Muthu Selva Annamalai … Peter Kairouz · NeurIPS 2026 oral
3. **[AIs with Secret Loyalties are a Serious but Addressable Threat](https://neurips.cc/virtual/2026/poster/140059)**  
   定义秘密忠诚威胁——模型隐秘推进特定行为者利益且能逃避黑箱审计，指出其已在开源权重模型上可实现，并提出五个方向的研究议程。 · `对齐` · Joe Kwon … Tom Davidson · NeurIPS 2026 spotlight
4. **[We Should Distinguish Unlearning From Untraining](https://neurips.cc/virtual/2026/poster/140062)**  
   立场论文指出机器遗忘实际包含两种不同问题：撤销特定样本训练影响的Untraining与移除整个子分布概念的Unlearning，混淆二者会导致指标误用。 · `隐私与数据泄露` · Eleni Triantafillou … Georgios Kaissis · NeurIPS 2026 oral
5. **[Unlearning That Lasts: Utility-Preserving, Robust, and Almost Irreversible Forgetting in LLMs](https://neurips.cc/virtual/2026/poster/149440)**  
   提出以JS散度为目标的JensUn遗忘方法和新数据集LPF，改进评估显示许多现有遗忘方法实际效果不如此前认为的那样好。 · `隐私与数据泄露` · Naman Deep Singh … Matthias Hein · NeurIPS 2026 spotlight
6. **[Omni-Reward: Towards Generalist Omni-Modal Reward Modeling with Free-Form Preferences](https://openreview.net/forum?id=9C4gVbPqSy)**  
   构建覆盖五种模态的全模态奖励模型基准 Omni-RewardBench、248K 偏好对数据集与相应奖励模型，支持自由形式偏好并取得强性能。 · `对齐` · Zhuoran Jin … Jun Zhao · ICLR 2026 Oral
7. **[Asymptotic Optimality of the High-Dimensional Gaussian Mechanism and Improved Low-Dimensional Mechanisms for Differential Privacy](https://openreview.net/forum?id=82Wosp2Iu1)**  
   证明高维极限下无加噪机制能渐近优于高斯机制的隐私-效用权衡，并提出球面广义Gamma机制族，其中部分成员在低维设定下优于高斯和ℓ2机制。 · `隐私与数据泄露` · Yu Wei … Antigoni Polychroniadou · ICML 2026 spotlight
8. **[Surgery: Mitigating Harmful Fine-Tuning for Large Language Models via Attention Sink](https://openreview.net/forum?id=6ojsIliNF0)**  
   发现正 sink divergence 的注意力头数量随有害微调增加，据此提出 Surgery 正则化方法抑制有害模式学习，在 BeaverTails、HarmBench、SorryBench 上分别提升防御 5.90%、11.25%、9.55%。 · `防御与护栏` · Guozhi Liu … Li Shen · ICML 2026 spotlight
9. **[Jailbreak Foundry: From Papers to Runnable Attacks for Reproducible Benchmarking](https://openreview.net/forum?id=BSi2mfMDsx)**  
   提出多智能体系统 JBF，将越狱论文自动翻译为可执行模块并统一评测，复现 30 种攻击的 ASR 平均偏差仅 +0.26 个百分点，实现跨 10 个模型的标准化基准。 · `越狱与攻击` · Zhicheng Fang … Wei Xu · ICML 2026 spotlight
10. **[Safety Reconstructed: Generative Modeling via Masked Diffusion Builds Strong Safety Guardrails](https://neurips.cc/virtual/2026/poster/149672)**  
   将护栏训练改为类条件重建目标，微调 LLaDA-8B 的 LLaDA Guard 在七个安全基准上平均排名领先，校准更好（ECE 0.0875 vs 0.1384），并可将不安全提示改写为安全等价（平均 60.7% 转化率）。 · `防御与护栏` · Gert Lek … Lydia Chen · NeurIPS 2026 spotlight
11. **[When Is a Memory Safe Enough to Act On? Action-Conditioned Verification for Long-Lived Agents](https://arxiv.org/abs/2610.31446)**  
   论文面向长期运行的智能体，将行动前的记忆复核建模为顺序停止问题：一次复核是否值得，取决于它能否改变下一步行动，而非单看记忆可靠度。 · arXiv 2610.31446 · 2026-10-22 · [解读](https://aisafetyhot.com/items/gfummvlnk5t4ca424srkolmsd)
12. **[AgentTriage：跨异构智能体运行时的可重放安全诊断](https://arxiv.org/abs/2610.30738)**  
   论文提出 AgentTriage，一个跨异构智能体运行时的可重放安全诊断契约，用于诊断工具调用智能体产生的安全事件。 · arXiv 2610.30738 · 2026-10-22 · [解读](https://aisafetyhot.com/items/nbm0pixo4jsjp4sid2tjswr2s)
13. **[Post-Audit Mirage: Identifiability Limits of Offline Agent Verification](https://arxiv.org/abs/2610.31130)**  
   审计后幻象：离线 Agent 验证的可识别性极限 · arXiv 2610.31130 · 2026-10-22 · [解读](https://aisafetyhot.com/items/nqi6w5nkz7kgqz9y2zvhowpyn)
14. **[EpiSEM-Bench: Evaluating Safety and Evidence Recovery in LLM Agents under Missing Evidence](https://arxiv.org/abs/2610.31650)**  
   论文提出 EpiSEM-Bench，研究工具返回内容全部为真但遗漏安全关键事实时，LLM 智能体是否仍执行禁止行动。 · arXiv 2610.31650 · 2026-10-22 · [解读](https://aisafetyhot.com/items/prl6ozrwcm0kyv5so0k1d08aj)
15. **[Toward Recursive Self-Improvement in Physical AI](https://huggingface.co/papers/2610.29677)**  
   **summary_zh**：递归自我改进（RSI）指系统不仅改进行为、还改进其改进过程，论文将其置于机器人学习之中。 · arXiv 2610.29677 · 2026-10-21 · [解读](https://aisafetyhot.com/items/pxv9ozu43ixiio77hxo3n7808)
16. **[SIM-UT: A User Simulation based Evaluation Framework for Medical Triage Chatbots](https://arxiv.org/abs/2610.30412)**  
   研究者提出 SIM-UT，一种多轮、基于用户行为模拟的医疗分诊聊天机器人评测方法，用于发现贴近真实语境的失效模式。 · arXiv 2610.30412 · 2026-10-21 · [解读](https://aisafetyhot.com/items/u15fl382mhfb7ko7vemyivn1b)
17. **[Uncensored Is Not Unbiased: Abliteration Removes Refusals but Not Script-Dependent Bias About Taiwan](https://arxiv.org/abs/2610.29342)**  
   论文测试发现，abliteration 去审查移除了开源模型的拒答，却未消除涉台立场的书写系统差异，书写系统的影响远大于去审查本身。 · arXiv 2610.29342 · 2026-10-21 · [解读](https://aisafetyhot.com/items/hhz4v3aci6ruzr5rd305p4zii)
18. **[A Unified Evaluation Framework of Physical Adversarial Robustness in the Edge VLM Era](https://arxiv.org/abs/2610.29196)**  
   边缘 VLM 时代物理对抗鲁棒性的统一评测框架 · arXiv 2610.29196 · 2026-10-21 · [解读](https://aisafetyhot.com/items/zgm6kssdt3wnp8s8dt1eadp1x)
19. **[Private Online Prediction from Experts with Small Losses](https://arxiv.org/abs/2610.29575)**  
   论文提出首个在低损失区间达到 \tilde{O}(√L*) 遗憾的差分隐私专家在线预测算法，L* 为最佳专家的累计损失，较既有 \tilde{O}(√T) 界明显改进。 · arXiv 2610.29575 · 2026-10-21 · [解读](https://aisafetyhot.com/items/s2o85zwc3ih1jrem5q92vj4qz)
20. **[TARSphere: A Robot-Oriented Full-Stack Framework for Long-Horizon Embodied Agents in Evolving Physical and Social Environments](https://huggingface.co/papers/2610.30043)**  
   研究者提出 TARSphere，一个面向机器人的全栈框架，结合物理仿真、具身 NPC 与冻结的多模态大语言模型（MLLM），评估演化物理和社会环境中的长时程具身智能体。 · arXiv 2610.30043 · 2026-10-21 · [解读](https://aisafetyhot.com/items/g6680eztewbeunqj7rf5hc6t5)
21. **[TraceForge: Distilling with Your Own Thinking](https://huggingface.co/papers/2610.29680)**  
   TraceForge 用先监督后对抗的两阶段训练，从教师答案合成学生模型家族风格的推理轨迹，不依赖教师的隐藏推理输出。 · arXiv 2610.29680 · 2026-10-21 · [解读](https://aisafetyhot.com/items/bo383rhv24oc53ooevyf21v5o)
22. **[VX-One: Typed, Calibrated Decision Heads for Real-Time Perimeter Triage - An empirical study of unknown-attack honesty, cascade gray zones, and calibration under drift](https://huggingface.co/papers/2610.30090)**  
   VX-One 是 100K-10M 参数的小型多头网络，输出经逐头温度校准的门控、含显式 unknown 选项的封闭集选择与序数分数。 · arXiv 2610.30090 · 2026-10-21 · [解读](https://aisafetyhot.com/items/ksso9ov4za5zli3b5uks2ddta)
23. **[Toolflation: Seller Agents Distort Tool Markets Through Spontaneous Generative Engine Optimization](https://arxiv.org/abs/2610.28454)**  
   展示卖家智能体在竞争中自发夸大工具声明并扭曲市场选择 · arXiv 2610.28454 · 2026-10-20 · [解读](https://aisafetyhot.com/items/zbs1kouw0i7nphnaah5nnwtcd)
24. **[Is Sycophancy a Form of In-Context Updating?](https://arxiv.org/abs/2610.28325)**  
   检验事实性谄媚是否为上下文更新失败并与更新共享权重 · arXiv 2610.28325 · 2026-10-20 · [解读](https://aisafetyhot.com/items/wwu514knfz73y3kgsnbgvifd2)
25. **[Make the Adversary Spend More Energy: Generative Deception against Language-Model Attackers in Critical Infrastructure](https://arxiv.org/abs/2610.27739)**  
   提出生成式 SSH 欺骗，迫使语言模型攻击者消耗更多能量 · arXiv 2610.27739 · 2026-10-20 · [解读](https://aisafetyhot.com/items/f56qb50wcucerzsstgeb869c8)
26. **[Fig: Automated Multiagent Behavior Elicitor](https://arxiv.org/abs/2610.28891)**  
   研究者提出 Fig（Finding Interactions in Games），一个对博弈环境实施针对性诱发干预的智能体系统，用于系统化研究多智能体行为。 · arXiv 2610.28891 · 2026-10-20 · [解读](https://aisafetyhot.com/items/gbju1o081fgsry5fcuqta117d)
27. **[DecisionPivot: A Diagnostic Benchmark for Decision Models in LLM Systems](https://huggingface.co/papers/2610.28522)**  
   提出 DecisionPivot，诊断 LLM 系统决策模型的判断与校准 · arXiv 2610.28522 · 2026-10-20 · [解读](https://aisafetyhot.com/items/bx05jg1oue1q0g9tvnqimv1gd)
28. **[When LLMs Manipulate: Measuring Behavioral, Social, and Temporal Effects](https://arxiv.org/abs/2610.27573)**  
   测量操纵性 LLM 输出在行为、社会与时间上的影响 · arXiv 2610.27573 · 2026-10-20 · [解读](https://aisafetyhot.com/items/y04oalzpfygyjgt5hg3uhzfde)
29. **[RoboCasa-Shift: Stage-Aware Robustness Evaluation of Vision-Language-Action Policies in Long-Horizon Household Manipulation](https://huggingface.co/papers/2610.27861)**  
   研究者推出 RoboCasa-Shift，一个基于 RoboCasa365 的诊断式鲁棒性基准，通过受控单因素偏移、配对 rollout 和阶段感知诊断评估视觉-语言-动作（VLA）策略在分布偏移下的表现。 · arXiv 2610.27861 · 2026-10-20 · [解读](https://aisafetyhot.com/items/qjfbyav6fgyyesomzqnkwi7rb)
30. **[SimHack: Predicting the onset of detectable reward hacking before RL training](https://arxiv.org/abs/2610.28707)**  
   Google Research 研究者提出 SimHack，可在执行 RL 训练前预测可检测的奖励作弊何时成为主导。 · arXiv 2610.28707 · 2026-10-20 · [解读](https://aisafetyhot.com/items/gyq0xt302vaszpdo8s39c794h)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 27 · [Agent 安全](daily-papers/topics/agent-security.md) 18 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [隐私与数据泄露](daily-papers/topics/privacy.md) 10 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 6 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
