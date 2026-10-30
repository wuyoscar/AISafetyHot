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
### 2026-10-31 · 30 篇

1. **[ShallowDefend: Harnessing Shallow Safety Alignment for Multi-Turn Defender](https://arxiv.org/abs/2610.40627)**  
   研究者提出 ShallowDefend 框架，让模型先给出显式、可解析的安全决策再生成回复，在两个模型家族、十四个基准的受控比较中取得最强的多轮安全表现。 · Qiyao Ma … Jianfeng Gao · arXiv 2610.40627 · 2026-10-29 · [解读](https://aisafetyhot.com/items/x0cnvbg5jfq5mycdt2y7587iw)
2. **[Where You Inject Matters: The Trust Region Effect in LLM Agents](https://arxiv.org/abs/2610.38867)**  
   微软研究院等机构的研究者系统测量了间接提示注入中注入位置对攻击效果的影响，提出信任区域效应，即智能体对环境不同区域隐式赋予不同信任。 · Chengquan Guo … Jianfeng Gao · arXiv 2610.38867 · 2026-10-28 · [解读](https://aisafetyhot.com/items/pi4p50z87o71rmvht38n1kk9i)
3. **[Aligning Autoresearch: Co-Improvement between Agents and Humans](https://arxiv.org/abs/2610.38882)**  
   研究者提出让自动研究智能体与人类协同改进（co-improvement）的对齐训练与评测方案。在基准创建领域的实证研究显示，人类在指导这类智能体时仍起关键作用，尤其在构思阶段。 · Tianjian Li … Jason Weston · arXiv 2610.38882 · 2026-10-28 · [解读](https://aisafetyhot.com/items/gr6m5kl50tbinjsc3xl7kz1eb)
4. **[Agentic Backdoors via Pretraining Poisoning](https://arxiv.org/abs/2610.37741)**  
   通过预训练投毒植入 Agent 后门 · Xinyan Hu … Yiming Zhang · arXiv 2610.37741 · 2026-10-27 · [解读](https://aisafetyhot.com/items/zhgqd7peh0n2ybxk57zmg86zh)
5. **[Efficient Scalable Oversight via Rewinding](https://arxiv.org/abs/2610.40535)**  
   研究者提出可回滚交互证明（RIP），一种面向可扩展监督的相对化交互证明新模型，让弱验证者核查更强 AI 系统执行的运算。 · Ziyi Guan … Zoe Xi · arXiv 2610.40535 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ipxbqeho2h416jhr7ztcs62vc)
6. **[Understanding and Mitigating Role Spoofing in LLMs](https://arxiv.org/abs/2610.40396)**  
   研究者提出并分析了针对大语言模型的“角色伪装”攻击：工具输出中的恶意文本（例如 Agent 访问的恶意网页）利用模型按文风而非标注角色判断说话来源的倾向冒充用户。 · Ezra Edelman … Eran Malach · arXiv 2610.40396 · 2026-10-29 · [解读](https://aisafetyhot.com/items/cftjbcuwtg5fiamld0yyoz82b)
7. **[SEAL: Sealed Queries for Local Sanitization against Indirect Prompt Injection](https://arxiv.org/abs/2610.39758)**  
   SEAL：用密封查询实现本地净化以对抗间接提示注入 · Doohyun Kim … Brent ByungHoon Kang · arXiv 2610.39758 · 2026-10-29 · [解读](https://aisafetyhot.com/items/gm4ulelcrxvf1fe5dhmz295xq)
8. **[HALO: Human-Grounded Granular Evaluation of Proactive Agents](https://arxiv.org/abs/2610.39086)**  
   研究者提出 HALO 基准，对主动智能体在无明确请求时是否、何时及以多大范围提供协助进行以人为本的细粒度评估。 · Wenqi Pei … Muhao Chen · arXiv 2610.39086 · 2026-10-29 · [解读](https://aisafetyhot.com/items/c6spyfyy4fukm6t7vti61mf4r)
9. **[Elucidating the Design Space of LM Data Attribution](https://arxiv.org/abs/2610.40655)**  
   研究者提出用于事实追踪的可控归因基准 CATT，在完全虚构的知识上微调语言模型，为数据归因提供无歧义真值，并以此系统考察语言模型数据归因的设计空间。 · Steven Yu … David Bau · arXiv 2610.40655 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ibrgrqi3y963df7xztegqx3xl)
10. **[Appreciation Teaches Unauthorized Execution: Self-Evolution Degrades the Robustness of Personal Agents to Indirect Prompt Injection](https://arxiv.org/abs/2610.39122)**  
   研究者发现，自我进化会显著削弱个人 Agent 对间接提示注入（IPI）的鲁棒性。 · Xinyan Wang … Chaowei Xiao · arXiv 2610.39122 · 2026-10-29 · [解读](https://aisafetyhot.com/items/nybmmg7y2auxygg7wtvp177wp)
11. **[Value Probes: Learned Value Functions for Beam-Search Red Teaming](https://arxiv.org/abs/2610.38526)**  
   Value Probes：用于束搜索红队测试的学习型价值函数 · Jonathan F. Jao, Andrew Kyle Lampinen · arXiv 2610.38526 · 2026-10-28 · [解读](https://aisafetyhot.com/items/id70v7jzc94cg54l2gy67fsua)
12. **[What Hallucinations Have We Measured? Semantic Illusion, Confabulation, and Expressed Uncertainty](https://arxiv.org/abs/2610.38520)**  
   研究者提出严格的幻觉定义，主张只把自信的错误回答称为幻觉，并与表达不确定性（UNK）区分开，因为幻觉不会像 UNK 那样提示模型可能出错，实践中更危险。 · Hazel H. Kim … Philip H. S. Torr · arXiv 2610.38520 · 2026-10-28 · [解读](https://aisafetyhot.com/items/vhbhowuyy8lp1woyex3rq91fz)
13. **[The Role of Quantization in Loss Spikes](https://arxiv.org/abs/2610.38277)**  
   研究者发现，语言模型预训练中延迟出现的终期发散（time-bomb spikes）出现前，LM head 的量化误差会快速增长并最终引发损失尖峰。降低数值精度会加速这类尖峰，提高精度则改善稳定性。 · Zaiqian Chen … Micah Goldblum · arXiv 2610.38277 · 2026-10-28 · [解读](https://aisafetyhot.com/items/i4npnjbgtahttcxiure2x0tqs)
14. **[RoleFUZZER: User-Behaviour Fuzzing for Role-Specification Adherence in Large Language Models](https://arxiv.org/abs/2610.38438)**  
   研究者提出 RoleFUZZER 框架，把软件测试中的覆盖导向模糊测试移植到大语言模型的角色规范遵循测试，通过搜索可能诱使模型违反角色规范的用户行为来发现漏洞。 · Kshitish Ghate … Aylin Caliskan · arXiv 2610.38438 · 2026-10-28 · [解读](https://aisafetyhot.com/items/cu8gjgjykiuiwvvcc4d0xf1l0)
15. **[Post-Training Large Language Models with LLMON](https://arxiv.org/abs/2610.38120)**  
   IBM Research 团队提出 LLMON（LLM Object Notation）后训练方法，用六个保留分隔符显式区分指令与数据，执行须通过引用标识符的执行块完成。 · Basel Shbita … Dan Gutfreund · arXiv 2610.38120 · 2026-10-28 · [解读](https://aisafetyhot.com/items/fmnvhc567dpx57hs0698012lk)
16. **[Context Inference Attacks Without Jailbreaks](https://arxiv.org/abs/2609.01663v1)**  
   穆罕默德·本·扎耶德人工智能大学（MBZUAI）研究者提出上下文推断攻击，攻击者仅凭不带对抗指令的良性查询，就能从响应分布中推断 Agent 隐藏上下文包含哪些记录，模型无需直接输出任何敏感内容。 · Prince Jha … Nils Lukas · arXiv 2609.01663 · 2026-08-31 · [解读](https://aisafetyhot.com/items/y546rqvqvw1jftdbkd77h09p0)
17. **[Validity-Aware Jailbreak Evaluation for Large Language Models](https://arxiv.org/abs/2609.00498v1)**  
   提出 SEAV，逐步核验越狱回复的事实与操作有效性 · Qilong Wu … Varun Chandrasekaran · arXiv 2609.00498 · 2026-08-31 · [解读](https://aisafetyhot.com/items/nklyegp2yx3hylcywi9unkqsy)
18. **[ECLIPSE: Self-Evolving Stealthy Prompt Injection Attack against Long-Horizon Agentic Systems](https://arxiv.org/abs/2608.30441v2)**  
   提出 ECLIPSE 双通道提示注入，劫持长程 Agent 的动作轨迹 · Shiqian Zhao … Luu Anh Tuan · arXiv 2608.30441 · 2026-08-31 · [解读](https://aisafetyhot.com/items/qaztgzcpuj9fy5pk555jn9yb6)
19. **[Distributed Implicit Harm: A Compositional Safety Blind Spot in MLLM-Based Video Moderation](https://arxiv.org/abs/2609.00206v1)**  
   构建分布式隐式有害视频数据集并评测多模态模型审核缺陷 · Ruotong Wang … Baoyuan Wu · arXiv 2609.00206 · 2026-08-31 · [解读](https://aisafetyhot.com/items/yfihxdur8gevs82vw9026j1ux)
20. **[VisER: Visual Evidence and Reliance for Object Hallucination Detection in LVLMs](https://arxiv.org/abs/2608.30480v1)**  
   提出 VisER，用内部视觉证据检测 LVLM 物体幻觉 · Afsaneh Hasanebrahimi … Sarah Erfani · arXiv 2608.30480 · 2026-08-31 · [解读](https://aisafetyhot.com/items/j9fb2m299znsrfpl46v6nfyk7)
21. **[AgentProv: Auditing Agentic LLM API Providers via Tool-use Policy Probes](https://arxiv.org/abs/2609.00052v1)**  
   研究者提出 AgentProv，通过模型的工具调用类别分布生成指纹，用 MMD 置换检验判定智能体 LLM API 背后部署的是否为宣称的基础模型，作者称这是首个基于动作的身份审计方法。 · Xun Wang … Adam Dziedzic · arXiv 2609.00052 · 2026-08-30 · [解读](https://aisafetyhot.com/items/bs6ngi7tozqreiafms4vquy6n)
22. **[Model Spec Midtraining: Improving How Alignment Training Generalizes](https://arxiv.org/abs/2605.02087v2)**  
   Anthropic 研究者提出 Model Spec 中期训练（MSM）：在预训练之后、对齐微调之前，用讨论 Model Spec 内容的合成文档训练模型，使其先掌握规范的内容与理由，再由后续示范数据引出对齐行为。 · Chloe Li … Jon Kutasov · arXiv 2605.02087 · 2026-05-03 · [解读](https://aisafetyhot.com/items/a0hbb17jzcj1q56nyey2djdu4)
23. **[Trojan Hippo Bench: A Dynamic Benchmark for Persistent Memory Attacks and Defenses in LLM Agents](https://arxiv.org/abs/2605.01970)**  
   构建 Trojan Hippo Bench，评测 Agent 持久记忆投毒与外泄 · Debeshee Das … David Wagner · arXiv 2605.01970 · 2026-05-03 · [解读](https://aisafetyhot.com/items/sl44mzze5yuij79npdhzqkxb2)
24. **[Safety Drift After Fine-Tuning: Evidence from High-Stakes Domains](https://arxiv.org/abs/2604.24902v1)**  
   大模型微调后的安全漂移：来自医疗与法律领域的证据 · Emaan Bilal Khan … Dylan Hadfield-Menell · arXiv 2604.24902 · 2026-04-27 · [解读](https://aisafetyhot.com/items/i8o2teo8dy7atvcvar94k64kb)
25. **[Securing Multimodal AI through Internal Information Decomposition](https://arxiv.org/abs/2607.21600v1)**  
   通过内部信息分解保障多模态 AI 安全 · Jehyeok Yeon … Heng Ji · arXiv 2607.21600 · 2026-05-03 · [解读](https://aisafetyhot.com/items/p4g8fm6vkjngzibfzzgtykvek)
26. **[From Stealthy Data Fabrication to Unsafe Driving: Realistic Scenario Attacks on Collaborative Perception](https://arxiv.org/abs/2605.01301v2)**  
   研究者提出一种针对网联自动驾驶汽车协同感知的隐蔽数据伪造攻击，不制造易被检测的大幅异常，而是细微篡改共享感知结果中已有目标的位姿，使扰动低于检测阈值，小误差经目标跟踪和轨迹预测等下游模块传播，最终诱发不安全驾驶决策。 · Qingzhao Zhang … Z. Morley Mao · arXiv 2605.01301 · 2026-05-02 · [解读](https://aisafetyhot.com/items/bydccavyib99vx57uy14i95vu)
27. **[Toward a Principled Framework for Agent Safety Measurement](https://arxiv.org/abs/2605.01644v1)**  
   论文提出 Agent 安全应由搜索而非采样来度量，并给出 BOA 框架，在 Agent 安全工作负载上发现了贪心和抽样评测漏掉的不安全轨迹。 · Shuyi Lin … Cheng Tan · arXiv 2605.01644 · 2026-05-02 · [解读](https://aisafetyhot.com/items/fymmen0e5ugq7iyis9qm70b8c)
28. **[I can't recognize (yet): Delayed Rendering to Defeat Visual Phishing Detectors](https://arxiv.org/abs/2605.00183v1)**  
   我还识别不出：延迟渲染可击败视觉钓鱼检测器 · Ying Yuan … Luigi Vincenzo Mancini · arXiv 2605.00183 · 2026-04-30 · [解读](https://aisafetyhot.com/items/fnu0212ff605p5z6euv0dagur)
29. **[Green Shielding: A User-Centric Approach Towards Trustworthy AI](https://arxiv.org/abs/2604.24700v1)**  
   论文提出 Green Shielding，一项以用户为中心的研究议程，通过刻画良性输入变化如何改变模型行为，为高风险场景构建有证据支撑的部署指导，并以 CUE 标准落地。 · Aaron J. Li … Bin Yu · arXiv 2604.24700 · 2026-04-27 · [解读](https://aisafetyhot.com/items/inysn5pnqs9z5so075vkx7u7v)
30. **[FlipJev: Fast Black-Box Red Teaming Finds Universal Adversarial Suffixes for Typed Decision Models](https://arxiv.org/abs/2610.38895)**  
   研究者提出 FlipJev，一种针对类型化决策模型（直接输出决策而非自由文本的语言模型）的快速黑盒查询攻击，不调用攻击者语言模型，在代表性模型 Jev 上几分钟内即可找到翻转高置信度答案的短后缀。 · Xiaogeng Liu … Chaowei Xiao · arXiv 2610.38895 · 2026-10-28 · [解读](https://aisafetyhot.com/items/dy143ofdi84y1lt6qj1lgmnjg)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 30 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [隐私与数据泄露](daily-papers/topics/privacy.md) 11 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
