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
### 2026-11-17 · 30 篇

1. **[An Operationalization of Opaque Serial Depth](https://arxiv.org/abs/2611.17495)**  
   提出 NLS depth 度量，量化模型不经可解释瓶颈的串行认知深度 · Nathan Sheffield … Ryan Greenblatt · arXiv 2611.17495 · 2026-11-12 · [解读](https://aisafetyhot.com/items/twe2tlczkudc4zei04rnq876b)
2. **[Soteria: Formally Verified Planning with Runtime Enforcement for Safe LLM Agents](https://arxiv.org/abs/2611.17880)**  
   Soteria 框架通过形式化验证的分层规划与运行时强制执行，让 LLM 智能体兼顾安全与任务效用。 · Mike He … Aarti Gupta · arXiv 2611.17880 · 2026-11-13 · [解读](https://aisafetyhot.com/items/w1wqaeg4wzjplcnts5tjbfhod)
3. **[Adaptable Watermarking: Transforming Image Watermarking Models via Lightweight Adapters](https://arxiv.org/abs/2611.18363)**  
   新框架让图像水印模型通过轻量级适配器即可转换为其他水印风格，无需重训完整模型。适配器以多域残差对齐损失微调，同时保持比特准确率。 · Mehrdad Saberi … John Collomosse · arXiv 2611.18363 · 2026-11-13 · [解读](https://aisafetyhot.com/items/k0c5m2kjgagd8c9s6t6e77wrg)
4. **[WebArena-Pro: A Heterogeneous, Multimodal, Reproducible Benchmark for Web Agents](https://huggingface.co/papers/2611.17955)**  
   WebArena-Pro：面向网页智能体的异构、多模态、可复现基准 · Imene Kerboua … Siva Reddy · arXiv 2611.17955 · 2026-11-13 · [解读](https://aisafetyhot.com/items/xm83aydb5r75ljxzzgw45b9wc)
5. **[Auditing Chatbots for Incursion into Professional Legal Practice](https://arxiv.org/abs/2611.17622)**  
   构建 UPLBench 审计聊天机器人是否越界提供构成无证执业的法律建议 · Nel Escher … Deirdre Mulligan · arXiv 2611.17622 · 2026-11-13 · [解读](https://aisafetyhot.com/items/a3j6av1gft2o4myvp2oioueae)
6. **[Beyond Attack-Based Accuracy: Rethinking Adversarial Robustness Evaluation Through Structural Gradient Alignment](https://arxiv.org/abs/2611.17377)**  
   提出 SGA 指标，用输入梯度结构对齐评估视觉模型对抗鲁棒性排序 · Hanrui Wang … Isao Echizen · arXiv 2611.17377 · 2026-11-11 · [解读](https://aisafetyhot.com/items/fvyh2qqf5mw3jw85dxflitatx)
7. **[Red-Teaming Auto Mode: Improving Blocking Classifiers Against Malign Coding Agents](https://arxiv.org/abs/2609.19587v2)**  
   提出 Auto Mode ++，加固编码 Agent 阻断监视器 · Alex Remedios … John Hughes · arXiv 2609.19587 · 2026-09-17 · [解读](https://aisafetyhot.com/items/sxcs1qxjh16iq223azuc5do78)
8. **[Coding Agents with Harness for Safe Robot Control](https://arxiv.org/abs/2609.20822v2)**  
   研究者评估了由大模型编写机器人控制程序的编码 Agent 在避障约束下的安全性，并提出护栏方案 SafeHarness。 · `Agent 安全` · Bingxin Xu … Emilio Ferrara · arXiv 2609.20822 · 2026-09-17 · [解读](https://aisafetyhot.com/items/g7lx5640c28tm2xzw6ki619hw)
9. **[Origin Is All You Need: Provenance-Aware Transformers for Structural Trust-Boundary Separation](https://arxiv.org/abs/2609.21088v1)**  
   提出 Provenance-Aware Transformers，隔离不可信来源防御间接提示注入 · Yuxuan Zhang … Guofei Gu · arXiv 2609.21088 · 2026-09-17 · [解读](https://aisafetyhot.com/items/gpxdtop770qo1xou6e2nvoco7)
10. **[Local Sparsity Enables Unsupervised LLM Safety Detection](https://arxiv.org/abs/2609.20129v1)**  
   提出局部稀疏无监督安全检测，标记偏离安全分布的输入 · `防御与护栏` · Xin Chen … Andreas Krause · arXiv 2609.20129 · 2026-09-17 · [解读](https://aisafetyhot.com/items/omqqywlnvksd7ideassvhul6y)
11. **[Inference-Engine Fingerprinting Attacks are Practical: Exploring Model-Driven Environmental Discovery, Exploitation, and Escape](https://arxiv.org/abs/2609.20614v1)**  
   提出推理引擎指纹识别攻击，误对齐模型探测引擎并发起逃逸链 · `Agent 安全` · Sarah Radway … James Mickens · arXiv 2609.20614 · 2026-09-17 · [解读](https://aisafetyhot.com/items/et5aips3hnx63jzbaft4m4950)
12. **[Robust Workflow Generation via Adversarial Learning for Audio Deepfake Detection](https://arxiv.org/abs/2609.20063v1)**  
   提出 ROGUE 对抗学习框架，生成抗真实扰动的音频深伪检测工作流 · Xiang Li … Wenqi Wei · arXiv 2609.20063 · 2026-09-17 · [解读](https://aisafetyhot.com/items/v49il6da9kmf3wr1pwgybqo98)
13. **[SoK: Trading Agents or Market Crashers? Dissecting Robustness and Security Failures in Academic Financial LLM Trading Schemes](https://arxiv.org/abs/2609.19705v1)**  
   用 FARSIGHT 方案级评测金融 LLM 交易 Agent 的稳健性与安全失败 · `Agent 安全` · Mengxiao Wang, Nitesh Saxena · arXiv 2609.19705 · 2026-09-17 · [解读](https://aisafetyhot.com/items/ggt3eoxtkir75tjj9arch3dw5)
14. **[Conditional Equivalence of DPO and RLHF: Implicit Assumption, Failure Modes, and Provable Alignment](https://arxiv.org/abs/2605.20834v1)**  
   证明 DPO 与 RLHF 等价有条件，揭示失效并提出 CPO 约束优化 · Zhiqin Yang … Yike Guo · arXiv 2605.20834 · 2026-05-20 · [解读](https://aisafetyhot.com/items/no1uz68wculdyvou942m1qp35)
15. **[Latent-space Attacks for Refusal Evasion in Language Models](https://arxiv.org/abs/2605.21706v2)**  
   提出受控潜空间规避攻击，将表征推过拒绝边界以绕过拒答 · Giorgio Piras … Battista Biggio · arXiv 2605.21706 · 2026-05-20 · [解读](https://aisafetyhot.com/items/r6w68ixmg06epskgii3g473nd)
16. **[Benchmarking and Improving Monitors for Out-Of-Distribution Alignment Failure in LLMs](https://arxiv.org/abs/2605.21602v2)**  
   提出 MOOD 基准并组合护栏与 OOD 检测器改进失准监控 · Dylan Feng … Cassidy Laidlaw · arXiv 2605.21602 · 2026-05-20 · [解读](https://aisafetyhot.com/items/iq6w5n55cxisb0hse5bdhq21t)
17. **[Disentangling Forgetting from Utility: Lightweight LLM Unlearning via Orthogonal Null-Space Projection](https://arxiv.org/abs/2611.17864)**  
   提出 UUE 零空间投影遗忘方法，在删除指定知识时保留模型效用 · Xiuyuan Wang … Xiaolin Zheng · arXiv 2611.17864 · 2026-11-13 · [解读](https://aisafetyhot.com/items/sgx5ksmts6mnjdfm0lo4qxp5x)
18. **[Representational Geometry as a Diagnostic for Adversarial Robustness](https://arxiv.org/abs/2611.17684)**  
   用 M-PHATE 嵌入与几何指标诊断对抗训练如何重塑网络表示几何 · Brandon Ismalej … Gal Mishne · arXiv 2611.17684 · 2026-11-13 · [解读](https://aisafetyhot.com/items/vgr97lqeojzprpq5lrai97d1a)
19. **[Antidistillation is Cheap: Lightweight Distillation-Resistance via Stylistic Corruption](https://arxiv.org/abs/2611.17772)**  
   提出向教师激活注入风格转向向量的反蒸馏防御，降低黑盒蒸馏克隆效果 · Anh Tu Ngo, Anupam Chattopadhyay · arXiv 2611.17772 · 2026-11-13 · [解读](https://aisafetyhot.com/items/t9a33pqkeoyjlmqztex6e1ul3)
20. **[A Generalizable Approach to Safety-Aware Robotic Behavior Planning with an Explicit Constraint Space](https://arxiv.org/abs/2611.18026)**  
   提出显式约束空间的安全机器人行为规划框架，执行前检查并纠正计划 · Xianxu Wu … Jianwei Zhang · arXiv 2611.18026 · 2026-11-13 · [解读](https://aisafetyhot.com/items/q7warhppkxh5sabs6rxhcuwar)
21. **[Alignment by Socialization: Learning Tradeoffs Under Selection](https://arxiv.org/abs/2611.18531)**  
   提出进化选择框架比较三类裁决策略，称经验学习策略能收敛人类权衡 · Thomas Brennan … Chaoyi Zhao · arXiv 2611.18531 · 2026-11-13 · [解读](https://aisafetyhot.com/items/pp5jn5vjyuhrchv30433hlamm)
22. **[Adversarially Attacking Symbolic Vocabulary Vulnerabilities In LLM Planners](https://arxiv.org/abs/2611.17910)**  
   研究者提出名为 Symbolic Swapper 的基于 LLM 的攻击模型，可自动生成使用非标准符号词汇的混淆规划域，系统性破坏强推理模型的规划能力。 · Stephen Obadinma, Xiaodan Zhu · arXiv 2611.17910 · 2026-11-13 · [解读](https://aisafetyhot.com/items/blnigo0xa5fk07w2c39111hf0)
23. **[Personalization of Basic and Moral Values Guiding LLM-Controlled Assistant Robots](https://arxiv.org/abs/2611.18230)**  
   用三份心理量表测用户期望与 LLM 默认价值画像，评估助理机器人价值观个性化 · Mateusz Wozniak … Agnieszka Wykowska · arXiv 2611.18230 · 2026-11-13 · [解读](https://aisafetyhot.com/items/w3pxqya4w4i0qni4rbtpa0tr3)
24. **[Securing Multi-Agent Systems by Design](https://arxiv.org/abs/2611.17883)**  
   提出响应操纵攻击 ReMA 与安全聚合规则 SecMAS，防御恶意智能体操纵多智能体聚合结果 · Xilong Wang … Neil Gong · arXiv 2611.17883 · 2026-11-13 · [解读](https://aisafetyhot.com/items/uuod2lmmngq5ublmreu12dp7s)
25. **[Can Mechanistic Interpretability Help Explain LLM Agent Failures? A Case Study on Web Element Hallucination](https://arxiv.org/abs/2611.18514)**  
   用机制可解释性工具分析网页智能体的元素幻觉，探针可预测、引导可修复但无法完整解释 · Mohamed Aghzal … Ziyu Yao · arXiv 2611.18514 · 2026-11-13 · [解读](https://aisafetyhot.com/items/oybuujjgoq2oppld87gkgk62g)
26. **[Creating Steering Vectors via Input Optimisation](https://arxiv.org/abs/2611.17481)**  
   提出 ActGCG，用 GCG 搜索输入后缀复现 steering vector 的激活与行为 · `越狱与攻击` · Batuhan Akar · arXiv 2611.17481 · 2026-11-12 · [解读](https://aisafetyhot.com/items/fxafmziktxxltvw1owro217yf)
27. **[Unfinished-Bench: Measuring Rule Violations by Persistent Agents in Realistic Work Environments](https://arxiv.org/abs/2611.17460)**  
   构建 Unfinished-Bench，测量持久化对 Agent 违反内部文档规则的影响 · `Agent 安全` · Seunghyun Lee … Sangdoo Yun · arXiv 2611.17460 · 2026-11-12 · [解读](https://aisafetyhot.com/items/nu2b0qt8zbparlcmgf150arwo)
28. **[Interpreting Coding Agents Through Their Behavioral Trajectories](https://huggingface.co/papers/2611.17440)**  
   通过行为轨迹解读编码智能体 · Ibragim Badertdinov, Alexander Golubev · arXiv 2611.17440 · 2026-11-12 · [解读](https://aisafetyhot.com/items/o58o1l2igncs5mb6qth7yi66s)
29. **[From Bytes to Behavior: Request-Level Attribution from Live GPU Hidden States](https://arxiv.org/abs/2611.18272)**  
   用非修改调试器从运行中 GPU 进程读取残差流，实现请求级行为归因 · Jonathan Pan … Brenda Ong · arXiv 2611.18272 · 2026-11-13 · [解读](https://aisafetyhot.com/items/s022pevgpbqtrt9cw643refi5)
30. **[Causal AI-Driven Secure mmWave Beam Alignment with Defensive Variational Autoencoders](https://arxiv.org/abs/2611.18321)**  
   提出因果特征选择加 DVAE 去噪的毫米波波束对齐防御，抵御 RSSI 对抗扰动 · Nasir Khan … Cicek Cavdar · arXiv 2611.18321 · 2026-11-13 · [解读](https://aisafetyhot.com/items/c5ypiuprfqp0eakk5ev3dkh8u)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[Agent 安全](daily-papers/topics/agent-security.md) 47 · [防御与护栏](daily-papers/topics/defense.md) 35 · [越狱与攻击](daily-papers/topics/jailbreak.md) 19 · [后门与投毒](daily-papers/topics/backdoor.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 13 · [奖励作弊](daily-papers/topics/reward-hacking.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 4 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [提示注入](daily-papers/topics/prompt-injection.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1
<!-- papers:end -->

## 反馈

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来。
