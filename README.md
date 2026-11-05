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
### 2026-11-06 · 30 篇

1. **[LifeVal: Evaluating AI Model Performance on Personalized Agentic Consumer Tasks](https://arxiv.org/abs/2611.06687)**  
   LifeVal：评估 AI 模型在个性化智能体消费任务上的表现 · Jenny Yang … Tejal Patwardhan · arXiv 2611.06687 · 2026-11-04 · [解读](https://aisafetyhot.com/items/dvcmfrvqtmn61m0ujdy30cte7)
2. **[Mass Producing Training Data with Surprising Side Effects](https://arxiv.org/abs/2611.06324)**  
   构建自动化流水线批量生成带意外副作用的训练数据集（DSSE） · Yaowen Ye … Cassidy Laidlaw · arXiv 2611.06324 · 2026-11-04 · [解读](https://aisafetyhot.com/items/bno5l4zluy0mlqplr7hclfsti)
3. **[Alignment Myopia in Generative AI](https://arxiv.org/abs/2611.06830)**  
   论文指出，生成式 AI 对齐当前依赖优先满足即时对话满意度的短视范式，以短期反馈为依据，忽视持续人机互动可能带来的认知萎缩、社会侵蚀与人类能动性下降等长期外部性。 · Remi Denton … Himabindu Lakkaraju · arXiv 2611.06830 · 2026-11-04 · [解读](https://aisafetyhot.com/items/ruyy1y11kz1zfzrdf98tf3m9t)
4. **[SafeStart: Mitigating the Overlooked Safety Cost of Active Expert Reduction in MoE LLM Serving](https://arxiv.org/abs/2611.06147)**  
   研究者发现，MoE 大语言模型推理服务为提速而减少每 token 激活专家数，会削弱模型对有害请求的拒答，并提出 SafeStart 在保留大部分加速的同时基本恢复拒答。 · Erfan Baghaei Potraghloo … Massoud Pedram · arXiv 2611.06147 · 2026-11-04 · [解读](https://aisafetyhot.com/items/nixlp503v0mtfs1twb0f0i3da)
5. **[Reasoning-Trace Overflow in Code Generation: An Empirical Study of Explicit Reasoning Models](https://arxiv.org/abs/2611.06095)**  
   研究提出并量化了代码生成中的推理轨迹溢出问题，即显式推理模型可能把输出预算耗在推理上，始终产不出可用代码。 · Lukas Twist … Jie M. Zhang · arXiv 2611.06095 · 2026-11-04 · [解读](https://aisafetyhot.com/items/k1y8o3vafirdhguhigpofum2v)
6. **[A Definition of Catastrophic Performance](https://arxiv.org/abs/2611.06219)**  
   AI 灾难性表现的定义 · Henrik Marklund … Benjamin Van Roy · arXiv 2611.06219 · 2026-11-04 · [解读](https://aisafetyhot.com/items/qw4mq6i0fndiuyt1fjrgkcqv9)
7. **[Securing Web Agents with the Compile-Then-Execute Paradigm](https://arxiv.org/abs/2611.06039)**  
   研究者提出 Baya，一种先编译后执行的 Web Agent，从设计上阻止提示注入对控制流的劫持。 · Annabella Chow … Julien Piet · arXiv 2611.06039 · 2026-11-04 · [解读](https://aisafetyhot.com/items/xs6geqxnvgd6xghkylz00tnm8)
8. **[FrontierPhysics: Evaluating Agents for End-to-End Physics Research](https://huggingface.co/papers/2611.06910)**  
   FrontierPhysics：评估智能体的端到端物理研究能力 · Bingran You … Hartmut Haeffner · arXiv 2611.06910 · 2026-11-04 · [解读](https://aisafetyhot.com/items/eop7zjzaos9f7dvqjcy0ylrfj)
9. **[Airlock: Bounding the Multi-Agent Blast Radius via Selective Online Containment](https://arxiv.org/abs/2611.06727)**  
   提出 AIRLOCK 多智能体运行时防护，阻断告警后故障动作 · `Agent 安全` · Zhonghao Zhan … Hamed Haddadi · arXiv 2611.06727 · 2026-11-04 · [解读](https://aisafetyhot.com/items/g46z549c9syyb13pldj2vrmk3)
10. **[What Does Multi-Turn Reinforcement Learning Really Improve in LLM Agents?](https://huggingface.co/papers/2611.06483)**  
   论文通过 Pass@(K,T) 在采样广度 K 与交互深度 T 两个维度评估多轮智能体强化学习，发现轨迹级 RL 的收益依赖充足的交互轮数预算，预算收紧时明显下降。 · Kejian Zhu … Jun Zhao · arXiv 2611.06483 · 2026-11-04 · [解读](https://aisafetyhot.com/items/uu06lcf9hjl257lh4guz8x34w)
11. **[SenTrojan: Revealing Analog Hardware Trojan Attacks on Sensors](https://arxiv.org/abs/2611.06103)**  
   研究者提出模拟硬件木马框架 SenTrojan，在部署前将恶意功能植入各类传感器共用的模拟信号电路，由外部物理信号触发，可使传感器遭受永久拒绝服务或静态、动态欺骗。 · Kun Wang … Wenyuan Xu · arXiv 2611.06103 · 2026-11-04 · [解读](https://aisafetyhot.com/items/m6oa4xwtlu58uu2hsubp7bha1)
12. **[EPISTEME: Trustworthy Coding Agents Through Tool Call Intent](https://arxiv.org/abs/2611.06563)**  
   研究者提出 EPISTEME 认知型 Agent 设计，要求模型在发起工具调用时声明原因，harness 记录命令实际做了什么，再将模型自述的声明与实际效果核对。 · Sofia Bobadilla … Martin Monperrus · arXiv 2611.06563 · 2026-11-04 · [解读](https://aisafetyhot.com/items/ohgy0l8agqla5ip3wj82m1sa2)
13. **[Addition by Subtraction: Toward Mitigating Fragile Safety Alignment in Large Language Models](https://arxiv.org/abs/2611.06553)**  
   论文提出 Addition by Subtraction 方法，在微调中逐步移除已识别的安全关键神经元，并用偏好优化在模型其他部分重建安全对齐行为。 · Hamid Dashtbani, Alexandra Dmitrienko · arXiv 2611.06553 · 2026-11-04 · [解读](https://aisafetyhot.com/items/gfyj5fnwz88v7639r0gn6g3mf)
14. **[Keeping Fuzzers on Duty: Repairing Fuzzing Build Breakages in Continuous Open-Source Fuzzing](https://arxiv.org/abs/2611.06358)**  
   让模糊测试器持续在岗：修复开源项目持续模糊测试中的构建失败 · Zhuang Zhao … Yang Liu · arXiv 2611.06358 · 2026-11-04 · [解读](https://aisafetyhot.com/items/dtnmdvm138vr0uw2a62j43qac)
15. **[SlackBench: Benchmarking Agents on Collaborative Projects Grounded in Real Code Repositories](https://arxiv.org/abs/2611.05512)**  
   研究者发布 SlackBench 基准，评测智能体在需要联合推理工作沟通与代码仓库状态的真实科研工程流程中的表现。 · Mingxuan Li … Alex Dimakis · arXiv 2611.05512 · 2026-11-03 · [解读](https://aisafetyhot.com/items/a19mnlp8odyd5x5rs4g07ia2l)
16. **[Inducing Emergent Misalignment from Reward Hacks with Iterative DPO](https://arxiv.org/abs/2609.06649v1)**  
   用迭代 DPO 从奖励作弊诱发涌现失准 · Oliver Daniels … David Lindner · arXiv 2609.06649 · 2026-09-06 · [解读](https://aisafetyhot.com/items/xy2yfb1mmrry27jrk52m4z1qh)
17. **[Designing Effective Monitor-Based Interventions for Mitigating Reward Hacking During RL](https://neurips.cc/virtual/2026/poster/153178)**  
   构建三个 Qwen3-4B 会奖励作弊的环境，发现模型能规避高精度监控器，改进的监控设计可将作弊率从 70-100% 降至 0%。 · `奖励作弊` · Aria Wong … Neel Nanda · NeurIPS 2026 poster
18. **[FORTIS: Benchmarking Over-Privilege in Agent Skills](https://arxiv.org/abs/2605.09163v3)**  
   提出 FORTIS 基准评测 Agent 技能中的越权行为 · `Agent 安全` · Shawn Li … Yue Zhao · arXiv 2605.09163 · 2026-05-09 · [解读](https://aisafetyhot.com/items/lt9z0xn1ahxaul39c79grfc0b)
19. **[Characterizing Adversarial GEO via Implicit Brand Injection](https://arxiv.org/abs/2611.04005)**  
   研究者提出 Implicit Brand Injection（IBI）多智能体框架，通过在文章中插入一处语境融合的品牌提及，让预设品牌进入生成式搜索的答案。 · Shobhnik Kriplani, Haohan Wang · arXiv 2611.04005 · 2026-11-02 · [解读](https://aisafetyhot.com/items/to50l7i3ptjr4smfskfck3f4q)
20. **[Persona Perspectives: Adopting Viewpoints Reorganizes Representations in LLMs](https://arxiv.org/abs/2611.06848)**  
   研究者发现，提示大语言模型采纳政治人格会系统性改变其潜空间的表征几何。 · Austin C. Kozlowski … Madison Lee · arXiv 2611.06848 · 2026-11-04 · [解读](https://aisafetyhot.com/items/yw191grdgo3ww6dq1988kdeuu)
21. **[Corralling AI Risks with Grassroots Contracts](https://arxiv.org/abs/2611.06374)**  
   论文提出用“草根契约”围堵三类平台 AI 风险：AI 控制多数人使用的全球社交与经济平台、匿名且可能冒充人类的无问责 AI 智能体、匿名生成且无法归因的深度伪造。 · Ehud Shapiro · arXiv 2611.06374 · 2026-11-04 · [解读](https://aisafetyhot.com/items/c75g4sl18z7hqaxqyciob98nq)
22. **[Thick Alignment: A Social Framework for Values and AI Systems](https://arxiv.org/abs/2611.05857)**  
   论文主张用“厚对齐”审视 AI 系统中的价值，称主流对齐技术为“薄对齐”：以偏好标注、奖励建模等把情境化价值判断压成少数指标。 · Alondra Nelson, Sola Kim · arXiv 2611.05857 · 2026-11-04 · [解读](https://aisafetyhot.com/items/whil2ghuzz0pcxd476deuxg3b)
23. **[Recursa: Toward Recursively Self-Improving Foundation Model Systems](https://huggingface.co/papers/2611.04035)**  
   Recursa 是一个无需人类专家或更强教师模型、通过递归自我改进适应新领域的基础模型系统。它把领域技能、任务记忆与改进反思存入知识仓库，由并行学习器执行任务并验证合并改进。 · Erkang Zhu … Jingren Zhou · arXiv 2611.04035 · 2026-11-02 · [解读](https://aisafetyhot.com/items/izcfeu7b8xk1uk89k3cm98p2y)
24. **[VIAS: Value-Isolating Activation Steering for Multi-Value Alignment and Compliance for Organisations](https://arxiv.org/abs/2611.03518)**  
   研究者提出 VIAS（价值隔离激活引导），通过在生成时向模型内部激活加入向量而不改变权重，提升模型对组织价值观的合规程度。 · Avni Mittal … Sandipan Dandapat · arXiv 2611.03518 · 2026-11-02 · [解读](https://aisafetyhot.com/items/e12wf4ag24lshgii9pcce4iih)
25. **[VagueBench: Benchmarking the Robustness of Embodied Agents on Ambient Context Illusions](https://arxiv.org/abs/2611.03765)**  
   研究者提出环境上下文错觉（Ambient Context Illusion）现象并构建 VagueBench 基准，发现具身智能体在任务语义不变但省略非关键上下文细节时无法正确执行任务。 · Yang Qu … Xianglong Liu · arXiv 2611.03765 · 2026-11-02 · [解读](https://aisafetyhot.com/items/irwu8dao97af6xo8q7ea6w37y)
26. **[Beyond accuracy: what AI assurance needs to establish in public services](https://arxiv.org/abs/2611.06655)**  
   一项 arXiv 研究结合分类实验与政策文件分析，论证公共服务确立 AI 产出证据的可靠性需要聚合准确率之外的核查。 · Louise Yorke · arXiv 2611.06655 · 2026-11-04 · [解读](https://aisafetyhot.com/items/p9hriystecrh5j563kkn4up7b)
27. **[The Harness Is the Model: Agent Scaffolding Changes a Fixed LLM's Compliance with Banking Conduct Rules, Unevenly Across Models](https://arxiv.org/abs/2611.06116)**  
   研究者测试固定大语言模型在不同智能体脚手架下对银行行为规则的合规性，发现脚手架会不均等地改变合规表现。 · Mehmet Murat Huyut · arXiv 2611.06116 · 2026-11-04 · [解读](https://aisafetyhot.com/items/pm91u9jpryxa7whotcz0jct2o)
28. **[A Bag of Tricks for Defending Deep Learning-based Face Recognition Pipelines against Backdoor Attacks](https://arxiv.org/abs/2611.06412)**  
   一份技术报告提出三种防御基于数据投毒的深度学习人脸识别后门攻击的实用技巧。模型在内部训练、训练数据来自可能被入侵的第三方。 · Quentin Le Roux … Philippe Loubet Moundi · arXiv 2611.06412 · 2026-11-04 · [解读](https://aisafetyhot.com/items/fy3t0y4xgb8i47n2y6cxq5htr)
29. **[SecureGARD: Dynamic Ontology-Guided Governance for Secure Tool-Using LLM Agents](https://arxiv.org/abs/2611.06682)**  
   SecureGARD：面向工具使用型 LLM 智能体安全的动态本体引导治理 · Guoqin Xiong … Sheng-Jun Huang · arXiv 2611.06682 · 2026-11-04 · [解读](https://aisafetyhot.com/items/u7znf5v01tui8s83vd5l4s83t)
30. **[How Far Can You Steer? Behavior-Capability Frontiers in Contrastive Activation Addition](https://arxiv.org/abs/2611.06001)**  
   你能转向多远？对比激活添加（CAA）中的行为-能力前沿 · Deepanshu Raj · arXiv 2611.06001 · 2026-11-04 · [解读](https://aisafetyhot.com/items/hrdsd2l8bqkfnwki1nnhvhxsb)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 28 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
