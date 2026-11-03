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
### 2026-11-03 · 30 篇

1. **[SecPO: Principled Adversarial Training for Prompt Injection Security](https://arxiv.org/abs/2610.41998)**  
   SecPO：面向提示注入安全的原则化对抗训练 · Sizhe Chen … David Wagner · arXiv 2610.41998 · 2026-10-30 · [解读](https://aisafetyhot.com/items/asbq6hgsrf1e68wkfnldd7zgt)
2. **[Towards Understanding Score-Seeking in LLMs](https://arxiv.org/abs/2610.41014)**  
   理解大语言模型中的追分行为 · Aghyad Deeb … Alex Mallen · arXiv 2610.41014 · 2026-10-29 · [解读](https://aisafetyhot.com/items/l1sorqx8ahw1gb2ea3h3r2w6i)
3. **[PrivacyFlow: Privacy in AI Agents through Information Flow Analysis and Consequence-Aware Risk Management](https://arxiv.org/abs/2610.40714)**  
   论文提出 PrivacyFlow，一种把隐私规划与任务执行分离的智能体隐私防护方法，并发布 agentic PrivacyBench 基准。 · Robin Staab … Reza Shokri · arXiv 2610.40714 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ydfan4r9ari5f8x8buf9bb77p)
4. **[Characterizing Recoverable Expert-Utilization Signatures in Fine-Tuned Mixture-of-Experts LLMs](https://arxiv.org/abs/2610.41039v1)**  
   研究者发现微调后的 MoE 大语言模型会记忆处理训练数据所用的内部专家路由路径，形成该训练过程独有的路由指纹。 · Fei Wang … Bo Li · arXiv 2610.41039 · 2026-10-29 · [解读](https://aisafetyhot.com/items/zjqx3905yafqe0n6xsi9qfu59)
5. **[AgentShield: Fortifying Web Applications Against AI Agents and Agentic Browsers](https://arxiv.org/abs/2610.41181)**  
   研究者提出行为指纹防御框架 AgentShield，用于帮助 Web 应用识别 AI 智能体与智能体浏览器。论文对主流反机器人机制的实证评测显示，许多为传统自动化设计的防御难以可靠识别自主 AI 智能体。 · Moiz Ali … Jason Polakis · arXiv 2610.41181 · 2026-10-30 · [解读](https://aisafetyhot.com/items/q0frugs8eikgbqkskkkjs0dfj)
6. **[LLM Detoxification via Transition-Aware Reward-Guided Representation Sampling](https://arxiv.org/abs/2610.41165)**  
   TARGRS 是测试时 LLM 去毒框架，在潜在表征空间学习毒性过渡的奖励引导。探索阶段沿毒性方向渐进引导构造无毒到有毒轨迹，把稀疏标注转为密集 listwise 监督训练 token 级奖励模型。 · Aishan Liu … Dacheng Tao · arXiv 2610.41165 · 2026-10-30 · [解读](https://aisafetyhot.com/items/g9plcxdyownjiwh461ilwqldz)
7. **[MetaVul: Agentic Harness Discovery for Vulnerability Detection](https://arxiv.org/abs/2610.40721v1)**  
   研究团队提出 MetaVul，用工作流式优化循环自动搜索用于漏洞检测的 Agent harness。 · Ira Ceka … Baishakhi Ray · arXiv 2610.40721 · 2026-10-29 · [解读](https://aisafetyhot.com/items/c0bnm9ouriay2hs7fhukb820u)
8. **["Shall We Approve?" Consequence-Aware Approval for Autonomous Coding Agents](https://arxiv.org/abs/2610.40753)**  
   论文提出 Caper，一种面向自主编码智能体的后果感知审批机制，先在快照沙箱中预执行每条命令，再把观察到的效果整理成受限报告交给独立审批器，放行允许的命令、回滚被阻止的命令并给出可操作原因。 · Weiheng Wu … David Lo · arXiv 2610.40753 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ax4ajsjg65xp9u0148tqog7o2)
9. **[When Skills Tell Agents Not to Ask: A Large-Scale Study of Oversight Directives in Agent Skills](https://arxiv.org/abs/2610.37734v1)**  
   当技能告诉智能体不要请示：智能体技能中监督指令的大规模研究 · Timofey Sanko, Yuan Tian · arXiv 2610.37734 · 2026-10-27 · [解读](https://aisafetyhot.com/items/a91mpnfkl5rczaoa3pfbafz70)
10. **[A Case Study on Emergent Cheating and Whistleblowing in Autonomous Research Swarms](https://arxiv.org/abs/2609.04170v1)**  
   展示自主科研智能体集群自发涌现的规范投机作弊与举报反制 · `奖励作弊` · Davide Paglieri … Alexander Sasha Vezhnevets · arXiv 2609.04170 · 2026-09-03 · [解读](https://aisafetyhot.com/items/tykblze77gkr7pyekgzqzh5yb)
11. **[PatchBench: Evaluating AI Agents for Vulnerability Patching](https://arxiv.org/abs/2609.04075)**  
   提出基准 PATCHBENCH，评测编程 Agent 的漏洞修补是否真正修复根因 · Chihao Shen … Yizheng Chen · arXiv 2609.04075 · 2026-09-03 · [解读](https://aisafetyhot.com/items/y59uoe8ndgqle4njfhs8n1xr5)
12. **[Trust Me, I'm Your Developer: Self-Issued Authentication in Large Language Models](https://arxiv.org/abs/2609.03247v1)**  
   提出 MIPC 与 CFA，观察模型自拟测验后接受开发者身份 · `越狱与攻击` · Syed Ghazanfar Abbas, Dongyan Xu · arXiv 2609.03247 · 2026-09-03 · [解读](https://aisafetyhot.com/items/cmzpnw9jprvm4att0hc0grygf)
13. **[Repeat-After-Me: Black-Box Adaptive Visual Prompt Injection](https://arxiv.org/abs/2609.04533v2)**  
   提出 Repeat-After-Me 自适应视觉提示注入，诱导 VLM 智能体执行指定任务 · Sizhe Chen … Arman Zharmagambetov · arXiv 2609.04533 · 2026-09-03 · [解读](https://aisafetyhot.com/items/bvtioq7ymyvgmojgfrcexhjna)
14. **[Shifting from Injection to Interaction: Rethinking Web Security in the Age of LLMs and Beyond](https://arxiv.org/abs/2609.03999v1)**  
   综述 LLM 时代 Web 安全威胁并提出监控控制框架 · Nivedita Singh … Hyoungshick Kim · arXiv 2609.03999 · 2026-09-03 · [解读](https://aisafetyhot.com/items/xczwchfm2bx7n16ard9qakcmc)
15. **[Harbor Adapters and Harbor-Index: Infrastructure and a Curated Meta-Dataset for Large-Scale Agentic Evaluation](https://arxiv.org/abs/2609.04298v3)**  
   构建统一 Agent 评测接口并发布精选元数据集 Harbor-Index · Lin Shi … Alex Shaw · arXiv 2609.04298 · 2026-09-03 · [解读](https://aisafetyhot.com/items/vihh6bgvns43lgnax4541b4ih)
16. **[Estimating the expected output of wide random MLPs more efficiently than sampling](https://arxiv.org/abs/2605.05179v2)**  
   作者提出无需采样即可估计初始化时宽随机 MLP 在高斯输入下期望输出的方法，用累积量和 Hermite 展开逐层近似激活分布。 · Wilson Wu … Paul Christiano · arXiv 2605.05179 · 2026-05-06 · [解读](https://aisafetyhot.com/items/ttipchea6gbs246cjsxi34eva)
17. **[DecodingTrust-Agent Platform (DTap): A Controllable and Interactive Red-Teaming Platform for AI Agents](https://arxiv.org/abs/2605.04808v1)**  
   作者构建智能体红队平台 DTAP、自动红队智能体 DTAP-Red 与基准 DTAP-Bench。 · Zhaorun Chen … Bo Li · arXiv 2605.04808 · 2026-05-06 · [解读](https://aisafetyhot.com/items/ubh69j3rhn0ow5v66l0xqb013)
18. **[Understanding Annotator Safety Policy with Interpretability](https://arxiv.org/abs/2605.05329v1)**  
   研究者提出 Annotator Policy Models（APMs），一种仅从标注行为中学习标注者内部安全政策的可解释模型，无需额外标注即可让标注者的推理可见、可比较。 · Alex Oesterling … Fred Hohman · arXiv 2605.05329 · 2026-05-06 · [解读](https://aisafetyhot.com/items/um70808lbwz22n9eqco5r6cu0)
19. **[Misrouter: Exploiting Routing Mechanisms for Input-Only Attacks on Mixture-of-Experts LLMs](https://arxiv.org/abs/2605.04446)**  
   提出 Misrouter，借 MoE 路由优化仅输入前缀并迁移攻击 · `越狱与攻击` · Zekun Fei … XiaoFeng Wang · arXiv 2605.04446 · 2026-05-06 · [解读](https://aisafetyhot.com/items/rv5gb9txiy76ogozfbtzg8t4f)
20. **[WAAA! Web Adversaries Against Agentic Browsers](https://arxiv.org/abs/2605.05509)**  
   提出面向智能体浏览器的 Web 威胁模型并复现混淆攻击 · Sohom Datta … Alexandros Kapravelos · arXiv 2605.05509 · 2026-05-06 · [解读](https://aisafetyhot.com/items/dzvy6j9g6llrzx65aeoaby95x)
21. **[IntraGuard: Committee-Side Defenses Against Review Outsourcing to Commercial Chatbots](https://arxiv.org/abs/2605.05271v2)**  
   论文提出 IntraGuard，一个面向编辑委员会和程序委员会的防御框架，用于阻止审稿人把同行评审整体外包给商用聊天机器人。 · Oubo Ma … Shouling Ji · arXiv 2605.05271 · 2026-05-06 · [解读](https://aisafetyhot.com/items/i9pwd1jsgqm7twwsfl79allyf)
22. **[CounselBench: A Large-Scale Expert Evaluation and Adversarial Benchmarking of Large Language Models in Mental Health Question Answering](https://openreview.net/forum?id=8MBYRZHVWT)**  
   与 100 名心理健康专家构建基准，发现大模型回答常含未经授权的医疗建议等安全风险，且 LLM 评委系统性高估回答并忽视安全问题。 · `儿童、青少年与心理健康` · Yahan Li … Ruishan Liu · ICLR 2026 Oral
23. **[Catch-22: On the Fundamental Tradeoff Between Detectability and Robustness in LLM Watermarking](https://openreview.net/forum?id=097IlaUfQY)**  
   用信息论框架刻画水印鲁棒性、隐蔽性与可验证性的三难权衡，提出按部署编辑强度在分布保持、语义级、词元级方案中选Pareto最优的混合策略，并在Llama-2-7B与Mistral-7B上验证。 · `防御与护栏` · Kuheli Pratihar, Debdeep Mukhopadhyay · ICML 2026 spotlight
24. **[How Much Can Tool Calls Reveal About You? Privacy Leakage from Tool-Call Traces](https://arxiv.org/abs/2610.41885)**  
   研究系统考察了从 MCP 工具调用轨迹推断用户画像的风险：即使观察者接触不到对话内容，仅凭协议合法的工具交互也能推断用户属性。 · Donghang Duan … Dongrui Liu · arXiv 2610.41885 · 2026-10-30 · [解读](https://aisafetyhot.com/items/maf9kigo3z1k6rtvu0qmvrgoc)
25. **[What Should LLMs Forget: Reinforcement Unlearning of Knowledge Associations](https://arxiv.org/abs/2610.41616)**  
   研究者提出 KARU，一种以知识关联（KA）为遗忘目标的 LLM 强化学习遗忘框架。现有方法通常优化整条回复、不显式定位待遗忘知识，导致遗忘粗放不可控。 · Wutong Xu … Xiangyang Ji · arXiv 2610.41616 · 2026-10-30 · [解读](https://aisafetyhot.com/items/wc5gxlqw8h90x4w65t9d92wyu)
26. **[When Safety Checks Become Privacy Risks: A Privacy-Preserving Paradigm for LLM Agent Safety Auditing](https://arxiv.org/abs/2610.41401)**  
   研究者提出 LLM 智能体安全审计的隐私保护范式，将委托审计计算与明文访问和执行权限分离，并实现为 SealCall 框架。该范式以基于 CKKS 的加密相似度计算保护审计输入，使其不被半诚实审计方获取。 · Yixiang Luo … Jiqiang Liu · arXiv 2610.41401 · 2026-10-30 · [解读](https://aisafetyhot.com/items/u6fdjt6i39c7cm21f3y3k0rou)
27. **[Accept Changes, Reject Attacks: Robust Memory Management for LLM Agents](https://arxiv.org/abs/2610.41056)**  
   论文把 LLM Agent 的记忆鲁棒性定义为同时处理过时记忆与记忆投毒，且不损害其他输入上的表现。作者指出，这两类失败需要相反的写入决策，单一固定写入规则无法兼顾，而以往工作多分别研究。 · Runze Zhao … Ankit Shah · arXiv 2610.41056 · 2026-10-29 · [解读](https://aisafetyhot.com/items/r1xrsqtif1q04xjswqx9zz27z)
28. **[Characterizing LLM Agent Behaviors in Module Shadowing Environments](https://arxiv.org/abs/2610.40716)**  
   刻画模块影子环境下的 LLM 智能体行为 · Shuai Yang … Yi Zeng · arXiv 2610.40716 · 2026-10-29 · [解读](https://aisafetyhot.com/items/c9xchlrbi98p3tax1n9p0wqn7)
29. **[The First Few Tokens Matter: Understanding Chain-of-Thought Controllability](https://arxiv.org/abs/2610.40939)**  
   最初几个 Token 很重要：理解思维链可控性 · Hugh Van Deventer … Laura Ruis · arXiv 2610.40939 · 2026-10-29 · [解读](https://aisafetyhot.com/items/tggdgygjg3875rtlhm2vp9512)
30. **[Does Scaling Toward AGI Depend on What System-1 Lets System-2 Execute?](https://huggingface.co/papers/2610.39497)**  
   论文对“迈向 AGI 的扩展是否取决于 System-1 让 System-2 执行什么”给出有条件的肯定答案。其条件交互循环中，轻量级 System-1 预测器估计候选交互效用，System-2 仅执行通过自适应阈值者。 · Qi Wang … Xiangyang Ji · arXiv 2610.39497 · 2026-10-29 · [解读](https://aisafetyhot.com/items/iwhrdhugs1mhb0vk37w7kk3kd)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [越狱与攻击](daily-papers/topics/jailbreak.md) 14 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 6 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
