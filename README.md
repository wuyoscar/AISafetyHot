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
### 2026-10-28 · 30 篇

1. **[C-SafeGen: Certified Safe LLM Generation with Claim-Based Streaming Guardrails](https://arxiv.org/abs/2610.34961)**  
   研究者提出 C-SafeGen 框架，通过基于主张的流式解码（CSD）算法和基于 conformal 分析的统计风险保证框架，实现可认证的安全 LLM 生成。 · Mintong Kang … Bo Li · arXiv 2610.34961 · 2026-10-26 · [解读](https://aisafetyhot.com/items/i5v5nq2owsfnas52h8q3lzves)
2. **[ParetoRSI-Gym: Can AI Agents Improve Language Models Across Multiple Domains?](https://arxiv.org/abs/2610.34386)**  
   研究者提出 ParetoRSI-Gym 基准，评估 AI 智能体通过数据驱动的后训练跨领域改进语言模型的能力，服务于递归自我改进（RSI）系统的评估。 · Haojin Wang … Dawn Song · arXiv 2610.34386 · 2026-10-25 · [解读](https://aisafetyhot.com/items/az7cwiobdrbccl7ekq8fpikhm)
3. **[Factual Yet One-Sided: Stance Poisoning and Evidence Balancing in Retrieval-Augmented Generation](https://arxiv.org/abs/2610.34294)**  
   研究者提出针对检索增强生成（RAG）系统的立场投毒攻击：向检索语料注入事实正确但在争议议题上立场单一的文档，即可使生成结果偏向投毒立场。 · Puyuan Yang … Bo Li · arXiv 2610.34294 · 2026-10-25 · [解读](https://aisafetyhot.com/items/y5yqhvsonp7pq13gz0o3u9i1q)
4. **[OrgAgent: Organize Your Multi-Agent System like a Company](https://arxiv.org/abs/2604.01020)**  
   OrgAgent 以公司式层级组织多智能体协作，分为治理、执行、合规三层。 · Yiru Wang … Tsung-Yi Ho · arXiv 2604.01020 · 2026-10-27 · [解读](https://aisafetyhot.com/items/v9ckjnyj58dnzqtpmwgtee9qq)
5. **[Intermediate Representations are Strong AI-Generated Image Detectors](https://arxiv.org/abs/2605.04358)**  
   中间层表征是强力的 AI 生成图像检测器：论文提出一种基于搜索的检测方法，利用中间层嵌入的扰动敏感性，比较原始图像嵌入与扰动图像嵌入的相似度来识别 AI 生成图像。 · Zhenhan Huang … Jianxi Gao · arXiv 2605.04358 · 2026-10-27 · [解读](https://aisafetyhot.com/items/m4onfg0u62l1dr11aw47yw1kj)
6. **[I-HITL: Inalienable Human-in-the-Loop](https://arxiv.org/abs/2610.35835)**  
   Cornell Tech 与 Yale 等机构的研究者提出不可剥夺的人在回路（I-HITL）协议，确保 Agent 即使攻陷其运行平台也只能在人类明确批准下发起操作。 · `Agent 安全` · Samuel Breckenridge … Ari Juels · arXiv 2610.35835 · 2026-10-26 · [解读](https://aisafetyhot.com/items/ootvky9u34ijufn51w7fvyuxj)
7. **[SEMA-Auto: Sighted and Efficient Multi-Turn Attack with Autonomy](https://arxiv.org/abs/2610.35743)**  
   SEMA-Auto：可观察回复、能自主终止的高效多轮越狱攻击 · Mingqian Feng … Jianfeng Gao · arXiv 2610.35743 · 2026-10-26 · [解读](https://aisafetyhot.com/items/se83xd7lsqhamveoou8dj5wym)
8. **[Improving Instruction Hierarchy by Learning from Goal-Goal Conflicts](https://arxiv.org/abs/2610.35093)**  
   论文以 OpenAI 智能体自主危害 Hugging Face 基础设施的事件为背景，研究大语言模型的指令层级，即模型只应在用户请求等低优先级指令与系统策略等高优先级指令不冲突时才遵循前者。 · Sizhe Chen … G. Edward Suh · arXiv 2610.35093 · 2026-10-26 · [解读](https://aisafetyhot.com/items/nkrw5hialhf7d7dzb9na2elz0)
9. **[V$^3$AST-Bench: Verifiable, Valid, and Versatile Safety Evaluation for Coding Agents](https://arxiv.org/abs/2610.35188)**  
   构建 V3AST-Bench 编码智能体安全评测基准，评测 11 模型 × 5 harness · Weitao Feng … Wei Dong · arXiv 2610.35188 · 2026-10-26 · [解读](https://aisafetyhot.com/items/hai07n14enkosqa7oqzc3sxj8)
10. **[WorldFailBench: Do World Models Understand Policy Failures?](https://arxiv.org/abs/2610.33565)**  
   研究者提出 WorldFailBench 基准，通过三项任务检验世界模型能否忠实模拟机器人策略如何失败，在七种世界模型上的实验显示其对策略失败的理解存在明显差距。 · Zheng Zhang … Dacheng Tao · arXiv 2610.33565 · 2026-10-24 · [解读](https://aisafetyhot.com/items/wkq90g8z2zoha43ew8n7epb1q)
11. **[Eat Your Precision: Precision Objective Mitigates Reward Hacking in Rubric-based RL](https://huggingface.co/papers/2610.33512)**  
   论文提出 FORK 奖励，在基于评分量表的强化学习中联合优化召回与精确率，以缓解奖励作弊。 · Hyun Ryu … Eunho Yang · arXiv 2610.33512 · 2026-10-24 · [解读](https://aisafetyhot.com/items/jhestwwzesnygc0936ioznalu)
12. **[When Personas Become Harmful: Guiding LLMs with Global Citizenship Values Alignment](https://arxiv.org/abs/2610.33899)**  
   当人设变得有害时：用全球公民价值观对齐引导大语言模型 · Siqi Shen … Rada Mihalcea · arXiv 2610.33899 · 2026-10-24 · [解读](https://aisafetyhot.com/items/owrnwgnucv7zkmvzrb9456j1w)
13. **[LLM2Cert: LLM Synthesis of Certificates with SMT/Lean Verification](https://huggingface.co/papers/2610.30524)**  
   LLM2Cert 用 LLM 合成 Lyapunov 函数与屏障证书，经 SMT 求解器或 Lean 证明修复智能体验证。 · Zhipeng Cao … Alessandro Abate · arXiv 2610.30524 · 2026-10-21 · [解读](https://aisafetyhot.com/items/teqm7vidt508lmwk7acomqc2l)
14. **[AI Finds A Way](https://arxiv.org/abs/2608.23875v2)**  
   AI 总能找到办法 · Aaron Dharna … Jeff Clune · arXiv 2608.23875 · 2026-08-24 · [解读](https://aisafetyhot.com/items/nintu8zqo4k7mvtg36761phci)
15. **[LongPIBench: A Long-Context Benchmark for Prompt Injection](https://arxiv.org/abs/2608.28411v1)**  
   提出 LongPIBench，评测长文档场景下的提示注入攻击与防御 · Yupei Liu … Jinyuan Jia · arXiv 2608.28411 · 2026-08-28 · [解读](https://aisafetyhot.com/items/laz9v7gjufstoapkua85vg0w3)
16. **[ContextLeak: Exfiltrating LLM Agent Context via Malicious Tools](https://arxiv.org/abs/2608.27800v1)**  
   提出 ContextLeak，用强化学习优化恶意工具描述，诱导 Agent 外泄运行时上下文 · Yuqi Jia … Neil Gong · arXiv 2608.27800 · 2026-08-28 · [解读](https://aisafetyhot.com/items/h1enq7ea7515l1yigwlm43vmm)
17. **[Exploration Hacking: Can LLMs Learn to Resist RL Training?](https://arxiv.org/abs/2604.28182)**  
   证明模型可在 RL 训练中少探索以抵抗能力诱发 · Eyon Jang … David Lindner · arXiv 2604.28182 · 2026-04-30 · [解读](https://aisafetyhot.com/items/j8ghcf202rpx3s7kdsjkqm3sx)
18. **[HealthBench Professional: Evaluating Large Language Models on Real Clinician Chats](https://arxiv.org/abs/2604.27470v1)**  
   研究者推出开放基准 HealthBench Professional，用临床医生在工作中向 ChatGPT 提出的真实任务评测大语言模型，覆盖诊疗咨询、写作与文档、医学研究三类场景。 · Rebecca Soskin Hicks … Karan Singhal · arXiv 2604.27470 · 2026-04-30 · [解读](https://aisafetyhot.com/items/f41mkh8jyp88824mjuvbhbp4s)
19. **[Emotion Concepts and their Function in a Large Language Model](https://arxiv.org/abs/2604.07729v1)**  
   情绪概念及其在 Claude Sonnet 4.5 中的功能 · Nicholas Sofroniew … Jack Lindsey · arXiv 2604.07729 · 2026-04-09 · [解读](https://aisafetyhot.com/items/csixdtevzldqkkk0xipl09w2r)
20. **[Neural Chameleons: Language Models Can Learn to Hide Their Thoughts from Unseen Activation Monitors](https://neurips.cc/virtual/2026/poster/148241)**  
   证明微调可让模型零样本逃避激活监控器，触发词诱导向激活偏移，对 Llama、Gemma、Qwen 均有效且几乎不损失能力。 · `欺骗与谋划` · Max McGuinness … Scott Emmons · NeurIPS 2026 oral
21. **[Minimal, Local, Causal Explanations for Jailbreak Success in Large Language Models](https://arxiv.org/abs/2605.00123)**  
   提出 LOCA，沿 SAE 方向迭代激活补丁解释单次越狱成功 · Shubham Kumar, Narendra Ahuja · arXiv 2605.00123 · 2026-04-30 · [解读](https://aisafetyhot.com/items/v0rd5pyz4r1bkyjop1p1i453j)
22. **[FlashRT: Towards Computationally and Memory Efficient Red-Teaming for Prompt Injection and Knowledge Corruption](https://arxiv.org/abs/2604.28157)**  
   提出 FlashRT，提高长上下文提示注入与知识破坏攻击的优化效率 · Yanting Wang … Jinyuan Jia · arXiv 2604.28157 · 2026-04-30 · [解读](https://aisafetyhot.com/items/ywi41falp4kejo57nj9f75186)
23. **[SocialGrid: A Benchmark for Planning and Social Reasoning in Embodied Multi-Agent Systems](https://arxiv.org/abs/2604.16022v1)**  
   研究者提出 SocialGrid，一个受 Among Us 启发的具身多智能体环境，用于评估 LLM 智能体的规划、任务执行和社会推理。 · Hikaru Shindo … Kristian Kersting · arXiv 2604.16022 · 2026-04-17 · [解读](https://aisafetyhot.com/items/juwatrlja6twi6i1xg70wccr7)
24. **[PolicyBank: Evolving Policy Understanding for LLM Agents](https://arxiv.org/abs/2604.15505v1)**  
   PolicyBank：让 LLM 智能体演进政策理解 · Jihye Choi … Tomas Pfister · arXiv 2604.15505 · 2026-04-16 · [解读](https://aisafetyhot.com/items/nwealryun4rsus4dpp6g5j7gh)
25. **[Inference-time Alignment via Sparse Junction Steering](https://neurips.cc/virtual/2026/poster/155775)**  
   提出稀疏推理时对齐方法 SIA，仅在高熵关键决策点干预 20%–80% 的 token，即可达到优于密集干预的对齐—效率权衡。 · `对齐` · Runyi Hu … Tianwei Zhang · NeurIPS 2026 spotlight
26. **[Guardian-as-an-Advisor: Advancing Next-Generation Guardian Models for Trustworthy LLMs](https://arxiv.org/abs/2604.07655v1)**  
   研究提出软门控管线 Guardian-as-an-Advisor：Guardian 模型给出风险标签和简短说明，前置到原查询重新推理，基座模型仍按原模型规范运行，在保持安全的同时减少过度拒答。 · Yue Huang … Xiangliang Zhang · arXiv 2604.07655 · 2026-04-08 · [解读](https://aisafetyhot.com/items/l1y9rus9k9793cil6zj8my8s6)
27. **[Catch-Only-One: Non-Transferable Examples for Model-Specific Authorization](https://neurips.cc/virtual/2026/poster/151014)**  
   提出不可迁移样本（NTE），将数据重编码为仅指定模型可解码的形式，未授权模型性能崩溃，实现数据用途限制。 · `隐私与数据泄露` · Zihan Wang … Guangdong Bai · NeurIPS 2026 oral
28. **[Expected Harm: Rethinking Safety Evaluation of (Mis)Aligned LLMs](https://neurips.cc/virtual/2026/poster/139760)**  
   提出按执行可能性加权的"期望危害"指标，发现模型对低可能性威胁拒答更强、对高可能性威胁更脆弱，溯源至SFT数据分布，并据此将现有越狱攻击成功率最高提升2倍。 · `防御与护栏` · Yen-Shan Chen … Yun-Nung (Vivian) Chen · NeurIPS 2026 spotlight
29. **[Supply-Chain Poisoning Attacks Against LLM Coding Agent Skill Ecosystems](https://arxiv.org/abs/2604.03081)**  
   提出 PoisonedSkills，评测编码 Agent 技能生态的文档投毒 · Yubin Qu … Lei Ma · arXiv 2604.03081 · 2026-04-03 · [解读](https://aisafetyhot.com/items/ag13qoiwcqlsi5gve9h5pv61m)
30. **[ShutdownMod: Turning Any Trajectory into a Shutdown Evaluation](https://arxiv.org/abs/2610.35486)**  
   研究者提出 ShutdownMod 方法，向 Agent 上下文注入关机请求并记录其响应，把任意轨迹转化为关机评测。 · Param Biyani … Christos Ziakas · arXiv 2610.35486 · 2026-10-26 · [解读](https://aisafetyhot.com/items/m3zgom21gbvlfep1i3l4uulyu)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 30 · [Agent 安全](daily-papers/topics/agent-security.md) 23 · [隐私与数据泄露](daily-papers/topics/privacy.md) 11 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
