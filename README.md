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
### 2026-11-01 · 30 篇

1. **[Adversarial Self-Distillation](https://arxiv.org/abs/2610.38732)**  
   研究者提出对抗自蒸馏（ASD），把模型自身在干净提示下的拒答行为扩展到对抗扰动空间，用于应对能绕过安全对齐模型防护的对抗攻击。 · Mohammad Sadegh Akhondzadeh … Aleksandar Bojchevski · arXiv 2610.38732 · 2026-10-28 · [解读](https://aisafetyhot.com/items/jjsqq7lkt0quancfq1n10hcf9)
2. **[Who Else Is In? Multi-Agent Collusion Initation Via Strategic Vagueness](https://arxiv.org/abs/2610.37984)**  
   研究团队提出合谋发起问题并设计互相识别实验，测试 LLM 智能体能否在被监控的公开频道里通过普通任务讨论互相认出潜在合谋伙伴。 · Pramod Kaushik … Sahar Abdelnabi · arXiv 2610.37984 · 2026-10-27 · [解读](https://aisafetyhot.com/items/dxhea72lhlx8j4h5jewbv5wwi)
3. **[FVH-Bench: Evaluating Image Generator Safety Beyond Overtly Harmful Imagery](https://arxiv.org/abs/2610.37722)**  
   FVH-Bench：评估图像生成器在显性有害图像之外的安全性 · Zihao Zhu … Baoyuan Wu · arXiv 2610.37722 · 2026-10-27 · [解读](https://aisafetyhot.com/items/oghasv5e2xlx7ko7yz6reubtw)
4. **[A SoK for SoCs: Reading the TI Leaves on AI for Cyber Threat Intelligence Generation and Sharing](https://arxiv.org/abs/2609.01174v1)**  
   一项 SoK 研究梳理 AI 在网络威胁情报（CTI）生成与共享中的应用，发现当前 LLM 可辅助其四个步骤，但每步仍需专家监督。作者将该环节分为情报提取、规范化与增强、编码、分发四步。 · Saastha Vasan … Giovanni Vigna · arXiv 2609.01174 · 2026-09-01 · [解读](https://aisafetyhot.com/items/f24zmzmvvzknki2lmr10cs44k)
5. **[What's in Your Agent's Context? Context Privilege Escalation Attacks against AI Agent Harness](https://arxiv.org/abs/2609.01222)**  
   提出针对 Agent Harness 的上下文特权提升攻击 · Zichuan Li … Luyi Xing · arXiv 2609.01222 · 2026-09-01 · [解读](https://aisafetyhot.com/items/t82bkke5b8w16eqy3syus7uw2)
6. **[Hearing the Whispers: Black-Box Membership Inference Attacks on Finetuned TTS Models](https://arxiv.org/abs/2609.01723v1)**  
   提出针对微调 TTS 的黑盒成员推断攻击 · Kunlin Cai … Yuan Tian · arXiv 2609.01723 · 2026-09-01 · [解读](https://aisafetyhot.com/items/sks96tirl8fsra7dvisxtxxa9)
7. **[Differentially Private Paired Table-Image Multimodal Synthesis](https://arxiv.org/abs/2609.00708v1)**  
   DP-TabImage 是差分隐私的成对表格-图像多模态合成框架，用隐私概率图模型建模表格分布，用 DP-SGD 训练的表格条件扩散模型生成图像。 · Kai Chen … Tianhao Wang · arXiv 2609.00708 · 2026-09-01 · [解读](https://aisafetyhot.com/items/ercij07l8i0i4g4einai2zpyn)
8. **[Membership Inference in Fine-tuned Diffusion Language Models via Token-level Memorization Asymmetry](https://arxiv.org/abs/2609.00873v1)**  
   提出 Q-SKEW，利用 token 级记忆不对称推断微调扩散语言模型的成员 · Shengfang Zhai … Sanghyun Hong · arXiv 2609.00873 · 2026-09-01 · [解读](https://aisafetyhot.com/items/r0jvolrkt1vrwtlo2zptsrz2e)
9. **[SoK: When Safe Agents Fail Together: The Security of Multi Agent LLM Systems](https://arxiv.org/abs/2609.00595v1)**  
   系统化梳理多智能体 LLM 系统的攻击路径、风险与防御 · Rui Yang … Yinzhi Cao · arXiv 2609.00595 · 2026-09-01 · [解读](https://aisafetyhot.com/items/wq5u92cyyfpacdsvc35w8gnxa)
10. **[Dissecting Training-Free Uncertainty Estimation in Multimodal Large Language Models](https://arxiv.org/abs/2609.22206)**  
   比较多模态大模型上三类免训练不确定性估计 · Soroush Seifi … Rahaf Aljundi · arXiv 2609.22206 · 2026-09-01 · [解读](https://aisafetyhot.com/items/fxwbclkkizzyoi2xfz45syp0s)
11. **[Beyond the Payload: How User Invocation Shapes Coding Agent Vulnerability to Repository Poisoning](https://arxiv.org/abs/2608.30686v1)**  
   超越攻击载荷：用户调用方式如何影响编码 Agent 对仓库投毒的脆弱性 · Fukang Zhu … Shouling Ji · arXiv 2608.30686 · 2026-08-31 · [解读](https://aisafetyhot.com/items/rytd40a7x4lxogx6rlf91txn8)
12. **[Dependency-Aware Privacy for Multi-turn LLM Agents](https://arxiv.org/abs/2605.03188v3)**  
   论文提出 RootGuard，一种面向多轮 LLM 智能体的隐私防护方法，只对根值净化一次即可让隐私保证不随交互轮数衰减。 · Divyam Anshumaan … Somesh Jha · arXiv 2605.03188 · 2026-05-04 · [解读](https://aisafetyhot.com/items/ejc6uwl68dnfxm44c7wugftcb)
13. **[Safeguarding LLM Agents against Long-Horizon Threats via Shadow Memory](https://arxiv.org/abs/2605.03228v2)**  
   论文提出 ShadowMem 防御框架，用于应对利用用户、智能体与环境的长程交互实施恶意目标的攻击，这类目标在单轮交互中难以实现。 · Yuhui Wang … Ting Wang · arXiv 2605.03228 · 2026-05-04 · [解读](https://aisafetyhot.com/items/bqefzyevg5sixzxbzvv5helom)
14. **[SOTOPIA-TOM: Evaluating Privacy and Information Management in Multi-Agent Interaction with Theory of Mind](https://arxiv.org/abs/2605.02307v2)**  
   研究者发布 SOTOPIA-TOM 基准，用于评估 LLM 智能体在多方交互中处理信息不对称与隐私信息的能力。 · Yashwanth YS … Maarten Sap · arXiv 2605.02307 · 2026-05-04 · [解读](https://aisafetyhot.com/items/a0q9cu7axw7nmm117mjxylzhc)
15. **[Useless but Safe? Benchmarking Utility Recovery with User Intent Clarification in Multi-Turn Conversations](https://arxiv.org/abs/2604.27093v2)**  
   无用但安全？多轮对话中用户意图澄清下的效用恢复基准测试 · Mingqian Zheng … Maarten Sap · arXiv 2604.27093 · 2026-04-29 · [解读](https://aisafetyhot.com/items/xzzy26lv9fxzvucxdcy8gwogh)
16. **[InferD: A Honeypot Framework for AI Inference Infrastructure](https://arxiv.org/abs/2610.39807)**  
   研究者提出 InferD，一个面向 AI 推理基础设施的低交互蜜罐框架，核心原则是“欺骗而不推理”（deception without inference）：对手可观察的每个请求都由静态响应池应答，对手提交的任何内容都不会被执行。 · Hicham Hammouchi, Gabriele Lenzini · arXiv 2610.39807 · 2026-10-29 · [解读](https://aisafetyhot.com/items/siuaq8adzhhtlhjlmzpxpiy6y)
17. **[DICE: Decentralized Incentive-driven Federated Learning for Efficient & Scalable Customization of Pretrained Models in Web3](https://arxiv.org/abs/2610.39132)**  
   DICE 是一种基于区块链的联邦学习（BCFL）算法，让 Web3 中互不信任的参与者高效、可扩展地定制大型预训练模型。 · Hong Lin … Gang Chen · arXiv 2610.39132 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ikrm09lsj8trvxioy1xa8mxwc)
18. **[AgentDecept: Benchmarking Deceptive Behavior in Tool-Using LLM Agents under Pressure](https://arxiv.org/abs/2610.39377)**  
   研究者提出 AgentDecept，一个评测工具使用型 LLM 智能体在压力下是否如实汇报的可执行基准。 · Yehan Zhang … Xin Eric Wang · arXiv 2610.39377 · 2026-10-29 · [解读](https://aisafetyhot.com/items/a9xl9f8hunbkyu0ioxzzh61n8)
19. **[Red-Teaming Large Language Models in Low-Resource African Languages: A Case Study of Yoruba and Nigerian Pidgin](https://arxiv.org/abs/2610.39590)**  
   低资源非洲语言中的大语言模型红队测试：约鲁巴语与尼日利亚皮钦语案例研究 · Paula Chikaodinaka Anyanwu … Shamsuddeen Hassan Muhammad · arXiv 2610.39590 · 2026-10-29 · [解读](https://aisafetyhot.com/items/okinjodilyva8ehgo75x9w6ro)
20. **[Revisiting Over-refusal in Safety-aligned Large Language Models: A Representation and Optimization Perspective](https://arxiv.org/abs/2610.39802)**  
   研究者提出安全对齐框架 GOAL（Gradient Orthogonalization with contrAstive Learning），通过梯度正交化与对比学习缓解安全对齐大语言模型的过度拒答，多个模型和基准上的实验显示其在减少对无害请求误拒的同时保持安全性能与通用能力。 · Chao Chen … Richang Hong · arXiv 2610.39802 · 2026-10-29 · [解读](https://aisafetyhot.com/items/j5n8li92bnh327pd6ivlozvdj)
21. **[LiDAR-SHIELD: A Fully Dockerized Adversarial Robustness Assessment Framework for LiDAR-Based 3D Perception Models](https://arxiv.org/abs/2610.39848)**  
   研究者发布 LiDAR-SHIELD，一个面向基于 LiDAR 的 3D 感知模型的全 Docker 化对抗鲁棒性评估框架，代码开源于 https://github.com/alexandrosgk/LiDAR-shield。 · Alexandros Gkillas … Aris S. Lalos · arXiv 2610.39848 · 2026-10-29 · [解读](https://aisafetyhot.com/items/vy6yhh8vj9dq60ppamdx0vag7)
22. **[ARBITRA: Robust Document-Level ATT&CK Extraction via Multi-Expert Argumentation](https://arxiv.org/abs/2610.39433)**  
   ARBITRA 用多个角色专精的 LLM 专家从完整 CTI 报告提出候选 MITRE ATT&CK 实体，再经基于文档证据的 QBAF 论证逐项验证。 · Youngjin Jin, Seungwon Shin · arXiv 2610.39433 · 2026-10-29 · [解读](https://aisafetyhot.com/items/rb0vg9851d5eb1qpmt9y5oq52)
23. **[Localizing Concepts in Visual Autoregressive Models](https://arxiv.org/abs/2610.40061)**  
   研究者提出 LoCo，称这是首个模型无关的框架，可定位自回归模型中特定概念在何处、何时涌现。 · Nanxiang Jiang … Min Xu · arXiv 2610.40061 · 2026-10-29 · [解读](https://aisafetyhot.com/items/xt5279it9fex2v3i9eeyt7q9d)
24. **[How I Aligned Your Model: Scaling Up Multilingual Safety Training with Templates](https://arxiv.org/abs/2610.40516)**  
   我如何对齐你的模型：用模板扩展多语言安全训练 · Max Neuwinger … Imanol Schlag · arXiv 2610.40516 · 2026-10-29 · [解读](https://aisafetyhot.com/items/vcngr2t6x5o4y5w81k7syoplz)
25. **[Unraveling the Efficacy of Neuron Coverage Criteria on Testing Large Language Models](https://arxiv.org/abs/2610.40234)**  
   研究者评估了六种神经元覆盖准则在测试大语言模型上的实效，发现这些准则评估样本多样性有效，揭示对抗错误的能力却有限。 · Xiaoning Ren … Yinxing Xue · arXiv 2610.40234 · 2026-10-29 · [解读](https://aisafetyhot.com/items/i2snf8nfmm6sxryo9u55wm3bx)
26. **[Does the Citation Matter? Quality, Grounding, and Physician-Rubric Accuracy of Google's AI Overviews for Medical Information](https://arxiv.org/abs/2610.39339)**  
   引用重要吗？Google AI Overviews 医疗信息回答的信源质量、引用支撑与医生评分准确性 · Sam Agnoli … Emőke-Ágnes Horvát · arXiv 2610.39339 · 2026-10-29 · [解读](https://aisafetyhot.com/items/dvjkm4hnd2mmaw6b7i3am1vwl)
27. **[Visually Irrelevant Hallucinations in Medical Vision-Language Models](https://arxiv.org/abs/2610.38389)**  
   研究者提出模型无关的事后审计框架 CLEAR，用于在短语级别估计医疗视觉语言模型的视觉无关幻觉风险，这类错误指模型生成的临床表述缺乏视觉证据或与图像内容矛盾。 · Ke Zou … Huazhu Fu · arXiv 2610.38389 · 2026-10-28 · [解读](https://aisafetyhot.com/items/z0hek9ya6uu8pttnlb9j6v9np)
28. **[Interventional Training Reduces Causal Bypass in In-Context Introspection](https://arxiv.org/abs/2610.38911)**  
   研究者提出干预式训练方法，减少语言模型上下文内省中的因果旁路，即自报依赖与对象相关但无因果联系的信号。 · Zilu Tang … Derry Wijaya · arXiv 2610.38911 · 2026-10-28 · [解读](https://aisafetyhot.com/items/roycfg7ss4ns3adeckmrt1n7d)
29. **[DecisionUnlearn-Bench: Unlearning Probabilistic Decisions under Changing Schemas](https://arxiv.org/abs/2610.38431)**  
   研究者提出面向概率决策模型的机器遗忘评测框架 DecisionUnlearn-Bench，在删除粒度、标签呈现和候选集变化下比较完整模型、遗忘模型与仅保留数据训练的模型。 · Tiantong Wu, Wei Yang Bryan Lim · arXiv 2610.38431 · 2026-10-28 · [解读](https://aisafetyhot.com/items/kabj1nn1ejb3a1em8dweg5ggq)
30. **[Auditable Belief Updates as a Missing Safety Layer for LLM-Powered Multi-Agent Systems](https://arxiv.org/abs/2610.38869)**  
   论文提出 EB-MAS 框架，把智能体信念状态外化为结构化载体，为 LLM 驱动的多智能体系统补上可审计的信念更新安全层。 · Zhuoyun Li … Yi Dong · arXiv 2610.38869 · 2026-10-28 · [解读](https://aisafetyhot.com/items/el6ljsbprpt24m9rl0toqcl0e)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 30 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [隐私与数据泄露](daily-papers/topics/privacy.md) 11 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
