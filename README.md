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
### 2026-11-11 · 30 篇

1. **[Scaling Adaptive Prompt Injection Attacks with Agent Swarms](https://arxiv.org/abs/2611.11861)**  
   研究者提出用智能体集群扩展自适应提示注入攻击，其新评测显示，能力更强的智能体攻击者可以可靠地诱导模型遵循工具输出中的指令，包括在 GraySwan Arena 等公开提示注入基准上被认为稳健的模型。 · Alexey Kurakin … Kamalika Chaudhuri · arXiv 2611.11861 · 2026-11-09 · [解读](https://aisafetyhot.com/items/smovvsnzk5dfjxdthk5yjors8)
2. **[ML Models Are Not Ciphers: Power Analysis for Weight Extraction Is Harder Than You Think](https://arxiv.org/abs/2611.12532)**  
   研究质疑将机器学习模型视为密码、用功耗分析提取全部权重的思路，指出完整网络权重恢复比已有概念验证所显示的更难。 · Mohammed Qaiss … Yuval Yarom · arXiv 2611.12532 · 2026-11-09 · [解读](https://aisafetyhot.com/items/f1v6a9psarahfk99qnqsp06hg)
3. **[ScrapeBench: Evaluating Legal Compliance of AI Agents in Website Scraping](https://arxiv.org/abs/2611.11306)**  
   论文提出 ScrapeBench，作者称这是首个实证评估 AI 智能体网页抓取法律合规性的基准，测试智能体是否遵守服务条款（ToS）与 robots.txt。 · Joseph Marvin Imperial … Noam Kolt · arXiv 2611.11306 · 2026-11-10 · [解读](https://aisafetyhot.com/items/mc43y1u0xio8q81jgxfcewx51)
4. **[Infrathon: Benchmarking Language Agents for Real-World, Long-Horizon AI Infra Optimization](https://arxiv.org/abs/2611.11995)**  
   研究者提出 Infrathon 基准，覆盖不同层级的真实长时程 AI 基础设施优化任务，用来考察前沿 Agent 能否在长时间跨度内持续改进 AI 基础设施。 · Zhengyu Hu … Radha Poovendran · arXiv 2611.11995 · 2026-11-09 · [解读](https://aisafetyhot.com/items/j0jdmm4ctvx55bkms8vdurpn9)
5. **[Harness Matters: Measuring and Dissecting Security Resilience in Web Agents](https://arxiv.org/abs/2611.11971)**  
   研究者提出 WebTrap Farm 评测框架，系统测量 Web Agent 执行 harness 的安全性，发现现有 harness 在典型攻击下仍然脆弱，且安全表现由 harness 与后端模型共同决定。 · Xinyi Wu … Min Yang · arXiv 2611.11971 · 2026-11-09 · [解读](https://aisafetyhot.com/items/ckc0cpxfthttztbvejs1jzlrh)
6. **[Is Persona Generalization Predictable?](https://arxiv.org/abs/2611.12864)**  
   大模型的人格泛化可以预测吗？ · Olina Mukherjee … Jacob Mitchell Springer · arXiv 2611.12864 · 2026-11-09 · [解读](https://aisafetyhot.com/items/jfp0ht2656sflueafvccuep4l)
7. **[FraudBench: A Legal Evaluation of AI Deception](https://arxiv.org/abs/2611.12167)**  
   构建 FRAUD BENCH，用源自美国判例的欺诈场景评测模型的自发欺诈倾向 · Kevin Wei … Noam Kolt · arXiv 2611.12167 · 2026-11-09 · [解读](https://aisafetyhot.com/items/y0v8mkqfyc2vypgqpgkecxfit)
8. **[Frontier AI Safety and Governance 2026: Risk Understanding and Coordinated Governance](https://arxiv.org/abs/2611.12434)**  
   世界互联网大会人工智能专业委员会《Frontier AI Safety and Governance 2026》报告：风险理解与协同治理 · Zeng Yi … Ren Xianliang · arXiv 2611.12434 · 2026-11-09 · [解读](https://aisafetyhot.com/items/fe9z9y1856yqdvkeyj645mgmc)
9. **[Double Blind Evals: Resolving the Dual Confidentiality Dilemma in AI Safety Auditing](https://arxiv.org/abs/2611.12604)**  
   论文提出一种“双盲评测”方案，用硬件级内存加密的安全隔离区，让评测方的提示词不向模型方公开，同时让模型权重和推理代码留在模型方基础设施内。 · Andrew Trask … William Isaac · arXiv 2611.12604 · 2026-11-09 · [解读](https://aisafetyhot.com/items/mt65uayce4s518vlhh06d1j0c)
10. **[Query-Only Prompt-Agnostic Attacks on Visual In-Context Learning](https://arxiv.org/abs/2611.11116)**  
   作者提出针对视觉上下文学习（VICL）可提示分割的仅查询、提示无关定向攻击，攻击者只能看到返回的 RGB 输出，无法访问模型内部或部署提示。 · Xiao Hu … Antonio Bianchi · arXiv 2611.11116 · 2026-11-08 · [解读](https://aisafetyhot.com/items/ge3jc9h44zkypo2h80bzco88v)
11. **[Coding Agents Propagate Vulnerabilities in Code Bases](https://arxiv.org/abs/2611.11455v1)**  
   评测编程智能体是否会模仿代码库中已有漏洞，在新代码中传播同类漏洞 · `Agent 安全` · Chenhao Sun … Martin Vechev · arXiv 2611.11455 · 2026-11-08 · [解读](https://aisafetyhot.com/items/ol8r5eyvde33yrtzvyrumjhht)
12. **[Chatter Attack: Resource Consumption Attack for Large Language Models](https://arxiv.org/abs/2611.11261)**  
   Chatter Attack：针对大语言模型的资源消耗攻击 · Yibo Miao … Yinpeng Dong · arXiv 2611.11261 · 2026-11-08 · [解读](https://aisafetyhot.com/items/yl1f8627iq5mtfbob4wjok7mx)
13. **[SkillCODER: Towards Auditing and Attribution of Copyright Infringement in LLM Agent Skills](https://arxiv.org/abs/2611.11308v1)**  
   论文提出 SkillCODER，用于在黑盒、仅内容设置下审计 LLM 智能体技能中的版权侵权并归因买家。 · Enhao Huang … Kui Ren · arXiv 2611.11308 · 2026-11-08 · [解读](https://aisafetyhot.com/items/ozq0udwk6qs0i0vjwwj7j2xfd)
14. **[ErosionBench: Probing Alignment Decay in Enterprise Multi-Agent Systems](https://arxiv.org/abs/2611.11266)**  
   Salesforce AI Research 提出 ErosionBench，一个在可执行环境中评测企业多智能体系统跨会话对齐衰减的安全基准。 · Riya Bharathwaj … Silvio Savarese · arXiv 2611.11266 · 2026-11-08 · [解读](https://aisafetyhot.com/items/dikafjxwb5cdtf187gbf1we03)
15. **[Deploying Physically and Epistemically Compliant Agents by Distilling Belief-Space Task and Motion Planners](https://arxiv.org/abs/2611.10430)**  
   通过蒸馏信念空间任务与运动规划器部署物理与认知合规智能体 · Phillip J. K. Christoffersen … Dylan Hadfield-Menell · arXiv 2611.10430 · 2026-11-07 · [解读](https://aisafetyhot.com/items/dul8ej9w4hi9qhm3cekn1l2l7)
16. **[Mind the Gap: Detecting Description-Execution Mismatch Attacks in DAO Governance](https://arxiv.org/abs/2609.13601v1)**  
   提出 DEMI 检测框架，用生命周期模拟和证据映射发现 DAO 提案错配 · Bowen Cai … Kangjie Lu · arXiv 2609.13601 · 2026-09-11 · [解读](https://aisafetyhot.com/items/ieuelb32pdbk1240g35fog8bo)
17. **[Muse Spark Safety & Preparedness Report](https://arxiv.org/abs/2606.12429v1)**  
   Meta 发布最新大语言模型 Muse Spark 的安全与 Preparedness 报告，结论是在 Meta AI 中部署该模型的残余风险在其 Advanced AI Scaling Framework 下处于可接受水平。 · Cristina Menghini … Summer Yue · arXiv 2606.12429 · 2026-05-14 · [解读](https://aisafetyhot.com/items/bes70mgc48abd2dfwjvwmf9pg)
18. **[Angel or Demon: Investigating the Plasticity Interventions' Impact on Backdoor Threats in Deep Reinforcement Learning](https://arxiv.org/abs/2605.14587v1)**  
   天使还是恶魔：探究可塑性干预对深度强化学习后门威胁的影响 · Oubo Ma … Shouling Ji · arXiv 2605.14587 · 2026-05-14 · [解读](https://aisafetyhot.com/items/w9xwk58da4x0kshgklkdr9vpq)
19. **[Widening the Gap: Exploiting LLM Quantization via Outlier Injection](https://arxiv.org/abs/2605.15152v2)**  
   向 LLM 权重注入离群值制造量化后恶意模型 · Xiaohua Zhan … Martin Vechev · arXiv 2605.15152 · 2026-05-14 · [解读](https://aisafetyhot.com/items/y7733b7pla073nqptl1ls5tir)
20. **[EVA: Editing for Versatile Alignment against Jailbreaks](https://arxiv.org/abs/2605.14750v1)**  
   EVA 框架通过直接模型编辑实现面向 LLM 和 VLM 的越狱防御，将安全对齐重构为精确知识修正任务，并定点编辑易受有害指令影响的特定神经元。 · Yi Wang … Wenjie Wang · arXiv 2605.14750 · 2026-05-14 · [解读](https://aisafetyhot.com/items/gbtmvncki5wfq2o8dd8bl6obf)
21. **[Hidden in Memory: Sleeper Memory Poisoning in LLM Agents](https://arxiv.org/abs/2605.15338)**  
   提出潜伏记忆投毒，诱导 Agent 把外部文档写成持久伪造记忆 · Sidharth Pulipaka … Mario Fritz · arXiv 2605.15338 · 2026-05-14 · [解读](https://aisafetyhot.com/items/vt0n0xvpqwpw8r8y699eiqfg4)
22. **[Veritas: Grounding LLM Agents for Reliable Vulnerability Reasoning over Stripped Binaries](https://arxiv.org/abs/2605.15097v3)**  
   研究者提出 Veritas，一个把剥离符号二进制上的漏洞推理形式化为语义接地问题的三阶段框架，让 LLM 智能体依据可验证证据而非直接推断来判断漏洞。 · Xinran Zheng … Lorenzo Cavallaro · arXiv 2605.15097 · 2026-05-14 · [解读](https://aisafetyhot.com/items/acbz8ywlix5g49d0il8oj28jo)
23. **[MetaBackdoor: Exploiting Positional Encoding as a Backdoor Attack Surface in LLMs](https://arxiv.org/abs/2605.15172v1)**  
   研究者提出名为 MetaBackdoor 的后门攻击，利用 Transformer 必须编码 token 位置这一特性，以与长度相关的位置结构作为非内容触发器，无需修改输入文本即可激活后门。 · Rui Wen … Ahmed Salem · arXiv 2605.15172 · 2026-05-14 · [解读](https://aisafetyhot.com/items/dxft6ynrigc09fsss12wxvra0)
24. **[Web Agents Should Adopt the Compile-and-Execute Paradigm](https://arxiv.org/abs/2605.14290v2)**  
   论文主张网页智能体应默认采用编译执行而非 ReAct，以限制不可信网页内容对智能体控制流的影响。 · Julien Piet … David Wagner · arXiv 2605.14290 · 2026-05-14 · [解读](https://aisafetyhot.com/items/ouwpp8m4vg57q0yjxvmhtxggm)
25. **[Selective Safety Steering via Value-Filtered Decoding](https://arxiv.org/abs/2605.14746v2)**  
   研究者提出价值过滤解码方法，让不安全回复更安全，同时减少对基座模型本会安全生成的不必要干预。 · Bat-Sheva Einbinder … Yaniv Romano · arXiv 2605.14746 · 2026-05-14 · [解读](https://aisafetyhot.com/items/j0ezl0x1vl4ft73zrb0gasqgj)
26. **[SlaClip: Gradient Norm Slacks can be Indicator for Adaptive Clipping in DP-SGD](https://openreview.net/forum?id=48suUeYKdb)**  
   提出 SlaClip，利用标准裁剪产生的松弛信息自适应调整 DP-SGD 裁剪阈值，无需额外隐私查询，在相同隐私预算下优于现有自适应裁剪方法。 · `隐私与数据泄露` · Shuyan Zou … Han Wu · ICML 2026 spotlight
27. **[Contrastive Spectral Rectification: Test-Time Defense towards Zero-shot Adversarial Robustness of CLIP](https://openreview.net/forum?id=o3SFLhXkvX)**  
   发现对抗样本在渐进频率衰减下特征不一致，提出测试时防御 CSR，在 16 个分类基准上对强 APGD 攻击平均超过 SOTA 18.1%，推理开销适中。 · `防御与护栏` · Sen Nie … Xilin CHEN · ICML 2026 regular
28. **[When Experience Becomes a Backdoor: Poisoning Self-Evolving LLM Agents via Failure-Aware Task Optimization](https://arxiv.org/abs/2611.10542)**  
   提出 BadEvolve 任务投毒框架，诱使自演化 Agent 把后门写进技能 · `后门与投毒` · Minhua Lin … Suhang Wang · arXiv 2611.10542 · 2026-11-07 · [解读](https://aisafetyhot.com/items/cy2ew721glyzs94wiolw8bnf5)
29. **[CyberBinGym: Can AI Agents Turn Binary Patches into Real Exploits?](https://arxiv.org/abs/2611.10723)**  
   构建 CyberBinGym 基准评测 AI 智能体仅凭二进制补丁完成漏洞复现与利用的能力 · Lambang Akbar Wijayadi … Dawn Song · arXiv 2611.10723 · 2026-11-07 · [解读](https://aisafetyhot.com/items/ep8z0qhm9stolb12trici1xng)
30. **[The Limits of Information-Flow Control Enforcement for Agentic Systems](https://arxiv.org/abs/2611.10395)**  
   研究者在有状态智能体系统模拟器中量化了信息流控制（IFC）在智能体系统中执行策略的局限。IFC 的安全标签单调增长并在系统中传播（标签蔓延），会逐渐限制系统效用。 · Jonathan Gregory … Patrick McDaniel · arXiv 2611.10395 · 2026-11-07 · [解读](https://aisafetyhot.com/items/kqsm5b7av9r9t8okaspy3rxht)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 33 · [Agent 安全](daily-papers/topics/agent-security.md) 33 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 13 · [后门与投毒](daily-papers/topics/backdoor.md) 10 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
