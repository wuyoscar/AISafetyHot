<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

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
### 2026-10-24 · 30 篇

1. **[Agentic Verified Optimization of Real-World Software](https://arxiv.org/abs/2610.30188)**  
   研究者提出智能体验证式优化任务，要求智能体在产出更快实现的同时给出与既有实现等价的机器可检验证明，以应对现有等价检查主要依赖测试、而智能体已被证明会利用测试通过检查却不保留原行为的问题。 · Zhe Ye … Soonho Kong · arXiv 2610.30188 · 2026-10-20 · [解读](https://aisafetyhot.com/items/f87rjw6ue0ndlqts0ml1vmw6d)
2. **[Reliable AI-Assisted Decisions via Selective Auditing](https://arxiv.org/abs/2610.31662)**  
   研究者提出一种选择性审计方法，在保证未被审计的 AI 错误比例低于用户设定阈值的前提下，尽量减少人工专家审查。 · Isaac Gibbs … Tijana Zrnic · arXiv 2610.31662 · 2026-10-22 · [解读](https://aisafetyhot.com/items/al3j0tqwv9nmcao2h6loxq0c7)
3. **[AgentVQA: A Unified Benchmark for Agentic Visual Understanding](https://huggingface.co/papers/2610.31494)**  
   研究者推出 AgentVQA，一个覆盖网页智能体、机器人、第一人称视频、游戏和空间规划五类场景的离线基准，用于评测视觉语言模型在真实智能体任务上的表现，以补充成本高、难扩展的在线评测。 · Advait Gupta … Zhuang Liu · arXiv 2610.31494 · 2026-10-22 · [解读](https://aisafetyhot.com/items/plkhelivg2je0clguk3yw8oq6)
4. **[Diffusion Language Models for Perplexity-Aware Black-Box Attacks](https://arxiv.org/abs/2610.31558)**  
   论文提出用连续扩散语言模型（dLLM）替换连续空间黑盒攻击中的随机映射，在保留标准高斯隐空间表述以及下游采样、优化流程的同时，生成更自然的提示词。 · Ali Al-Lawati … Suhang Wang · arXiv 2610.31558 · 2026-10-22 · [解读](https://aisafetyhot.com/items/quxuqf98smwv3fnix8slj3j9a)
5. **[RIDAR: Safeguarding Research Integrity in Autonomous Research Agents via Automated Detection and Runtime Intervention](https://huggingface.co/papers/2610.31372)**  
   RIDAR 是一个自动检测研究诚信违规（RIV）并在智能体运行时进行干预的框架。 · Jiening Siow … Juanzi Li · arXiv 2610.31372 · 2026-10-22 · [解读](https://aisafetyhot.com/items/goqn1r4h5k1x6wr2p2dmj4wa2)
6. **[Interpreting Model Reasoning through Behavioral Counterfactuals](https://arxiv.org/abs/2610.30630)**  
   研究者提出一种基于行为反事实的可解释性方法，用于定位和分析提示干预如何影响模型的思维链推理。 · Shawn Im … Sharon Li · arXiv 2610.30630 · 2026-10-22 · [解读](https://aisafetyhot.com/items/tix4qxca5dccjnhuz5q1dp1t3)
7. **[OP-Print: Tracing Membership Imprints in On-Policy Self-Distillation](https://arxiv.org/abs/2610.31616)**  
   论文提出 OP-Print 攻击框架，作者称这是首个针对在线策略自蒸馏的成员推断攻击研究，在灰盒和黑盒两种威胁模型下均能有效判断样本是否参与训练。 · Qi Li, Xinchao Wang · arXiv 2610.31616 · 2026-10-22 · [解读](https://aisafetyhot.com/items/gqz4s7k7zocvy0hlic1tdd274)
8. **[Not Where You Think: Protecting Location Privacy Against Reasoning-Based Geolocation](https://arxiv.org/abs/2610.30439)**  
   研究者提出结构化推理攻击 GeoTrace，揭示大型推理模型如何在元数据和明显地理标识被移除后，仅凭视觉信息从普通照片中提取位置线索并进行由粗到细的地理推理。 · Shanghao Shi … Ning Zhang · arXiv 2610.30439 · 2026-10-21 · [解读](https://aisafetyhot.com/items/j18t4fqgkurv6t0oo4ob25eum)
9. **[Beyond End-to-End Recovery: Towards a Better Understanding of LLM Steganography via Rolewise Decomposition](https://arxiv.org/abs/2610.30516)**  
   研究者提出按角色分解的框架，将 LLM 隐写的评估从端到端恢复拆分为编码端文本如何表示私密消息、解码端恢复出什么，以及确定性验证能确立什么。 · Om Tailor … Kaiqing Zhang · arXiv 2610.30516 · 2026-10-21 · [解读](https://aisafetyhot.com/items/k04pc1yj8s5r11eilkoqwdph2)
10. **[FrontierCS 2: A Benchmark for Computer Science R&D](https://huggingface.co/papers/2610.29932)**  
   FrontierCS 2：面向计算机科学研发的基准 · Qiuyang Mang … Alvin Cheung · arXiv 2610.29932 · 2026-10-21 · [解读](https://aisafetyhot.com/items/pw8lvs8d6f9uhz0twr88tdrdm)
11. **[Beyond the Mandate: A Systematic Security Analysis of the Agent Payments Protocol (AP2)](https://arxiv.org/abs/2608.23858)**  
   系统分析智能体支付协议的前置上下文操纵与授权威胁 · `Agent 安全` · Avital Aviv … Asaf Shabtai · arXiv 2608.23858 · 2026-08-24 · [解读](https://aisafetyhot.com/items/dm4zx6om9wqwxmerjr3l5yob1)
12. **[AI Agents Push Humans Out of the Loop](https://arxiv.org/abs/2608.23642)**  
   主张用认知脚手架维持对 AI 智能体的人工监督 · Margaret Mitchell … Samir Passi · arXiv 2608.23642 · 2026-08-24 · [解读](https://aisafetyhot.com/items/ztrrc9h7xtbq9q0as442uba49)
13. **[Tracing Provenance and Detecting Tampering with Complementary LLM Watermarks](https://arxiv.org/abs/2608.12713v1)**  
   提出 Cocktail 水印，共嵌稳健与脆弱信号以溯源并发现篡改 · Xiaoyan Feng … Shirui Pan · arXiv 2608.12713 · 2026-08-13 · [解读](https://aisafetyhot.com/items/zf2w382uer2ebbgv7ok0q2dy4)
14. **[Refusing Intent, Not Form: Wrapper-Based Intent-Group Supervision for LLM Safety](https://arxiv.org/abs/2608.13304v1)**  
   提出 WIFA 意图组监督微调，缓解包装式越狱与过度拒答 · `防御与护栏` · Ping Wu … Yi Zeng · arXiv 2608.13304 · 2026-08-13 · [解读](https://aisafetyhot.com/items/sez6mdkitgj2vmmh0afe0z599)
15. **[RedTeamCUA: Realistic Adversarial Testing of Computer-Use Agents in Hybrid Web-OS Environments](https://openreview.net/forum?id=yWwrgcBoK3)**  
   提出混合沙箱对抗测试框架与含864个样本的RTC-Bench，发现前沿CUA对间接提示注入脆弱，Claude 3.7 Sonnet攻击成功率42.9%，最安全的Operator也有7.6%。 · `提示注入` · Zeyi Liao … Huan Sun · ICLR 2026 Oral
16. **[GoodDiffusion: Proactive Copyright Protection for Diffusion Bridge Models via Learnable Sample-specific Signatures](https://openreview.net/forum?id=wkV9jSqwa9)**  
   借鉴后门机制将授权内化进生成过程，授权签名可正常生成、未授权输入被拒绝，并用可学习签名网络防止替代签名被梯度优化恢复。 · `开源模型与权重安全` · Shixi Qin … Qingming Huang · ICML 2026 spotlight
17. **[Certified Execution Harness for Agentic AI: Safe and Least-Intrusive Petri-Net Supervisory Control Between Reasoning and Action](https://arxiv.org/abs/2610.31376)**  
   论文提出一种基于 Petri 网的经认证执行护栏，用于在提示注入下约束 LLM 智能体的工具调用。 · Chao Gu, Quanyan Zhu · arXiv 2610.31376 · 2026-10-22 · [解读](https://aisafetyhot.com/items/dn4u8rvi6xb3kngtqgyhibo87)
18. **[Inherited, Not Invented: Tracing the Provenance of Wait in Reasoning Models](https://huggingface.co/papers/2610.30882)**  
   一项研究追踪推理模型中 wait 一词的来源，发现它来自训练数据而非强化学习。 · Zhizhuo Kou … Yike Guo · arXiv 2610.30882 · 2026-10-22 · [解读](https://aisafetyhot.com/items/kqts21njqciiiq21wyl911ysn)
19. **[UniGuard: Multi-View Guardrail Learning for Cross-Interface Safety Generalization](https://arxiv.org/abs/2610.30742)**  
   UniGuard：面向跨接口安全泛化的多视图护栏学习 · Viet-Thanh Pham … Lizhen Qu · arXiv 2610.30742 · 2026-10-22 · [解读](https://aisafetyhot.com/items/zvd11nc59ye1ddceoksxz903j)
20. **[Governed Self-Evolution for Autonomous Investing: A Multi-Agent LLM System with an Invariant Core](https://arxiv.org/abs/2610.30557)**  
   Steward 是面向自主投资的多智能体 LLM 系统，九个角色化智能体联合决策，以自我修改无法触及的不变核心约束自进化。 · Yebo Feng … Yang Liu · arXiv 2610.30557 · 2026-10-22 · [解读](https://aisafetyhot.com/items/r91sjet8ufiblid0eb2czjbw6)
21. **[Network topology shapes consensus and vulnerability in LLM populations](https://arxiv.org/abs/2610.31165)**  
   研究者发现，网络拓扑既影响大语言模型群体共识的形成速度，也决定其被对抗攻击推翻的难度。 · Roberto Passaro … Luca Maria Aiello · arXiv 2610.31165 · 2026-10-22 · [解读](https://aisafetyhot.com/items/csbcm5wys7ojgj52k7ikiaf9s)
22. **[AI Risk Ontologies for the EU AI Act Compliance: AIRO, VAIR, and their Integration with DPV](https://arxiv.org/abs/2610.31380)**  
   研究者开发了 AI 风险本体 AIRO 和 AI 风险词汇表 VAIR，用于按欧盟 AI Act 要求协助高风险 AI 系统的风险管理与文档记录。AIRO 描述 AI 用例及其相关风险，VAIR 以概念分类填充 AIRO。 · Delaram Golpayegani … Dave Lewis · arXiv 2610.31380 · 2026-10-22 · [解读](https://aisafetyhot.com/items/cqurkafsoejlxunacq6wa1mji)
23. **[WildFakeToolBench: Benchmarking AI-Generated Image Detectors with Web-Sourced Image Processing](https://arxiv.org/abs/2610.31152)**  
   WildFakeToolBench：用网络来源的图像处理工具评测 AI 生成图像检测器 · Mingjie Li … Yang Zhang · arXiv 2610.31152 · 2026-10-22 · [解读](https://aisafetyhot.com/items/pw7f9pg3go3a72yrgzgebj547)
24. **[Probing and Steering for Safety-Relevant Behaviours in Large Language Models](https://arxiv.org/abs/2610.30363)**  
   论文在 Llama-3.1-8B-Instruct 上用统一流程检验激活 Probe 的设计选择如何影响对欺骗、高风险感知和谄媚三种安全相关行为的检测与 steering。 · Nimun Bajwa, Massimo Poesio · arXiv 2610.30363 · 2026-10-21 · [解读](https://aisafetyhot.com/items/cykedbl4uawd87n0qug4yqskj)
25. **[Rethinking the Evaluation of LLM Fact-Checkers](https://arxiv.org/abs/2610.30504)**  
   重新思考 LLM 事实核查器的评测 · Ayana Niwa … Satoshi Sekine · arXiv 2610.30504 · 2026-10-21 · [解读](https://aisafetyhot.com/items/k6xddkdou21cu53n4seokhvqg)
26. **[Membership Inference Attack on Private Evolution](https://arxiv.org/abs/2610.30514)**  
   研究者提出一种白盒成员推断攻击，作者称这是首个针对 Private Evolution（PE）框架底层投票算法的此类攻击。 · Daniil Filienko … Martine De Cock · arXiv 2610.30514 · 2026-10-21 · [解读](https://aisafetyhot.com/items/bk92nk4vo4j4b19oppx8unc15)
27. **[JANUS: Agentic Cross-Language Fuzzing Harness Generation for Android Native Libraries](https://arxiv.org/abs/2610.30218)**  
   JANUS 首次用智能体为 Android 原生库生成跨语言模糊测试 harness。 · Xiangyu Zhang … Sen Chen · arXiv 2610.30218 · 2026-10-21 · [解读](https://aisafetyhot.com/items/ix81za68nwy9hoje2gbqjjist)
28. **[Polarity Blindness in LLM Safety: A Systematic Study of Negation, Antonym Substitution, and Adversarial Framing](https://arxiv.org/abs/2610.27908)**  
   提出极性盲视探针，用否定与反义词替换绕过聊天模型安全护栏 · `越狱与攻击` · Diego Miguel Lozano … Nuria Oliver · arXiv 2610.27908 · 2026-10-20 · [解读](https://aisafetyhot.com/items/xoch8z7lovrsw6znh1bjv6ko7)
29. **[Attention-based Classification for Indirect Prompt Injection](https://arxiv.org/abs/2610.28988)**  
   论文作者在 AgentDojo 基准上评测发现，白盒提示注入检测方法 Attention Tracker 在多数模型家族上检测效果接近随机，并提出改进方法 AttnDA。 · Amelia Kawasaki, Stefan Lee · arXiv 2610.28988 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ftuaeamiutri4lwiu4udwyl50)
30. **[Disclosure Begets Disclosure: A Self-Reinforcing Privacy Loop in LLM Agents with Persistent Memory](https://arxiv.org/abs/2610.28315)**  
   测量持久记忆 LLM 智能体查阅记忆引发的自我强化隐私泄露循环 · `Agent 安全` · Masahiro Kaneko … Timothy Baldwin · arXiv 2610.28315 · 2026-10-20 · [解读](https://aisafetyhot.com/items/y3r8l1llcgu5y8f8sbaadjgxo)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 23 · [Agent 安全](daily-papers/topics/agent-security.md) 17 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [越狱与攻击](daily-papers/topics/jailbreak.md) 7 · [隐私与数据泄露](daily-papers/topics/privacy.md) 6 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
