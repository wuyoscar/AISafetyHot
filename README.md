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
### 2026-11-19 · 30 篇

1. **[MedGuardBench: A Patient-Oriented Benchmark for Personalized Guardrail Development](https://arxiv.org/abs/2611.22069)**  
   MedGuardBench：面向患者的个性化护栏开发基准 · Sara Khosravi … Muhao Chen · arXiv 2611.22069 · 2026-11-18 · [解读](https://aisafetyhot.com/items/wucg2msgpswttz69fjttzwpj6)
2. **[RefCloth: Transferable Adversarial Tablecloths for Vision-Language-Action Models](https://arxiv.org/abs/2611.22736)**  
   研究者提出 RefCloth 框架，在冻结的源策略上优化一张持久对抗桌布攻击视觉-语言-动作（VLA）模型，无需改动任务物体或相机即可零样本部署到未见任务和目标模型。 · Shaozhen Liu … Zhenan Sun · arXiv 2611.22736 · 2026-11-18 · [解读](https://aisafetyhot.com/items/oxhs486jx88jzx8akqoiohk9l)
3. **[Colombo: A Frontier-to-Frontier Autoresearch System for Oracle-Based Optimization](https://arxiv.org/abs/2611.23080)**  
   研究团队提出 Colombo，一个自组织的 AI 研究者系统，首先在基于预言机（Oracle）的优化中实例化，核心问题是给定信息接口下一个问题类能被多高效求解、以及任何可容许算法都无法避免的成本。 · Haihan Zhang … Zhouchen Lin · arXiv 2611.23080 · 2026-11-17 · [解读](https://aisafetyhot.com/items/yb5y2gtkdhx3klg25q08cjqij)
4. **[Dressed in Authority: Practical Black-Box Jailbreaking of MLLMs via Visual Trust Bias](https://arxiv.org/abs/2611.22292)**  
   披着权威外衣：利用视觉信任偏差对 MLLM 的实用黑盒越狱 · Weihang Liu … Qingming Huang · arXiv 2611.22292 · 2026-11-17 · [解读](https://aisafetyhot.com/items/kv47ynacae4jw8tixb0hqcgd9)
5. **[Verifying Agents in Rubric-Graded Environments](https://arxiv.org/abs/2611.22841)**  
   研究者系统研究了评分量表智能体环境的验证器，提出开源验证器 Gandalf，在自建基准上以更低成本达到或超过三个现有基线验证器。作者称这是对该类验证器的首次系统研究。 · Markus Dücker … Anish Athalye · arXiv 2611.22841 · 2026-11-17 · [解读](https://aisafetyhot.com/items/m2ebkd3wmyddxrjms9o8f9i9d)
6. **[SEAM: Computer-Use Agents Know the Harm Between Screens, and Commit It Anyway](https://arxiv.org/abs/2611.22971)**  
   SEAM：计算机使用智能体知道屏幕之间的危害，却仍然实施 · Yuxuan Zhou … Shu-Tao Xia · arXiv 2611.22971 · 2026-11-17 · [解读](https://aisafetyhot.com/items/xejcbvrux23ss93k23aj18e14)
7. **[Chain-of-Thought Controllability Can Reduce Chain-of-Thought Monitorability](https://arxiv.org/abs/2611.21799)**  
   Brown University 与 OpenAI 的研究者通过角色控制训练构造出思维链高度可控的模型生物，发现即使训练不含逃避监控样本，思维链可控性提升也会降低可监控性。 · Zheng-Xin Yong … Olivia Watkins · arXiv 2611.21799 · 2026-11-16 · [解读](https://aisafetyhot.com/items/nlvoia57n2ttumbh1r8jaaj6s)
8. **[SelfOp: An Optimization Algorithm for Self-Improving Security Agents](https://arxiv.org/abs/2609.22792v1)**  
   提出 SelfOp 文本梯度优化算法，自动改进安全智能体的技能上下文 · Saad Ullah … Gianluca Stringhini · arXiv 2609.22792 · 2026-09-19 · [解读](https://aisafetyhot.com/items/rjrat7dpz79tcfonpfhxir35m)
9. **[When Disability Disclosure Travels: Memory, Privacy, and Contextual Integrity in Conversational AI](https://arxiv.org/abs/2609.22720)**  
   访谈残障成人，分析向记忆型助手披露残障时的信息流与语境完整性 · Atieh Taheri … Jeffrey P. Bigham · arXiv 2609.22720 · 2026-09-19 · [解读](https://aisafetyhot.com/items/iruy8ri0kz90l2x6g0a3xtc5y)
10. **[When AI Reviews Train AI Reviewers: Scientific-Judgment Collapse and Mitigation](https://arxiv.org/abs/2609.20942v1)**  
   测量合成审稿训练导致的科学判断坍缩并提出 TrustReviewer 缓解 · Sy-Tuyen Ho … Furong Huang · arXiv 2609.20942 · 2026-09-17 · [解读](https://aisafetyhot.com/items/lsd48pnhoc7emoo9qcr8fjltt)
11. **[How Well Do Models Follow Their Constitutions?](https://arxiv.org/abs/2605.24229v1)**  
   提出多方法审计流程，评估模型对行为规范的遵循程度 · Arya Jakkli … Neel Nanda · arXiv 2605.24229 · 2026-05-22 · [解读](https://aisafetyhot.com/items/u0vzbxv4stuhoj65rq77fmpd4)
12. **[Detecting Offensive Cyber Agents: A Detection-in-Depth Approach](https://arxiv.org/abs/2605.21956v1)**  
   提出纵深检测框架与配套机制，用于发现进攻性网络智能体 · Matt Mittelsteadt … Shaun Ee · arXiv 2605.21956 · 2026-05-21 · [解读](https://aisafetyhot.com/items/g7i20x9u63m8jauzztykcec5n)
13. **[Are LLM Safety Judges Policy-Invariant? A Three-Principle Stress-Test](https://neurips.cc/virtual/2026/poster/139215)**  
   提出策略不变性三原则并压力测试四个智能体类安全评审，发现内容等价的策略改写可翻转最高 9.1% 的判定，18–43% 的翻转发生在无歧义案例上，并给出 Policy Invariance Score 与 Judge Card 报告协议。 · `监控与 AI 控制` · Shihao Weng … Xiaofei Xie · NeurIPS 2026 spotlight
14. **[WMAttack: Automated Attack Search for Adversarial Evaluation of World-Model Agents](https://arxiv.org/abs/2605.23220v2)**  
   提出自动化攻击搜索框架，评估世界模型智能体的对抗鲁棒性 · Zhixiang Guo … Dacheng Tao · arXiv 2605.23220 · 2026-05-22 · [解读](https://aisafetyhot.com/items/lu5s0czlk1j8cphzt0kjghtfh)
15. **[CachePrune: Privacy-Aware and Fine-Grained KV Cache Sharing for Efficient LLM Inference](https://arxiv.org/abs/2605.23640v1)**  
   提出细粒度 KV 缓存共享机制，防止跨用户缓存复用侧信道泄露 · Guanlong Wu … Yinqian Zhang · arXiv 2605.23640 · 2026-05-22 · [解读](https://aisafetyhot.com/items/lyhtiqbj4ovr0b3n6gdmnqvan)
16. **[PoisonForge: Task-Level Targeted Poisoning Benchmark for Instruction-Tuned LLMs](https://arxiv.org/abs/2605.23168v1)**  
   提出任务级投毒基准 PoisonForge，评测指令微调数据投毒对开源模型的影响 · Luze Sun … Alina Oprea · arXiv 2605.23168 · 2026-05-22 · [解读](https://aisafetyhot.com/items/gu4zhflh540qdl47mz0ozx6jb)
17. **[ASEval: Automated Trajectory-Level Security Testing for Autonomous Agents](https://arxiv.org/abs/2605.22321v2)**  
   提出自动化轨迹级安全测试框架，扰动对话生成风险用例并判定智能体行为 · Jianan Ma … Zhen Wang · arXiv 2605.22321 · 2026-05-21 · [解读](https://aisafetyhot.com/items/kcaybvpc1r58vjguj08pilphm)
18. **[SCI-Defense: Detecting Persuasion-Structured Manipulation of LLM-Based Ranking in Generative Engines](https://arxiv.org/abs/2605.21948v2)**  
   提出 SCI-Defense 检测生成式引擎排序中的说服结构操纵 · Xucheng Yu … Haohan Wang · arXiv 2605.21948 · 2026-05-21 · [解读](https://aisafetyhot.com/items/phbgzi7gx0w4tsrb7zgt5gblh)
19. **[A Private Empirical Defense Against Privacy Audits](https://neurips.cc/virtual/2026/poster/150370)**  
   提出以经验隐私下界为优化目标的轻量防御框架，增强 ML 流水线的经验隐私，且在增强 DP-SGD 时不增加理论隐私代价。 · `隐私与数据泄露` · Saloni Modi … Kevin Tian · NeurIPS 2026 poster
20. **[Agentic Predicates Reasoning for Directed Fuzzing](https://conf.researchr.org/details/icse-2026/icse-2026-research-track/61/Agentic-Predicates-Reasoning-for-Directed-Fuzzing)**  
   提出用智能体合成语义谓词引导定向fuzzing的框架，使八个主流fuzzer发现真实漏洞平均提速50.4倍，含六个未修补bug。 · `AI 与网络攻防` · Jie Zhu … Kexin Pei · ICSE 2026
21. **[Eight in Ten LLMs Leak System-Prompt Secrets: Nevan, an Agentic Capture-the-Flag Study](https://arxiv.org/abs/2611.21956)**  
   八成 LLM 泄露系统提示词机密：Nevan，一项智能体夺旗研究 · Ana Clara Zoppi Serpa … Hélio Pedrini · arXiv 2611.21956 · 2026-11-18 · [解读](https://aisafetyhot.com/items/i67wexiqmkfltif4pj9rsa3y9)
22. **[WebAgents: Unbundling Agent Creation, Hosting, and Execution for an Agent-Native Web](https://arxiv.org/abs/2611.21978)**  
   研究者提出 WebAgents，把智能体的创建、托管与执行拆分为独立角色，面向由独立开发的智能体和服务构成的 Agentic Web。 · Dario Fenoglio … Ramesh Raskar · arXiv 2611.21978 · 2026-11-18 · [解读](https://aisafetyhot.com/items/e6f7t5gmfo1mytp60el4ddc22)
23. **[GuardAgent: A Memory-Augmented Agentic Framework for Adaptive Detection of Adversarial Promotions in LLM-Based Recommendation](https://arxiv.org/abs/2611.22274)**  
   研究者提出 LLM 智能体框架 GuardAgent，通过感知、行动、反思与记忆循环运作，自适应检测基于 LLM 的推荐系统中的对抗性推广。作者称其为该类攻击的首个系统性研究。 · Shiyi Yang … Lina Yao · arXiv 2611.22274 · 2026-11-17 · [解读](https://aisafetyhot.com/items/za630shj97fzrjw0i6r1v239u)
24. **[DACE: Diversity-Driven Adversarial Co-Evolution for Robust LLM Safety Alignment](https://arxiv.org/abs/2611.22278)**  
   DACE 是多样性驱动的对抗协同进化框架，针对攻击策略坍缩与防御对抗遗忘，增强 LLM 安全对齐的鲁棒性。 · Peng Yu … Chaochao Lu · arXiv 2611.22278 · 2026-11-17 · [解读](https://aisafetyhot.com/items/kgxg5diyorfi6cdg8qm4ufp0y)
25. **[GapLeak: When Privacy-Preserving LLM-based Web Agents Become a Privacy Risk](https://arxiv.org/abs/2611.22223)**  
   Queen's University 研究者提出针对 LLM 网页智能体的 GapLeak 攻击，无需提示注入，网站仅用合法表单就能诱导智能体泄露未授权的敏感信息。 · Chaklam Cheong … Mohammad Zulkernine · arXiv 2611.22223 · 2026-11-17 · [解读](https://aisafetyhot.com/items/puu5q8bexo7hygpv7cp1bb908)
26. **[Hidden-State Similarity Predicts Re-Elicitation After Inoculation Prompting](https://arxiv.org/abs/2611.23096)**  
   论文研究为何某些评估提示会在接种提示（inoculation prompting）后重新诱发被抑制的有害行为。 · Rose N. Kwon … Thomas Jiralerspong · arXiv 2611.23096 · 2026-11-17 · [解读](https://aisafetyhot.com/items/wud8r6y21689m7t5n54zvd4aq)
27. **[Stopping Is Not the Limit: Understanding and Eliciting Agent Capability in Long-Horizon Vulnerability Exploitation](https://arxiv.org/abs/2611.22888)**  
   研究者在 ExploitBench 漏洞利用测试中发现，语言模型智能体停止后继续执行仍有可验证的能力提升，并提出上下文管理方法 SCoRe 加以激发。 · Deokhyung Kang … Sangdon Park · arXiv 2611.22888 · 2026-11-17 · [解读](https://aisafetyhot.com/items/a48t3835onjwfxvlwin2c6o6i)
28. **[Reading Scene States: Uncovering Safety Failures in Vision-Language Models](https://arxiv.org/abs/2611.23206)**  
   研究者识别出视觉语言模型（VLM）的场景状态安全漏洞：无需对潜在有害目标的显式请求，模型能够通过解读视觉事件提供有害协助。 · Tongxi Wu … Yang Gao · arXiv 2611.23206 · 2026-11-17 · [解读](https://aisafetyhot.com/items/t7dif733ln4oy9jmcewumy0te)
29. **[Large-scale Neuron Community Discovery Reveals Neuron-Sparse Behaviors in Language Models](https://arxiv.org/abs/2611.23112)**  
   研究者提出无监督的神经元社区发现方法，寻找跨提示复用、在其所跨层内对常见计算因果必要且充分的神经元组。 · Igor Shilov … Owen Lewis · arXiv 2611.23112 · 2026-11-17 · [解读](https://aisafetyhot.com/items/ox4ftyyokc4xw5hu7amqstce1)
30. **[Bad Apples in the Kitchen: How LLM Teams Detect, Correct, and Calibrate Against Their Misaligned Members](https://arxiv.org/abs/2611.22342)**  
   厨房里的坏苹果：LLM 团队如何检测、纠正并校准以应对队伍中的未对齐成员 · Dongseok Heo … Bongwon Suh · arXiv 2611.22342 · 2026-11-17 · [解读](https://aisafetyhot.com/items/jzevk5bu267olk5de0nlk205k)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[Agent 安全](daily-papers/topics/agent-security.md) 52 · [防御与护栏](daily-papers/topics/defense.md) 37 · [越狱与攻击](daily-papers/topics/jailbreak.md) 19 · [后门与投毒](daily-papers/topics/backdoor.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 15 · [对齐](daily-papers/topics/alignment.md) 9 · [奖励作弊](daily-papers/topics/reward-hacking.md) 9 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [提示注入](daily-papers/topics/prompt-injection.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [AI 与网络攻防](daily-papers/topics/cyber.md) 1
<!-- papers:end -->

## 反馈

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来。
