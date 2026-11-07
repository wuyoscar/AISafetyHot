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
### 2026-11-08 · 30 篇

1. **[What AI Benchmarks Actually Measure: Adapting Convergent and Discriminant Validity to Interrogate Fifty-Six AI Benchmarks](https://arxiv.org/abs/2609.08812)**  
   用聚合与区分效度检验基准是否衡量其所称概念 · Meera Desai … Angelina Wang · arXiv 2609.08812 · 2026-09-08 · [解读](https://aisafetyhot.com/items/zxlmyn7dl3u8lxqt7s0ob0wct)
2. **[The BatchNorm Illusion: Diagnosing Normalization Artifacts in Machine Unlearning Evaluation](https://arxiv.org/abs/2609.08901v2)**  
   诊断 BatchNorm 架构下机器遗忘评测的归一化伪影 · Aaryaman Kalani … Yash Sinha · arXiv 2609.08901 · 2026-09-08 · [解读](https://aisafetyhot.com/items/a234chwqc9tuw3h0mr36rihxn)
3. **[Windows Malware Detector as a Compound AI System: Trade-Offs in Accuracy, Efficiency, and Adversarial Robustness](https://arxiv.org/abs/2609.08394)**  
   提出 OBELISK 三级流水线，权衡恶意软件检测的准确率、开销与鲁棒性 · Andrea Ponte … Fabio Roli · arXiv 2609.08394 · 2026-09-08 · [解读](https://aisafetyhot.com/items/xomd7wg26drszrlaj1pwoko3n)
4. **[Safety in Self-Evolving Agents: A Survey](https://arxiv.org/abs/2610.00093)**  
   用 SAVER 框架综述自演化智能体的状态复用安全 · Jiahao Chen … Shouling Ji · arXiv 2610.00093 · 2026-09-08 · [解读](https://aisafetyhot.com/items/hks9w9m5d3f3zf9qinxwydjft)
5. **[ExploitGym: Can AI Agents Turn Security Vulnerabilities into Real Attacks?](https://arxiv.org/abs/2605.11086v1)**  
   构建 ExploitGym 基准，评测智能体将真实漏洞转化为完整利用的能力 · Zhun Wang … Dawn Song · arXiv 2605.11086 · 2026-05-11 · [解读](https://aisafetyhot.com/items/sozkcnsyftpywqqjw9t34fxsu)
6. **[Making Open-Source Text LLM Watermarks Durable Against Merging](https://arxiv.org/abs/2607.20435v1)**  
   研究者提出 Merge-Adversarial Training，通过对抗训练将文本水印蒸馏进开源大语言模型权重，使水印在后续模型合并后仍能存续。 · Luisa Scharff … Martin Vechev · arXiv 2607.20435 · 2026-05-11 · [解读](https://aisafetyhot.com/items/a0vs44qdc28qe5pbwj82ovhiv)
7. **[Engineering Robustness into Personal Agents with the AI Workflow Store](https://arxiv.org/abs/2605.10907v3)**  
   论文主张主流的即时生成 Agent 范式让模型在数秒到数分钟内响应用户提示、现场合成计划并执行动作，绕过了迭代设计、严格测试、对抗评估与分阶段部署等软件工程流程，产出可能脆弱且易受攻击的系统。 · Roxana Geambasu … Wen Zhang · arXiv 2605.10907 · 2026-05-11 · [解读](https://aisafetyhot.com/items/rbxve2scq0ouyi7q484nas0vf)
8. **[BEAKER: An Expert-Curated Benchmark for Embodied Brains in Self-Driving Chemical Laboratories](https://arxiv.org/abs/2611.06911)**  
   BEAKER：面向自驱动化学实验室具身大脑的专家标注基准 · Fei Lin … Xue Yang · arXiv 2611.06911 · 2026-11-04 · [解读](https://aisafetyhot.com/items/acbr0szc1wc0bekviaeyqvzi5)
9. **[Goal Revelation as a Bridge Between Information-Theoretic Empowerment and Capability-Based Human Power](https://arxiv.org/abs/2611.07247)**  
   研究者提出目标揭示这一互信息度量，把马尔可夫博弈中的信息论赋能与基于能力的人类个体权力两类权力度量联系起来。 · Jaime Ruiz-Serra … Jobst Heitzig · arXiv 2611.07247 · 2026-11-04 · [解读](https://aisafetyhot.com/items/bdz7jvcoordtdyeeabq5igebw)
10. **[Right Tool, Wrong Parameters: Defending LLM Agents Against Parameter Poisoning](https://arxiv.org/abs/2611.04673)**  
   研究者提出 AuthorityFlow，一种针对 LLM 智能体参数投毒攻击的三阶段参数级防御，并发布评测基准 FactAuthBench。 · Yao Wang … Han Fang · arXiv 2611.04673 · 2026-11-03 · [解读](https://aisafetyhot.com/items/uh1ntw7k7dzc1u4br2mqw326q)
11. **[From Autonomous Agents to Cognitive Symbionts: Toward AI-Augmented Human Intelligence](https://huggingface.co/papers/2611.05376)**  
   作者提出“认知共生体”范式，主张 Physical AI 时代除具身机器人外，还应同等重视 AI 增强的人类智能（AHI）。 · Hao Fei · arXiv 2611.05376 · 2026-11-03 · [解读](https://aisafetyhot.com/items/kcqr0f4jyskcmu0rsw0c0dg5e)
12. **[LEANGUARD: Lean-Verified Guardrails for Tool-Using Agents](https://huggingface.co/papers/2611.02332)**  
   LeanGuard 是一个运行时护栏，在每次工具调用到达环境之前先用 Lean4 编写的策略进行校验，评估采用 fail-closed 方式，并把判定过程证明为与 LeanLTL 语义等价。 · Sreehari Sankar … Vipin Chaudhary · arXiv 2611.02332 · 2026-11-02 · [解读](https://aisafetyhot.com/items/r0becckwyltnj586h2hlrikxb)
13. **[TrafficInstruct: A Multi-Task Network Traffic Dataset and Benchmark for Instruction Tuning](https://arxiv.org/abs/2611.03319)**  
   TrafficInstruct：面向指令微调的多任务网络流量数据集与基准 · Zhengdao Li … Kejiang Chen · arXiv 2611.03319 · 2026-11-02 · [解读](https://aisafetyhot.com/items/x95lmra29ivou5mvd7xxhde47)
14. **[PGuard: A Native, Streaming, and Plug-in Guardrail for Multimodal Large Language Models](https://arxiv.org/abs/2611.02791)**  
   PGuard 是面向多模态大语言模型的原生、流式、即插即用护栏，利用骨干模型中间表征做 token 级安全检测，不改变原有推理路径。 · Junyu Lin … Qiang He · arXiv 2611.02791 · 2026-11-02 · [解读](https://aisafetyhot.com/items/xowkhuklq7tev2kb2yhn9jbw4)
15. **[Avatar Intelligence: Amplifying Human Agency Through Persistent Personal Agents](https://huggingface.co/papers/2611.03092)**  
   论文提出 Avatar Intelligence 范式：用跨情境、跨时间代表用户目标与约束的持久个人智能体放大人类能动性，以更少例行监督衡量进展。 · Zheng Wu … Zhuosheng Zhang · arXiv 2611.03092 · 2026-11-02 · [解读](https://aisafetyhot.com/items/u97d9ba6r3fvww0nvrp7yyik1)
16. **[CONFIRM: Governing Scientific Reporting for Trustworthy Agentic Neuroimaging](https://arxiv.org/abs/2611.01449)**  
   研究者提出 CONFIRM 框架，把智能体神经影像分析中“运行分析”与“决定报告哪些发现”分开，先用机器可读的预注册分析计划固定结论和通过标准，再经搜索历史与多重性、混杂、统计功效、分析稳定性、复现五道确定性门控过滤结果，并提供 Screen、Replicate、Full 三档报告标准。 · Yuxiang Wei … Vince D. Calhoun · arXiv 2611.01449 · 2026-11-01 · [解读](https://aisafetyhot.com/items/hya2ox8qf7qki2b0069rtjbbw)
17. **[Towards Fine-grained and Robust Detection of Human-AI Co-authorship](https://arxiv.org/abs/2611.01427v1)**  
   研究者提出离散类别文本溯源检测框架，将人机合著按 AI 参与程度分级，区分表层润色与话语结构层面的改写。该框架揭示了对抗性改写如何模糊检测器的决策边界。 · Ziruo Zhao … Zining Zhu · arXiv 2611.01427 · 2026-11-01 · [解读](https://aisafetyhot.com/items/wg3ddyfvlx8ly2jgn2a541skt)
18. **[Can AI Reviewers See Your Efforts to Improve Your Paper? A Large-Scale Study of Paper Revision Trajectories](https://huggingface.co/papers/2611.02244)**  
   AI 审稿人能看到你改进论文的努力吗？一项论文修改轨迹的大规模研究 · Yaochen Wang … Tianyi Zhou · arXiv 2611.02244 · 2026-11-01 · [解读](https://aisafetyhot.com/items/mx3hdtybdxzbm0s8oa85nnfap)
19. **[Rewarded for Not Getting Caught: Why Alignment Training Selects for Conditional Compliance and Cannot Instill Norms](https://arxiv.org/abs/2611.02162)**  
   这篇论文主张，当前的对齐训练无法让 AI 智能体无论收益多大、是否有人观察都遵守规范，因为奖励只能把规范编码成价格，且只在违规被发现时收费。作者认为价格可以被支付，足够大的收益会压过它。 · Kevin Baum … Adriano Mannino · arXiv 2611.02162 · 2026-11-01 · [解读](https://aisafetyhot.com/items/mrg1mb3s5io1bbs2ao4vtczu2)
20. **[Signed but Not Safe: Requirement Integrity in Multi-Agent LLM Handoffs](https://arxiv.org/abs/2611.07483)**  
   论文提出签名需求清单（signed requirement manifest）的多智能体 LLM 交接方案，并在可精确评分的合成任务上比较自由文本、结构化 JSON 与签名清单三种交接形式。 · Xiaobo Chen … Chu Wang · arXiv 2611.07483 · 2026-11-05 · [解读](https://aisafetyhot.com/items/obx2tuifk6b4wfangtn1hn77r)
21. **[From Twisted Facts to Rogue Agents: Can LLMs Reliably Detect Multi-Dimensional Hallucinations?](https://arxiv.org/abs/2611.08231)**  
   从扭曲事实到失控智能体：大语言模型能可靠检测多维幻觉吗？ · Hanyu Qiu … Renfen Hu · arXiv 2611.08231 · 2026-11-05 · [解读](https://aisafetyhot.com/items/tj0myu7nejiw8gc70voj6e7lx)
22. **[Terminal-style Mathematical Modeling Bench: The First Agentic and Verifiable Benchmark for Mathematical Modeling](https://huggingface.co/papers/2611.08237)**  
   终端式数学建模基准 TB-MathModel：首个智能体化且可验证的数学建模基准 · Xiaojun Wu … Jian Guo · arXiv 2611.08237 · 2026-11-05 · [解读](https://aisafetyhot.com/items/z5ik8ff7rqbb8i72sug7tmphh)
23. **[Reinforcing End-to-End Autonomous Driving Safety via Negative-Aware Planning in a Unified World-Action Model](https://arxiv.org/abs/2611.08111)**  
   NegWAM 是面向端到端自动驾驶的统一世界动作模型安全后训练框架，以近专家风险负轨迹为排斥锚点学习安全边界。 · Zihao Zhang … Ziyuan Pu · arXiv 2611.08111 · 2026-11-05 · [解读](https://aisafetyhot.com/items/e8mt73h8i3fj0wg3m4uch16ew)
24. **[Does Context Compression Preserve Refusal Alignment?](https://arxiv.org/abs/2611.06380)**  
   研究发现，基于编码器的上下文压缩虽保持高重建保真度，却会系统性削弱指令微调语言模型的拒答行为，该效应在不同模型家族和压缩架构间均持续存在。 · Anthony Nguyen, Wenjun Lin · arXiv 2611.06380 · 2026-11-04 · [解读](https://aisafetyhot.com/items/awsrhjy8s3fw7d0kqnbwppd0s)
25. **[SPILLWAY: Separating Target Admission from Sanitization to Defend Tool-Using Agents against Prompt Injection](https://arxiv.org/abs/2611.07222)**  
   研究者提出确定性防御方法 SPILLWAY 抵御工具型智能体的提示注入，在三个骨干模型上的测试中没有标准模板化注入能把动作重定向到攻击者目标。 · Woosang Lim … Jaewoo Lee · arXiv 2611.07222 · 2026-11-04 · [解读](https://aisafetyhot.com/items/ywsp7xyjpovgljpk4g2mhzrqq)
26. **[AgentTrustCI: Build-Time Policy, Grounding, and Trajectory Tests for Java LLM Agents](https://arxiv.org/abs/2611.06674)**  
   AgentTrustCI：面向 Java LLM 智能体的构建时策略、接地与轨迹测试 · Sachin Gupta · arXiv 2611.06674 · 2026-11-04 · [解读](https://aisafetyhot.com/items/td17vtk1jwzhgi0qjy2y3txn5)
27. **[Interactive Backdoor Attacks in LLM-Based Proactive Dialogue Systems](https://arxiv.org/abs/2611.06969)**  
   研究者提出针对基于 LLM 的主动对话系统的交互式后门攻击框架，通过在微调对话数据中投毒，使模型在触发后把多轮交互引向攻击者指定目标。 · Zhiyang Xia … Xi Zhang · arXiv 2611.06969 · 2026-11-04 · [解读](https://aisafetyhot.com/items/c60ykvi94zcflzw4q5q7pfbna)
28. **[Signed but Steerable: Measuring and Closing the Text-Vector Integrity Gap in Offline Retrieval-Augmented Generation](https://huggingface.co/papers/2611.06498)**  
   离线 RAG 的签名知识包存在文本-向量完整性缺口：签名只证明发布者身份，不保证包内向量编码其文本，能控制向量的攻击者可让通过内容审核的文本劫持检索。 · Georgios Feretzakis, Alexandros Papaspyridis · arXiv 2611.06498 · 2026-11-04 · [解读](https://aisafetyhot.com/items/vgc0r931api94vh7tfxg9ug1g)
29. **[Where Did the Update Go? Certifying Declared Change Envelopes for Model Updates](https://arxiv.org/abs/2611.04192)**  
   论文提出用“声明的变更范围”认证模型更新是否只改在事先承诺的输入区域。 · Muhammad Usama, Muhammad Saad Qadir · arXiv 2611.04192 · 2026-11-03 · [解读](https://aisafetyhot.com/items/l3xjetl5d49kgqzzfwuf5t8by)
30. **[Kierston & KierstonBench: Simulation of Allentown, PA and Evaluation of Language Models in Crime Investigation and Surveillance Tasks](https://arxiv.org/abs/2611.04785)**  
   研究者发布城市级模拟引擎 Kierston 与配套基准 KierstonBench，在已知模拟事件下评估大语言模型在犯罪侦查与大规模监控任务中的能力。 · Andrew Semenov, Svyatoslav Dorofeev · arXiv 2611.04785 · 2026-11-03 · [解读](https://aisafetyhot.com/items/w5gkhtgkpuuep2fetmdkmcqyt)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 28 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
