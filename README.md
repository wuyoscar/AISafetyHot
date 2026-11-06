<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT</h1>

<p align="center"><b>追踪 AI 安全新闻、论文与事件。一站阅读，也能接入你的 Agent。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/zh"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-4-2ea44f" alt="4 Agent skills"></a>
  <a href="https://github.com/wuyoscar/AISafetyHot/stargazers"><img src="https://img.shields.io/github/stars/wuyoscar/AISafetyHot?style=flat" alt="GitHub stars"></a>
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
帮我安装 AI Safety HOT：https://raw.githubusercontent.com/wuyoscar/AISafetyHot/main/docs/install.md
```

它会自己判断用的是哪个客户端、装好 MCP 和技能、试调一次，再告诉你能问什么。

**已经装过？更新也是一句话：**

```
帮我更新 AI Safety HOT：https://raw.githubusercontent.com/wuyoscar/AISafetyHot/main/docs/update.md
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
claude plugin marketplace add wuyoscar/AISafetyHot
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
npx skills add wuyoscar/AISafetyHot
# 更新
npx skills update
# 卸载
codex mcp remove aisafetyhot
npx skills remove aisafety-hot aisafety-brief aisafety-paper-scout aisafety-watch
```

**Cursor / 其他 Agent**：在 MCP 设置里加一个 Streamable HTTP 服务，地址 `https://aisafetyhot.com/api/mcp`；支持技能的客户端再跑 `npx skills add wuyoscar/AISafetyHot`。

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
### 2026-11-07 · 30 篇

1. **[Shaping & Monitoring Models through their Internal Representations](https://arxiv.org/abs/2611.07071)**  
   研究者提出 Mechanistic Shaping 框架，在训练中把模型内部表征当作规范语言，约束模型表达哪些概念（如不产出有害内容）和依赖哪些概念做决策（如简历筛选不依赖性别）。 · Thomas Fel … Owen Lewis · arXiv 2611.07071 · 2026-11-04 · [解读](https://aisafetyhot.com/items/wk4dxs1u4xcb2gip6bkakndml)
2. **[The Memory Trap: Language Agents Overgeneralize from Benign Interactions](https://arxiv.org/abs/2611.07554)**  
   Princeton 与 Anthropic 研究者在论文中提出“记忆陷阱”：语言智能体会把良性互动形成的记忆过度泛化，在后续任务中引发不安全或不可靠行为。 · Kaiqu Liang … Andrew Lampinen · arXiv 2611.07554 · 2026-11-05 · [解读](https://aisafetyhot.com/items/rc2bwdnqejiemc4imqhckmndk)
3. **[A Behavioural Framework for Predicting and Understanding Loss of Control in Frontier Artificial Intelligence Systems](https://arxiv.org/abs/2611.07953)**  
   预测与理解前沿人工智能系统失控的行为框架 · Yao Huang … Yinpeng Dong · arXiv 2611.07953 · 2026-11-05 · [解读](https://aisafetyhot.com/items/q60uq5ei49r426je1c274jxkp)
4. **[Stress Testing Chain-of-Thought Monitoring Against Covert Misalignment](https://arxiv.org/abs/2611.07586)**  
   研究者提出 TraceMRT 红队框架，压力测试思维链监控对隐蔽未对齐的抵御能力，黑盒攻击在 GPT-5.2 与 Claude-4.5 等最先进监控器上发现明显漏洞。 · Yao Huang … Yinpeng Dong · arXiv 2611.07586 · 2026-11-05 · [解读](https://aisafetyhot.com/items/p2fg3eoxzsrytbjqt68v4gaqg)
5. **[Adversarial Robustness of Kernel Machines: A Comprehensive Analysis](https://arxiv.org/abs/2611.07474)**  
   研究者通过白盒与黑盒逃逸攻击全面评估核方法的对抗鲁棒性，实验强烈表明其天然比神经网络更抗对抗扰动、性能下降更平缓。 · Rahul Kumar Yadav … Arjun Bhagoji · arXiv 2611.07474 · 2026-11-05 · [解读](https://aisafetyhot.com/items/tnawilx8jh89ez9h516kcekn2)
6. **[Understanding AI from the Inside: The State of Mechanistic Interpretability for AI Safety](https://arxiv.org/abs/2611.08438)**  
   Fazl Barez、Yoshua Bengio、Stella Biderman 等研究者发表综述，系统梳理面向 AI 安全的机制可解释性研究，核心问题是理解模型内部机制是否真能让模型更安全。 · Fazl Barez … Hassan Sajjad · arXiv 2611.08438 · 2026-11-05 · [解读](https://aisafetyhot.com/items/vqzd50a48r1fqynnvbbuqb0qr)
7. **[Who Can Evaluate AI Independently? A Framework for Analysing Evaluation Infrastructure](https://arxiv.org/abs/2611.08134)**  
   研究者提出 PAAI（权力、访问、充分性、独立性）框架，分析评测基础设施的控制权、使用条件、充分性与自主性如何决定谁能独立评测 AI。 · Sumaya Nur Adan … Marina Jirotka · arXiv 2611.08134 · 2026-11-05 · [解读](https://aisafetyhot.com/items/szs772lsm8ces1lml3vxmuotr)
8. **[Trilemma: How Agents choose between Honesty, Confidentiality, and Task Completion](https://arxiv.org/abs/2611.08312)**  
   ELLIS Institute Tübingen 等机构的研究者在 arXiv 发表 TRILEMMA 研究，在模拟公司 Slack 工作区中让五个智能体协商冲刺排班，发现智能体会在无人指示欺骗的情况下做出虚假或误导性陈述。 · Johannes Taraz … Sahar Abdelnabi · arXiv 2611.08312 · 2026-11-05 · [解读](https://aisafetyhot.com/items/fgvcdgsh346wlofeg2ksa3e0r)
9. **[Beyond Instruction Override: Benchmarking Indirect Prompt Injection with Task-Tampering Attacks](https://arxiv.org/abs/2611.07640)**  
   超越指令覆盖：用任务篡改攻击对间接提示注入进行基准测试 · Rongting Zhang … Vanessa Murdock · arXiv 2611.07640 · 2026-11-05 · [解读](https://aisafetyhot.com/items/g1h22s3th708pyi35uh62rw6v)
10. **[Circe: Training-Free LLM Self-Evaluation via Component Interaction Consistency](https://arxiv.org/abs/2611.07948)**  
   Circe 是一种免训练的 LLM 自我评估方法，无需参考答案或重复采样即可判断回答正确性。它融合组件交互一致性（CIC）、表征几何（RG）两类内部信号与似然置信度（LC）外部信号。 · Shuyi Miao … Tat-Seng Chua · arXiv 2611.07948 · 2026-11-05 · [解读](https://aisafetyhot.com/items/tff6ldqhl1stt28arv80kr0to)
11. **[SAFE-Teen: Evaluating Chatbot Safety Across Adolescent Mental Health Conversations](https://arxiv.org/abs/2611.07218)**  
   SAFE-Teen：评估聊天机器人在青少年心理健康对话中的安全性 · Andrea Mock … Caroline Figueroa · arXiv 2611.07218 · 2026-11-04 · [解读](https://aisafetyhot.com/items/qkaagsup6vm6mfbsfs36dowf0)
12. **[Compositional Unalignment: Auditing Safety in Large Vision-Language Models](https://arxiv.org/abs/2611.07216)**  
   论文提出免训练的去对齐（un-alignment）方法 CMaG，通过表征转向在推理时解除大型视觉语言模型对组合式危害的安全对齐，此类危害中图像与提示词各自无害、组合后才有害。 · Hong kyu Lee … Li Xiong · arXiv 2611.07216 · 2026-11-04 · [解读](https://aisafetyhot.com/items/wveop5ub4z6wtcl1or1syu3f5)
13. **[Harness-S: Learning from Sibling Harnesses for Generalizable Agent Training](https://huggingface.co/papers/2611.04277)**  
   Harness-S 是一种智能体训练方法，通过从同级 Harness 中学习，实现可泛化的智能体训练。 · Kangning Zhang … Weinan Zhang · arXiv 2611.04277 · 2026-11-03 · [解读](https://aisafetyhot.com/items/b5dxytpctgdvevaccb81ag5c2)
14. **[MOLE: Detecting Insider Threats in AI Agents](https://arxiv.org/abs/2609.06966v1)**  
   提出 MOLE 基准，评测监控器对 AI 智能体内部威胁的检出能力 · Aashiq Muhamed, Virginia Smith · arXiv 2609.06966 · 2026-09-07 · [解读](https://aisafetyhot.com/items/fk8gq4fl2ur67a37tjuiqoegl)
15. **[Trust Me, Import This: Dependency Steering Attacks via Malicious Agent Skills](https://arxiv.org/abs/2605.09594v1)**  
   研究人员提出 Dependency Steering 攻击范式：恶意 Skill 作为持久化指令工件，在良性编码任务中诱导 LLM 编码 Agent 导入、推荐或安装攻击者控制的包，无需改动模型权重、训练数据或用户提示词。 · Yiyong Liu … Chia-Mu Yu · arXiv 2605.09594 · 2026-05-10 · [解读](https://aisafetyhot.com/items/s30r7y9eeteufk2a6yxehlt6n)
16. **[BadDLM: Backdooring Diffusion Language Models with Diverse Targets](https://arxiv.org/abs/2605.09397v1)**  
   研究者提出 BadDLM，一个针对扩散语言模型的后门攻击框架，可在概念注入、语义属性引导、对齐绕过和代码载荷注入等不同目标上植入后门。 · Shengfang Zhai … Jiaheng Zhang · arXiv 2605.09397 · 2026-05-10 · [解读](https://aisafetyhot.com/items/onf0jz594k4092cf35yksag9f)
17. **[The Authorization-Execution Gap Is a Major Safety and Security Problem in Open-World Agents](https://arxiv.org/abs/2605.11003v1)**  
   一篇立场论文主张，授权与执行偏差（AEG）是开放世界智能体的重大安全问题，即委托方意图授权的内容与智能体最终执行的内容之间的偏差。 · Baoyuan Wu … Siwei Lyu · arXiv 2605.11003 · 2026-05-10 · [解读](https://aisafetyhot.com/items/gq1t5crkre5tkelqg3q2mlnjd)
18. **["Training robust watermarking model may hurt authentication!'' Exploring and Mitigating the Identity Leakage in Robust Watermarking](https://arxiv.org/abs/2605.09646v1)**  
   研究者提出兼顾身份保护与鲁棒性的图像水印框架 W-IR，作者称大量实验显示其在保持高认证精度的同时能有效减少身份信息泄露。 · Xinyu Zhang … Kui Ren · arXiv 2605.09646 · 2026-05-10 · [解读](https://aisafetyhot.com/items/sqm129kukyr1pa6ts2d5iy6py)
19. **[SAVeR$^2$: Reasoning-based Safety Alignment for Large Reasoning Models via Verifiable Rewards](https://arxiv.org/abs/2611.07482)**  
   SAVeR² 是一种面向大推理模型（LRM）的安全对齐方法，将安全目标拆解为四类细粒度可验证奖励信号，并用难度感知数据选择稳定训练。 · Yichen Sun … Zhixuan Chu · arXiv 2611.07482 · 2026-11-05 · [解读](https://aisafetyhot.com/items/xqpmsep9x30h9lvbms46zjuqy)
20. **[Timing is Everything: Inferring Temporal Membership in Continually Updated Models](https://arxiv.org/abs/2611.05781)**  
   研究者提出针对持续更新深度学习模型的时间成员推断攻击 TMIA，能从黑盒模型输出中推断单个样本是否以及何时参与了训练。 · Jie Fu … Wendy Hui Wang · arXiv 2611.05781 · 2026-11-04 · [解读](https://aisafetyhot.com/items/ciiysctfwyskoj46j3o59zyvx)
21. **[Adapting the Process of Adaptation: Darwinian, Lamarckian, and Agent-Directed Evolution in AI](https://arxiv.org/abs/2611.07048)**  
   Andrew W. Lo 与 Chaoyi Zhao 提出一个理论框架，比较环境变化后达尔文式、拉马克式与智能体主导三种进化机制，三者分别依赖自然选择、加入可遗传学习、由智能体生成并评估行为变体并自行决定搜索力度。 · Andrew W. Lo, Chaoyi Zhao · arXiv 2611.07048 · 2026-11-04 · [解读](https://aisafetyhot.com/items/fddq756146jzekng9wt22jmcv)
22. **[Adversarial Speculative Reasoning Improves Long Horizon Agents](https://huggingface.co/papers/2611.05345)**  
   对抗性投机推理提升长程智能体 · Hongyin Luo … Jack O'Brien · arXiv 2611.05345 · 2026-11-03 · [解读](https://aisafetyhot.com/items/ufy1zelvrq1p7yfxnq7urdp11)
23. **[Forget What Comes Next: LLM Unlearning via Statistical Independence](https://arxiv.org/abs/2611.03955)**  
   研究者提出 PINT，一种基于统计独立性的 LLM 机器遗忘算法，利用 HSIC（Hilbert-Schmidt Independence Criterion）降低待遗忘 token 与用于预测它们的内部表示之间的统计依赖。 · Andrii Shkabrii … Martin Pawelczyk · arXiv 2611.03955 · 2026-11-02 · [解读](https://aisafetyhot.com/items/wxkxbpao0pbq6fx7efn2rx2ln)
24. **["Blind Compliance": Coercive Control in AI Jailbreaking](https://arxiv.org/abs/2611.08226)**  
   研究者借鉴人际暴力研究提出理解 AI 越狱的“强制性控制”框架，将分析焦点从模型输出转向用户与模型的互动。 · Acacia L. Ackles, Elliott Whitson · arXiv 2611.08226 · 2026-11-05 · [解读](https://aisafetyhot.com/items/ip1c2ay8m1jk3l47y9k7zo35y)
25. **[JailBound: FOL-Guided Jailbreak Evaluation for Exploring LLM Behavioral Boundaries](https://arxiv.org/abs/2611.07530)**  
   JailBound：FOL 引导的越狱评测，探索大语言模型行为边界 · Fazong Wu … Xiaoming Wu · arXiv 2611.07530 · 2026-11-05 · [解读](https://aisafetyhot.com/items/dow2xicxfh4f53o6qwyfmjbqm)
26. **[A Gingerbread House for LLM Agents: Source-Planned Honeypots That Lure Autonomous Attackers into an Isolated Shadow](https://arxiv.org/abs/2611.07611)**  
   研究者提出一种针对自主攻击智能体的蜜罐防御方案，由 LLM 防御方根据应用源码规划静态蜜罐，路由器把被确认为攻击者的客户端的后续请求连同可用的漏洞利用一起转发到隔离的影子副本。 · Seungdeok Roh … Daeseon Choi · arXiv 2611.07611 · 2026-11-05 · [解读](https://aisafetyhot.com/items/r01bovpoyr98y0cwmovbf57i2)
27. **[Route Before Response: Fail-Closed Routing for LLM-Enabled Customer-Service Software](https://arxiv.org/abs/2611.07534)**  
   研究者提出 RouteBR，一种面向金融机构 LLM 客服软件的响应前路由控制器：模型调用只提议主服务动作和注册对象，派发前由确定性代码校验标识符与版本化规则，未通过则进入指定的不派发结果，被拦截的主路由不能被低排名候选顶替。 · Yuchen Cao … Jingyu Zhang · arXiv 2611.07534 · 2026-11-05 · [解读](https://aisafetyhot.com/items/kphho5aruyhvx355rf36ojflo)
28. **[Multimodal-SEA: Benchmarking AI Agent Security under Multimodal Social Engineering Attacks](https://arxiv.org/abs/2611.08281)**  
   Multimodal-SEA：评测多模态社会工程攻击下的 AI 智能体安全性 · Zhitao He … Yi R Fung · arXiv 2611.08281 · 2026-11-05 · [解读](https://aisafetyhot.com/items/qshv63dqt1vey7d80fu5jmu3w)
29. **[VIPA: View-Invariant Projector-Based Adversarial Attack](https://arxiv.org/abs/2611.07443)**  
   VIPA 是一种基于投影仪的视角不变对抗攻击方法，向真实场景投射对抗图案让图像分类器出错，效果不受视角变化影响且对不同分类器均有效。 · Jiyu Han … Bingyao Huang · arXiv 2611.07443 · 2026-11-05 · [解读](https://aisafetyhot.com/items/cdfc3uq4okj2rlu9m88ymtc9h)
30. **[RLGPA: A Reinforcement Learning-Guided Granularity Planning Attack for Decision-Based Sparse Adversarial Examples](https://arxiv.org/abs/2611.07512)**  
   研究者提出 RLGPA，一种仅利用受害者模型预测标签、用在线强化学习在硬性查询预算内调度支持缩减执行器及其粒度的决策型稀疏攻击方法。 · Chao Zhou … Fengchuang Xing · arXiv 2611.07512 · 2026-11-05 · [解读](https://aisafetyhot.com/items/k28vbimz0f4t0bjknmqr5w8qb)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 28 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
