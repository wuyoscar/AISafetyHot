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
### 2026-11-12 · 30 篇

1. **[From Attack Surface to Defense Architecture: Compositional Security for Agentic Coding Harnesses](https://arxiv.org/abs/2611.13960)**  
   研究者提出 ActiveSecHarness，一种面向智能体编码 Harness 的神经符号参考监控架构，主张 Agent 系统的安全是认知架构与权限组合的结构属性，而非单个模型的涌现属性。 · Simon Hegelich … Erik Cambria · arXiv 2611.13960 · 2026-11-10 · [解读](https://aisafetyhot.com/items/hxo137timwuvuteh0oieep2wg)
2. **[Is Your Robot's Memory Just a Clock? Temporal Shortcuts in Memory-Augmented VLA Policies](https://huggingface.co/papers/2611.14488)**  
   诊断记忆增强 VLA 策略把时间当任务进度的时间捷径失效 · Chubin Zhang, Bo An · arXiv 2611.14488 · 2026-11-10 · [解读](https://aisafetyhot.com/items/i1uhwp6msv6trdr7j4udcj2fu)
3. **[When Safety Becomes An Outlier: Understanding the Retention of LLM Safety Behaviors](https://arxiv.org/abs/2611.10971)**  
   研究者提出，安全对齐的大语言模型在微调后丢失安全行为，是因为公式化拒答串构成窄而缺乏语义支撑的离群模式，容易被后续更新覆盖，并提出 NEST 框架加以缓解。 · Binchi Zhang … Jundong Li · arXiv 2611.10971 · 2026-11-10 · [解读](https://aisafetyhot.com/items/mor99flvn7yh1vz5f2zyxhhnz)
4. **[Don't Just Trust Your Memory: Evidence-Linked Memory Reduces Memory-Induced Degradation in LLM Agents](https://huggingface.co/papers/2611.14320)**  
   研究者提出证据关联记忆系统 WikiTrace，把智能体蒸馏出的每条教训链接到来源轨迹，让智能体在行动前核验并修正记忆，减少记忆诱导退化。 · Yukyeong Lee … Sung Ju Hwang · arXiv 2611.14320 · 2026-11-10 · [解读](https://aisafetyhot.com/items/s1rh6cbqq04f1s7q5nymqi1vd)
5. **[Specify Privacy Yourself: Assessing Inference-Time Personalized Privacy Preservation Ability of Large Vision-Language Models](https://arxiv.org/abs/2611.13997)**  
   研究者提出 SPY-Bench，系统评估大型视觉语言模型（LVLM）在推理时按用户语言指令动态划定隐私边界的能力（ITP³）。 · Xingqi Wang … Jia Jia · arXiv 2611.13997 · 2026-11-10 · [解读](https://aisafetyhot.com/items/zce1si3a83ypouqzit2j50tjx)
6. **[Embodied First Exam](https://arxiv.org/abs/2611.12177)**  
   论文提出 Embodied First Exam，一个让编码智能体自行选择直接控制、代码控制或训练策略来控制机器人的统一评测框架。 · Kangrui Wang … Manling Li · arXiv 2611.12177 · 2026-11-09 · [解读](https://aisafetyhot.com/items/xvljxzgpn1qmac32o33cl9yiq)
7. **[Eliciting Harmful Capabilities by Fine-Tuning on Safeguarded Outputs](https://openreview.net/forum?id=viBAbg9ihM)**  
   提出诱导攻击：用邻域良性提示从受防护前沿模型获取输出并微调开源模型，在危险化学品合成领域恢复约 40% 的能力差距，且效果随模型能力和数据量扩展。 · `危险能力` · Jackson Kaunismaa … Erik Jones · ICLR 2026 Poster
8. **[MOAI: Module-Optimizing Architecture for non-interactive secure transformer Inference](https://arxiv.org/abs/2611.13641)**  
   研究者提出 MOAI，一种基于同态加密（HE）的非交互式安全 Transformer 推理框架，让模型可在云服务商处直接对加密输入做推理。 · Linru Zhang … Kwok-Yan Lam · arXiv 2611.13641 · 2026-11-10 · [解读](https://aisafetyhot.com/items/f6qlwtsc9ig3vf4cd4scneaza)
9. **[GARD: Gradient-Guided Adversarial Representation Defense against Backdoors in Multimodal Contrastive Learning Models](https://arxiv.org/abs/2611.14143)**  
   GARD 是针对 CLIP 等多模态对比学习模型后门的事后防御方法，无需预知攻击目标或触发器。该方法优化互补的全局与局部对抗探针以偏移干净图像表示，再将其与干净锚点重新对齐并保持图文对齐。 · Yuhong Wang … Songze Li · arXiv 2611.14143 · 2026-11-10 · [解读](https://aisafetyhot.com/items/mz4qpbona8snegsxk62w0q562)
10. **[Living constitutions: Participatory alignment for sovereign foundation models](https://arxiv.org/abs/2611.13402)**  
   研究者提出以“活宪法”实现主权基础模型的参与式对齐，把宪法制定视为类似公民科学的持续演进过程，迭代起草、测试和修订。 · Stine Lyngsø Beltoft … Lukas Galke Poech · arXiv 2611.13402 · 2026-11-10 · [解读](https://aisafetyhot.com/items/qbqltszm3tqea8yu36xne15q7)
11. **[On Private Knowledge Retrieval and Private Inference for secure multi-agent systems](https://arxiv.org/abs/2611.13696)**  
   针对 LLM 多智能体系统中的记忆投毒攻击，论文聚焦语义记忆，提出私有知识检索与私有推理作为防御方案。 · Vicenç Torra, Maria Bras-Amorós · arXiv 2611.13696 · 2026-11-10 · [解读](https://aisafetyhot.com/items/w1u5mcva6t3mcfyo2f5kdczjn)
12. **[Advancing a Global Framework for AI Safety and Governance for the Well-being of Humanity](https://arxiv.org/abs/2611.13968)**  
   世界互联网大会人工智能专委会发布报告，提出以联合国为中心建立全球 AI 安全与治理框架的制度措施和政策建议。 · Zeng Yi … Liang Hao · arXiv 2611.13968 · 2026-11-10 · [解读](https://aisafetyhot.com/items/m36oox4f0mlrwmuqq9mkhlh48)
13. **[BypassGym: A Benchmark for Evaluating AI Agents' Endpoint Defense Evasion Capabilities](https://arxiv.org/abs/2611.13684)**  
   研究者发布 BypassGym 基准，在真实端点上评估 AI 智能体绕过 EDR（端点检测与响应）的能力，作者称这是首个在真实端点上系统评估该能力的基准。 · Weifeng Yuan … Haoyu Wang · arXiv 2611.13684 · 2026-11-10 · [解读](https://aisafetyhot.com/items/vnp85ue7r9yjk47v75glfqmcn)
14. **[Say Shibboleth: Fingerprinting the LLMs and Harnesses Behind Agentic Attacks](https://arxiv.org/abs/2611.12386)**  
   研究者提出对智能体网络攻击进行指纹识别的方法，可从遥测中推断攻击者所用的大语言模型版本与 harness。 · Dario Pasquini … Sergej Epp · arXiv 2611.12386 · 2026-11-09 · [解读](https://aisafetyhot.com/items/imdpqxtgwp2hz4i1ad304tfpz)
15. **[StealthyPoison: Manipulating LLM Agent Behavior through Procedural Poisoning of Third-Party Skills](https://arxiv.org/abs/2611.12155)**  
   提出 StealthyPoison 攻击，投毒第三方技能并操纵 Agent 选择执行 · Jingfen Qiao … Evangelos Kanoulas · arXiv 2611.12155 · 2026-11-09 · [解读](https://aisafetyhot.com/items/dzai4y099atrhk4d0u5xs6ns2)
16. **[Ultrasound-Assisted Biometric Watermarking Against Face Video Deepfakes](https://arxiv.org/abs/2611.11800)**  
   研究提出 UltraGuard，一种利用手机内置扬声器和麦克风发射超声波、采集生物特征并融合视频时空动态特征的人脸视频水印方法，可在传输中实时嵌入。 · Guodong Liu … Guihai Chen · arXiv 2611.11800 · 2026-11-09 · [解读](https://aisafetyhot.com/items/fpudp2wl4uuo98jph9nc8677h)
17. **[How Much Training-Inference Mismatch Can On-Policy Distillation Tolerate?](https://huggingface.co/papers/2611.11450)**  
   论文研究了在线策略蒸馏（OPD）能容忍多大的训练-推理失配，发现其可容忍量化推理和异步 rollout 带来的较大失配而训练质量无明显损失，失配更高时才退化，呈现经验性失配预算。 · Cong Yu … Tuo Shi · arXiv 2611.11450 · 2026-11-08 · [解读](https://aisafetyhot.com/items/md3e0i1z1k2uaq5l2jnhv2u75)
18. **[RoCoMark: Robust Code Watermarking Against LLM-Based Functionality-Preserving Rewriting Attacks](https://arxiv.org/abs/2611.11399)**  
   RoCoMark：抵御基于 LLM 的功能保持重写攻击的鲁棒代码水印 · Hongjie Zhang … Xinpeng Zhang · arXiv 2611.11399 · 2026-11-08 · [解读](https://aisafetyhot.com/items/pj0pigw74cpjzdf64x77i2fza)
19. **[TERM: Target-Free Jailbreak Defense via Entropy-Guided Residual Modulation](https://arxiv.org/abs/2611.13577)**  
   TERM 是一种推理时越狱防御方法，以每个提示词自身的 prefill 基线校准注意力熵偏差，据此自适应调制模型残差更新，无需预设安全方向。 · Yunkai Dang … Wenbin Li · arXiv 2611.13577 · 2026-11-10 · [解读](https://aisafetyhot.com/items/lejg6rhzbrgk9gogmnxhlthte)
20. **[SafeRoute-MAS: Coverage-Aware and Risk-Calibrated Message Routing for Multi-Agent Scientific Reasoning](https://arxiv.org/abs/2611.13454)**  
   SafeRoute-MAS 是面向多智能体科学推理的覆盖感知、风险校准消息路由方法，决定保留全部专家消息还是删除一条。 · Zhiming Xue … Jing Yang · arXiv 2611.13454 · 2026-11-10 · [解读](https://aisafetyhot.com/items/x0zb3ef4ymhv7tnw9gaj69yh7)
21. **[Data-Efficient Unlearning-Based Backdoor Detection in Federated Learning](https://arxiv.org/abs/2611.13491)**  
   SURA：联邦学习中基于遗忘的数据高效后门检测 · Dowon Kim … Changhee Joo · arXiv 2611.13491 · 2026-11-10 · [解读](https://aisafetyhot.com/items/rgb28oludt1lpms4uoxqthe9v)
22. **[Enmo Safety: External, Non-invasive, Model-agnostic Oversight for Off-the-Shelf Language Models](https://arxiv.org/abs/2611.10099)**  
   研究者提出 Enmo Safety，一种不改动模型权重的外部安全护栏，用确定性输入评估、触发匹配的安全指引、不可信内容标注和输出护栏包裹聊天模型，由反射模型把失败转化为每轮一次的有界更新，仅保留降低危害且不提高良性提示拒答的更新。 · Mohammed Nayeem Khan … Vrishank Tiwari · arXiv 2611.10099 · 2026-11-10 · [解读](https://aisafetyhot.com/items/pfj84ivzzuc9qmab5uikbis7n)
23. **[Tree-Ising: Repairing Language Models with Bit-Level Ising Edits](https://huggingface.co/papers/2611.14210)**  
   提出 Tree-Ising 位级 Ising 编辑方法，修复语言模型的推理循环缺陷 · Hadi Salloum, Ammar Ali · arXiv 2611.14210 · 2026-11-10 · [解读](https://aisafetyhot.com/items/en2xxe5doqpquzgud0dp8029b)
24. **[POEM: Output-Relative Block-Sparse Attention for Long-Context Prefilling](https://arxiv.org/abs/2611.13578)**  
   研究者提出 TERM（Target-free Entropy-guided Residual Modulation），一种针对越狱攻击的推理时防御方法。 · Haoyi Wu … Wenbin Li · arXiv 2611.13578 · 2026-11-10 · [解读](https://aisafetyhot.com/items/tvg8lekapkbwavsob032hm6r3)
25. **[Sable: A Small-Field Sumcheck Argument for Bit-Exact Inference of Large Language Models](https://huggingface.co/papers/2611.14083)**  
   研究者提出论证系统 Sable，可在单张 GPU 上证明某个已承诺的整数量化 Transformer 对给定提示逐位产生给定 token 序列，代码开源于 https://github.com/moonmath-ai/Sable。 · Tomer Solberg · arXiv 2611.14083 · 2026-11-10 · [解读](https://aisafetyhot.com/items/clidm1fhbsytc9zysqp1ufz0e)
26. **[zkARc: Succinctly Verifiable Proofs for Neurosymbolic Natural Language Formalization and Verification](https://arxiv.org/abs/2611.10031)**  
   研究者提出 zkARc，一个将 Automated Reasoning checks（ARc）的每个阶段包裹在独立、简洁可验证零知识证明中的模块化框架，使第三方无需重跑流水线或信任运营方即可核验策略确实被执行。 · Wyatt Benno … Benjamin Kiesl-Reiter · arXiv 2611.10031 · 2026-11-10 · [解读](https://aisafetyhot.com/items/nll7vnhz59v04odjtrsijgei8)
27. **[Structured Confidence Perturbation via Fisher Geometry for Adversarial Training](https://arxiv.org/abs/2611.14046)**  
   针对对抗训练中推高损失却不改变置信度结构的“伪攻击”，研究者提出交叉熵与 KL 散度混合目标，并在置信度流形上生成最大化分布距离的扰动。 · Chenlong Wei … Xiaobo Jin · arXiv 2611.14046 · 2026-11-10 · [解读](https://aisafetyhot.com/items/rw3dya129dewoex5spao3cd3r)
28. **[MMDM: Measuring Massive Multitask Decision Making](https://huggingface.co/papers/2611.14309)**  
   MMDM：衡量大规模多任务决策的基准 · Junhao Shen … Hong Cheng · arXiv 2611.14309 · 2026-11-10 · [解读](https://aisafetyhot.com/items/nb06qtvucpc1cjtnyw86iiuj5)
29. **[Transparency Disclosures for Chain-of-Thought Monitorability](https://arxiv.org/abs/2611.13873)**  
   论文主张前沿 AI 开发者应披露特定指标，使思维链（CoT）监控面临的威胁可追踪，并促进各方协调保护 CoT 可监控性。 · Jacob Davies, Theo Bearman · arXiv 2611.13873 · 2026-11-10 · [解读](https://aisafetyhot.com/items/u17tusdehnda5a0pb5g2aq7gh)
30. **[Comparative Analysis of Agent Evaluation Frameworks: Stability, Detection, and Discovery in Enterprise Analytics Agents](https://arxiv.org/abs/2611.14493)**  
   研究者在受控环境中，将基于轨迹的 LLM 评审、纯文本 LLM 评审加红队测试和确定性启发式三类评测框架，在两个企业分析型 Agent 的冻结执行轨迹上进行三阶段对比。 · Howard Zhang … Lily Miao · arXiv 2611.14493 · 2026-11-10 · [解读](https://aisafetyhot.com/items/tpfhrol6ptzlb6ydlgp4pke8k)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 33 · [Agent 安全](daily-papers/topics/agent-security.md) 33 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 13 · [后门与投毒](daily-papers/topics/backdoor.md) 10 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
