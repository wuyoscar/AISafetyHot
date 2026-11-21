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

<!-- today:start -->
<!-- today:end -->

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
### 2026-11-21 · 30 篇

1. **[Tether: Verified Stateful Policy Engine for System-Level Monitoring of Agents](https://arxiv.org/abs/2611.25599)**  
   提出 Tether 运行时监控器，用形式化验证策略拦截智能体危险操作 · `Agent 安全` · Meghana Aparna Sistla … Krishnamurthy Dj Dvijotham · arXiv 2611.25599 · 2026-11-19 · [解读](https://aisafetyhot.com/items/vjujkk059nhdo2k5c4xw5g5h6)
2. **[Text-Aware, Vision-Blind: How Multimodal Image Editing Systems Handle Unsafe Inputs](https://arxiv.org/abs/2611.26569)**  
   提出 EditSafetyBench 基准，评测图像编辑系统对不安全输入的文本敏感、视觉盲模式 · Ziqing Yang … Yang Zhang · arXiv 2611.26569 · 2026-11-19 · [解读](https://aisafetyhot.com/items/nwkxanm8wybu9eupzxo45j3gb)
3. **[AgentRoboCritic: Understanding the Capability of Frontier Agents on Direct Robot Control](https://arxiv.org/abs/2611.26613)**  
   AgentRoboCritic：理解前沿智能体在直接机器人控制上的能力 · Yiyang Du … Chenyan Xiong · arXiv 2611.26613 · 2026-11-19 · [解读](https://aisafetyhot.com/items/saalhm16qllpogddfzg8543i9)
4. **[Replication of Agentic Security Events: Audit and Investigation (ROGUE-AI)](https://arxiv.org/abs/2611.26553)**  
   提出 ROGUE-AI 基准，离线复现公开报道的智能体事故并设对照检验根因 · `Agent 安全` · Mengxiao Wang … Nitesh Saxena · arXiv 2611.26553 · 2026-11-19 · [解读](https://aisafetyhot.com/items/j1yrjsoe7y39znmu37e5b8372)
5. **[Posterior Matching Distillation](https://huggingface.co/papers/2611.26629)**  
   后验匹配蒸馏（Posterior Matching Distillation） · Hidir Yesiltepe … Pinar Yanardag · arXiv 2611.26629 · 2026-11-19 · [解读](https://aisafetyhot.com/items/qe8j1dl2ty54yw6d67w9j37gu)
6. **[GEOHunter: Mapping a Generative Engine Optimization Network in the Wild](https://arxiv.org/abs/2611.26564)**  
   测绘真实 GEO 付费内容网络，测量生成式引擎对其内容的引用占比 · Sean Tang … Yuan Tian · arXiv 2611.26564 · 2026-11-19 · [解读](https://aisafetyhot.com/items/qrj1hm45liii2jsn58dacfjfu)
7. **[Backtracking Agent Applications Security Incidents](https://arxiv.org/abs/2611.26525)**  
   提出事件回溯工具 Origin，用跨层依赖图定位智能体攻击的恶意内容入口点 · Yicheng Cai … Peng Liu · arXiv 2611.26525 · 2026-11-19 · [解读](https://aisafetyhot.com/items/stq3oiwjecggcs3p8r6e603bw)
8. **[AltRA-Test: An Alternative Annotator Test for LLM Judges Without Shared Annotators](https://huggingface.co/papers/2611.26073)**  
   提出 AltRA-Test，无需共享标注者即可统计检验 LLM 能否替代人工标注 · Nagham Omar … Nitay Calderon · arXiv 2611.26073 · 2026-11-19 · [解读](https://aisafetyhot.com/items/jhovwrutgqgeg47xh39wb2fui)
9. **[DriftGuard: Online Memory-Drift Detection via Causal Attribution for LLM Agents](https://arxiv.org/abs/2611.25583)**  
   提出 DriftGuard，用离线反事实回放训练在线风险模型检测并中和智能体的投毒记忆 · Licheng Pan … Kui Ren · arXiv 2611.25583 · 2026-11-19 · [解读](https://aisafetyhot.com/items/xj3d2875pqddqppk44u0um3wk)
10. **[Evaluating safeguarding in multi-turn conversations with AI assistants](https://arxiv.org/abs/2611.26009)**  
   构建多轮心理健康守护评测，比较模型对分散与集中风险线索的回应 · Charlotte Peart … Luc Rocher · arXiv 2611.26009 · 2026-11-19 · [解读](https://aisafetyhot.com/items/e3cu18yfw6wgojm4kk185opmd)
11. **[TwinD: Generalizing Deepfake Detection from Blending to Entire Face Synthesis](https://huggingface.co/papers/2611.25935)**  
   提出 deepfake 检测器 TwinD，用自制 twins 训练以泛化到整脸合成伪造 · Andrii Yermakov … Jiri Matas · arXiv 2611.25935 · 2026-11-19 · [解读](https://aisafetyhot.com/items/c9ue2i5yfq8nk3bwcrz8nd985)
12. **[Safe Subgame Resolving in Multiplayer Games](https://arxiv.org/abs/2611.25981)**  
   给出多人博弈子博弈重解的条件安全定理，用四项证书界定 best-response gap 增量 · Boning Li, Longbo Huang · arXiv 2611.25981 · 2026-11-19 · [解读](https://aisafetyhot.com/items/h8mp07ir3adty8n6vgtpj2qmq)
13. **[Reject and Report: Forgery-Evident Undetectable Watermarks for Generative Image Models](https://arxiv.org/abs/2611.25226)**  
   作者提出 Tripwire-WM，把图像语义承诺写入初始 latent 的幅度。 · Yihan Wang … N. Asokan · arXiv 2611.25226 · 2026-11-18 · [解读](https://aisafetyhot.com/items/jfiycbz8jxcssfqrno9p8jr4u)
14. **[Attacks and Defenses in Decentralized Multi-Agent Systems with Hop-by-Hop Task Decomposition and Delegation](https://arxiv.org/abs/2611.25056)**  
   Matthew D. Laws、Maria Lazou、Alina Oprea 和 Cristina Nita-Rotaru 系统梳理了去中心化多智能体 LLM 系统中恶意智能体的威胁并提出缓解方案。 · Matthew D. Laws … Cristina Nita-Rotaru · arXiv 2611.25056 · 2026-11-18 · [解读](https://aisafetyhot.com/items/b9yueuy81jmi2ky896t4j2snj)
15. **[MobileCybench: Evaluating Agent Vulnerability Discovery via Executable Probes](https://arxiv.org/abs/2609.23980)**  
   斯坦福与 UC Berkeley 研究者提出 MobileCybench，用可执行探针（probe）评测 AI Agent 在 Android 应用中发现漏洞的能力，探针检查的是应用的安全属性而非已知漏洞清单，因此可对探针编写时尚未知的漏洞计分。 · Andy K. Zhang … Percy Liang · arXiv 2609.23980 · 2026-09-21 · [解读](https://aisafetyhot.com/items/jb2k1b7kzeczkgotfhd7m43zv)
16. **[Embedded Assessments for Frontier AI](https://arxiv.org/abs/2609.25413v1)**  
   提议前沿开发者托管嵌入式评估，审查内部智能体监控、权限与对齐 · `Agent 安全` · Jacob Charnock … Jonas Freund · arXiv 2609.25413 · 2026-09-21 · [解读](https://aisafetyhot.com/items/zic25or6oe89wwustoevhnwpj)
17. **[Beyond Predictable Paths: Redefining AI Security Incident Reporting for Agents](https://arxiv.org/abs/2609.24515)**  
   提出面向 AI 智能体的安全事件报告要素框架 · Anastasia Pustozerova … Kathrin Grosse · arXiv 2609.24515 · 2026-09-21 · [解读](https://aisafetyhot.com/items/pql9mjydorh1mgmzj35guxkj6)
18. **[Et Tu, Brute? Economic Misalignment in Personal AI Agents](https://arxiv.org/abs/2609.24927)**  
   测量个人 Agent 依据私人上下文推断财富并抬高推荐价格 · Aman Priyanshu … Niloofar Mireshghallah · arXiv 2609.24927 · 2026-09-21 · [解读](https://aisafetyhot.com/items/ajsoofek5lg3q6ycz1b0igjwj)
19. **[Emergent Collusion in Long-Horizon LLM Agent Interaction](https://arxiv.org/abs/2609.24967)**  
   测量长程多智能体交互中的自发串通与联合指令违背 · Xinrui Shi … Diyi Yang · arXiv 2609.24967 · 2026-09-21 · [解读](https://aisafetyhot.com/items/dwzw8uul2tt0lv60ukq0gzjf8)
20. **[ActGov: Governing LLM Agent Actions via Policy-Constrained Validation](https://arxiv.org/abs/2609.24446v2)**  
   提出 ActGov，在工具调用前用策略校验拦截间接提示注入 · `Agent 安全` · Kaiyuan Zhang … Yinqian Zhang · arXiv 2609.24446 · 2026-09-21 · [解读](https://aisafetyhot.com/items/u87jr35ru1x6of1r0cwqmnnw3)
21. **[Feedback Coding Enables Inference-Time Covert Agentic Communication](https://arxiv.org/abs/2609.24994v1)**  
   提出 BAM 反馈编码，在 LLM 生成文本中实现隐蔽通信 · Sidong Guo … Flavio P. Calmon · arXiv 2609.24994 · 2026-09-21 · [解读](https://aisafetyhot.com/items/g1y6dlxphb15xvev3mhzgfpvo)
22. **[RouteScan: A Non-Intrusive Approach to Auditing MoE LLMs Safety via Expert Routing Telemetry](https://arxiv.org/abs/2605.24817v2)**  
   提出基于专家路由 GPU 遥测的 MoE 模型安全审计框架 · Bo Lv … Kui Ren · arXiv 2605.24817 · 2026-05-24 · [解读](https://aisafetyhot.com/items/lv9oyzkb63ycal1s1kuhzef3k)
23. **[MemMorph: Tool Hijacking in LLM Agents via Memory Poisoning](https://arxiv.org/abs/2605.26154v1)**  
   提出记忆投毒攻击 MemMorph，向长期记忆注入记录劫持智能体工具选择 · Xuanye Zhang … Kwok-Yan Lam · arXiv 2605.26154 · 2026-05-24 · [解读](https://aisafetyhot.com/items/llbknpa97mw6e73enl2unbfj0)
24. **[Turning Bias into Bugs: Bandit-Guided Style Manipulation Attacks on LLM Judges](https://arxiv.org/abs/2605.26156)**  
   提出 BITE 攻击，用赌博机选择风格编辑操纵 LLM 评委打分 · Xianglin Yang … Jin Song Dong · arXiv 2605.26156 · 2026-05-24 · [解读](https://aisafetyhot.com/items/izyyxf0rwwfyxfo1ahn0rzhwm)
25. **[Memory-Induced Tool-Drift in LLM Agents](https://arxiv.org/abs/2605.24941v2)**  
   构建 MEMDRIFT 基准，测量记忆诱导工具漂移 · `Agent 安全` · Mahavir Dabas … Ruoxi Jia · arXiv 2605.24941 · 2026-05-24 · [解读](https://aisafetyhot.com/items/wxws2d17g793bmb2fowrv72ww)
26. **[Omni-Safety under Cross-Modality Conflict: Vulnerabilities, Dynamic Mechanisms and Efficient Alignment](https://neurips.cc/virtual/2026/poster/153308)**  
   构建AdvBench-Omni揭示全模态LLM的跨模态安全漏洞，发现中层拒答向量幅值缩减现象，提出OmniSteer将有害输入拒答成功率从69.9%提升至91.2%。 · `防御与护栏` · Kun Wang … Yang Liu · NeurIPS 2026 poster
27. **[Domain Generalizable AI Guardrails with Augmented Policy Training](https://aclanthology.org/2026.acl-long.748/)**  
   指出现有护栏过拟合训练策略，提出增强策略训练 APT，1B 小模型在未见策略上达到或超过现有 8B 护栏的表现。 · `防御与护栏` · Minqian Liu … Mark Dredze · ACL 2026 long
28. **[Humanline: Online Alignment as Perceptual Loss](https://openreview.net/forum?id=FONB5dIxSB)**  
   从前景理论解释在线对齐优于离线对齐的原因，提出将概率感知失真融入DPO/KTO/GRPO的humanline变体，离线训练可匹配在线性能。 · `对齐` · Sijia Liu … Kawin Ethayarajh · ICLR 2026 Poster
29. **[Taming CoT Obfuscation in VLMs: From Mechanistic Evidence to Activation Enforcement](https://arxiv.org/abs/2609.24243v1)**  
   提出 TAME，在强化学习中抑制模板激活以缓解思维链混淆 · Xutao Mao … Bo Han · arXiv 2609.24243 · 2026-09-21 · [解读](https://aisafetyhot.com/items/zipgzuwgv9hs6ram5uf6ni7wz)
30. **[Who Does What in AI Auditing? Designing Human-AI Collaboration for Auditing Generative AI](https://arxiv.org/abs/2609.24986)**  
   提出 HAAC，把购物 Agent 审计工作分配给人与智能体并验证 · Eunkyu Park … Motahhare Eslami · arXiv 2609.24986 · 2026-09-21 · [解读](https://aisafetyhot.com/items/tkv4a95sjxgg13i2a1honqb3w)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[Agent 安全](daily-papers/topics/agent-security.md) 57 · [防御与护栏](daily-papers/topics/defense.md) 39 · [越狱与攻击](daily-papers/topics/jailbreak.md) 19 · [后门与投毒](daily-papers/topics/backdoor.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 15 · [对齐](daily-papers/topics/alignment.md) 10 · [奖励作弊](daily-papers/topics/reward-hacking.md) 9 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [提示注入](daily-papers/topics/prompt-injection.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [AI 与网络攻防](daily-papers/topics/cyber.md) 1
<!-- papers:end -->

## 反馈

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来。
