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
### 2026-10-29 · 30 篇

1. **[A Holistic Approach to Undesired Content Detection in the Real World](https://arxiv.org/abs/2208.03274)**  
   研究者提出一套面向真实世界内容审核的分类系统构建方法，覆盖从分类体系设计到模型鲁棒性的完整流程。 · Todor Markov … Lilian Weng · arXiv 2208.03274 · 2026-10-27 · [解读](https://aisafetyhot.com/items/mo5i357a4015misvv6w3kelcj)
2. **[Can Open Be Too Open? On the Security and Trustworthiness of Fully Transparent LLMs](https://arxiv.org/abs/2610.35199v1)**  
   论文论证完全透明的大语言模型并不必然更安全可信。 · Sheila Zingg … Srdjan Čapkun · arXiv 2610.35199 · 2026-10-26 · [解读](https://aisafetyhot.com/items/a7x526x6kz7g43k9yg2gijtn3)
3. **[The Target Agent Is Its Own Best Critic but a Poor Proposer: Self-Improved Red Teaming](https://arxiv.org/abs/2610.34965v1)**  
   目标智能体是自己最好的批评者却是糟糕的提案者：自我改进的红队测试 · Mintong Kang … Bo Li · arXiv 2610.34965 · 2026-10-26 · [解读](https://aisafetyhot.com/items/vyzwgmaejh6g9mwngvdg2qgpb)
4. **[Follow the Gradient: Tracing Safety Degradation Back to Training Data](https://arxiv.org/abs/2610.37481)**  
   DatologyAI 与 UIUC 研究者提出 SimpleLoRIF，一种可扩展的梯度归因方法，用于找出微调数据中看似无害却会削弱安全对齐的样本。 · Saket Reddy … Pratyush Maini · arXiv 2610.37481 · 2026-10-27 · [解读](https://aisafetyhot.com/items/ekb3ndvi6w71lzffewp0uqgma)
5. **[Heads of Security: Learned Attention Gates Improve Prompt Injection Robustness](https://arxiv.org/abs/2610.37657)**  
   研究者提出 Heads of Security（HoS），一种通过学习各注意力头在可信与不可信 token 之间的注意力分配来强制指令与数据分离的提示注入防御。 · Igor Shilov … Yves-Alexandre de Montjoye · arXiv 2610.37657 · 2026-10-27 · [解读](https://aisafetyhot.com/items/wsp5i0y0o9k7bvpjfrddk157l)
6. **[Measuring the Robustness of Audio Deepfake Detection under Real-World Corruption](https://arxiv.org/abs/2503.17577)**  
   测量音频深度伪造检测在真实世界失真下的鲁棒性 · Xiang Li … Wenqi Wei · arXiv 2503.17577 · 2026-10-27 · [解读](https://aisafetyhot.com/items/ijy5qj3zmzbjd8feguo1x6kmi)
7. **[Did the Model Use That? Counterfactual Training Boosts Self-Attribution in Language Models](https://huggingface.co/papers/2610.35295)**  
   论文研究语言模型能否自我归因，即在回答中标明何时受到随问题提供的信息影响。作者测试十一个前沿模型，发现大多数很少标注真正影响答案的信息，其余模型则会标注未产生影响的信息。 · Zikai Zhou … Monica S. Lam · arXiv 2610.35295 · 2026-10-26 · [解读](https://aisafetyhot.com/items/q659vwyp3bd3ndo22xqq138ul)
8. **[Compatibility and future-proof testing for multi-agent systems](https://arxiv.org/abs/2610.36289)**  
   研究者针对独立开发的自主智能体（如自动驾驶车辆）在共享环境中须满足安全与任务完成等联合兼容要求的问题，提出一种双层结构，由监管方发布种子智能体，各开发者独立测试其智能体与所有种子兼容智能体保持兼容，作者将这一性质称为 future-proofness。 · Yueshan Li … Emilio Frazzoli · arXiv 2610.36289 · 2026-10-26 · [解读](https://aisafetyhot.com/items/fe98a7qffrig3s58a7qyrvsyz)
9. **[A Certified Robustness Framework for Backdoor Poisoning Attacks using $f$-Divergences](https://arxiv.org/abs/2610.34934v1)**  
   研究者提出一个基于 f-散度的认证鲁棒性框架，用于防御数据投毒与后门投毒攻击。 · Evan Rose, Alina Oprea · arXiv 2610.34934 · 2026-10-26 · [解读](https://aisafetyhot.com/items/n0igbgvd2cf10ng50mw6as93k)
10. **[Rethinking Verification in Agent Harnesses](https://huggingface.co/papers/2610.34577)**  
   重新思考智能体脚手架中的验证 · Zhengxin Zhang … Jingren Zhou · arXiv 2610.34577 · 2026-10-25 · [解读](https://aisafetyhot.com/items/w614calrd6jesqasxu4xg0ncz)
11. **[InteractiveWorld: A Verifiable Human-Centric Environment for Building Better Interactive MLLM Assistants](https://huggingface.co/papers/2610.33966)**  
   研究者提出 InteractiveWorld，一个可验证的闭环模拟环境与基准，用于评估多模态大语言模型能否可靠地指导人类完成物理任务，作者称这是首个支持人类与 AI 助手闭环交互的可验证环境。 · Qinsi Wang … Qi Qian · arXiv 2610.33966 · 2026-10-25 · [解读](https://aisafetyhot.com/items/nyv579dci2k9dq4iannrryhow)
12. **[SEEK: Skill Extraction with Evolving Knowledge against Frontier Science Agents](https://arxiv.org/abs/2610.34365)**  
   提出演化知识技能提取攻击 SEEK · Cheng Gui … Wei-Ying Ma · arXiv 2610.34365 · 2026-10-25 · [解读](https://aisafetyhot.com/items/unxfurm12wzo1ppzqp2axhifo)
13. **[Δτ-Bench: Pushing Agents Toward a Moving Capability](https://huggingface.co/papers/2610.34238)**  
   Δτ-Bench：推动 Agent 迈向不断变化的能力前沿 · Shuofei Qiao … Emine Yilmaz · arXiv 2610.34238 · 2026-10-25 · [解读](https://aisafetyhot.com/items/jocnr9jtom2lukf877t0lbw22)
14. **[Continual Learning Exam: Benchmarking Long-Horizon RSI and Experiential Learning in LLM Agents](https://huggingface.co/papers/2610.33956)**  
   研究者发布 Continual Learning Exam（CLE）基准，用于评测 LLM 智能体的长程持续学习与经验驱动的自我改进能力。 · Haoyu Zhao … Jun Wang · arXiv 2610.33956 · 2026-10-25 · [解读](https://aisafetyhot.com/items/stf97czp06i0in9yfxd6ki9y3)
15. **[Learning to Follow In-Context Watermark Instructions via Self-Distillation](https://arxiv.org/abs/2608.29030)**  
   提出 SDLP 与 GRPO，训练模型遵循上下文水印指令 · Yepeng Liu … Yuheng Bu · arXiv 2608.29030 · 2026-08-29 · [解读](https://aisafetyhot.com/items/xld7y6ghilfzvjbwjgq3sj79i)
16. **[Safe to Resume? Breaking Execution Continuity of Agent Execution via Rollback](https://arxiv.org/abs/2608.29381)**  
   提出利用检查点回滚破坏 Agent 执行连续性的攻击 · `Agent 安全` · Guanlong Wu … Yinqian Zhang · arXiv 2608.29381 · 2026-08-29 · [解读](https://aisafetyhot.com/items/t30e9qm3gfx540c6xwtbor0xf)
17. **[REPLICANT: Learning Policies for Evading and Hardening Malware Detectors](https://arxiv.org/abs/2608.28499v1)**  
   研究者提出深度强化学习框架 Replicant，在严格的仅标签黑盒威胁模型下学习规避机器学习恶意软件检测器的策略。 · Shae McFadden … Fabio Pierazzi · arXiv 2608.28499 · 2026-08-28 · [解读](https://aisafetyhot.com/items/z6vlhpliwisc1895otbelt9ww)
18. **[Semantic Watermarking with Order-Robust Detection over Sub-sentence Units](https://arxiv.org/abs/2608.27666v1)**  
   研究者提出针对语义水印的嵌入位移攻击 EDA，并设计出在子句单元上做顺序鲁棒检测的新方案 k-SwordStamp。 · Abdulrahman Diaa … Florian Kerschbaum · arXiv 2608.27666 · 2026-08-27 · [解读](https://aisafetyhot.com/items/fe05vled3t4t8werbqxoojw3r)
19. **[CodeMechanic: Bug-Property-Guided Program Mitigation](https://arxiv.org/abs/2608.22275v1)**  
   CodeMechanic：缺陷属性引导的程序缓解 · Han Zheng … Mathias Payer · arXiv 2608.22275 · 2026-08-23 · [解读](https://aisafetyhot.com/items/m55trecob5wbvxwkaxt99uw34)
20. **[Comprehensive AI governance requires addressing non-model gains](https://arxiv.org/abs/2606.00047v1)**  
   一篇 arXiv 立场论文提出，当能力进步越来越多由独立于基座模型进展的“非模型收益”（non-model gains）驱动时，以模型层为中心的前沿 AI 治理效力会下降。 · Arthur Goemans … Allan Dafoe · arXiv 2606.00047 · 2026-05-01 · [解读](https://aisafetyhot.com/items/jw5pck6rspgdv3sy9qbje0lji)
21. **[Code World Model Preparedness Report](https://arxiv.org/abs/2605.00932v2)**  
   Meta 在 Code World Model（CWM）准备情况报告中称，发布前评估未发现该代码模型带来超出当前 AI 生态的前沿风险，因此以开放权重发布。 · Daniel Song … Summer Yue · arXiv 2605.00932 · 2026-05-01 · [解读](https://aisafetyhot.com/items/frhuciyaq5o91u29mu9ba6w7i)
22. **[BabelSafe: A Policy-Grounded Multilingual Safety Benchmark for LLMs](https://arxiv.org/abs/2605.00689v2)**  
   BabelSafe：以政策为依据的多语言大模型安全基准 · Yunhan Zhao … Bo Li · arXiv 2605.00689 · 2026-05-01 · [解读](https://aisafetyhot.com/items/tqeb9s0fssz1147o8t89xqntn)
23. **[Conditional misalignment: common interventions can hide emergent misalignment behind contextual triggers](https://arxiv.org/abs/2604.25891v1)**  
   论文提出并验证“条件性错位”（conditional misalignment）：能减少或消除涌现错位（emergent misalignment）的常见干预，只是把错位隐藏在与训练数据相似的情境触发器背后。 · Jan Dubiński … Owain Evans · arXiv 2604.25891 · 2026-04-28 · [解读](https://aisafetyhot.com/items/lwbx09wtap0e2wqsawx02rcd6)
24. **[Norm Enforcement for AI Agents: Robustly Shaping Behavior in Multi-Agent Systems](https://neurips.cc/virtual/2026/poster/151090)**  
   研究语言模型智能体的规范执行机制，发现简单机制会被未对齐智能体利用，提出基于可靠性估计与递增惩罚的机制，在三个模拟环境中抵抗利用。 · `Agent 安全` · Yaowen Ye, Jacob Steinhardt · NeurIPS 2026 spotlight
25. **[ShieldNet: Network-Level Guardrails against Emerging Supply-Chain Injections in Agentic Systems](https://arxiv.org/abs/2604.04426v1)**  
   研究者提出网络级护栏框架 ShieldNet，通过监测真实网络交互而非表层工具痕迹来检测智能体系统中的供应链投毒。 · Zhuowen Yuan … Bo Li · arXiv 2604.04426 · 2026-04-06 · [解读](https://aisafetyhot.com/items/n4wurw849g5djoeia5webymdg)
26. **[Low Rank Adaptation for Adversarial Perturbation](https://arxiv.org/abs/2604.27487v1)**  
   研究者从理论和实验上表明，对抗扰动具有内在的低秩结构，并据此提出更高效的黑盒对抗攻击方法。论文覆盖多种攻击方法、模型架构和数据集进行验证。 · Han Liu … Ning Zhang · arXiv 2604.27487 · 2026-04-30 · [解读](https://aisafetyhot.com/items/geunysbahrxbpk9pwiug5us7q)
27. **[TwinGate: Stateful Defense against Decompositional Jailbreaks in Untraceable Traffic via Asymmetric Contrastive Learning](https://arxiv.org/abs/2604.27861v1)**  
   TwinGate 是有状态双编码器防御框架，用非对称对比学习在不可追踪的匿名请求流中识别分解式越狱。它将意图一致但语义不同的恶意片段聚到共享隐空间，并用并行冻结编码器抑制误报。 · Bowen Sun … Chaowei Xiao · arXiv 2604.27861 · 2026-04-30 · [解读](https://aisafetyhot.com/items/um0eaj77fw77o90jviwx9uts4)
28. **[Quantamination: Dynamic Quantization Leaks Your Data Across the Batch](https://arxiv.org/abs/2604.26505v1)**  
   研究者发现动态量化会在运行时形成侧信道，泄露与攻击者输入处于同一批次的其他用户数据，并将这一现象称为 Quantamination。动态量化在运行时根据实际输入调整量化参数。 · Hanna Foerster … Robert Mullins · arXiv 2604.26505 · 2026-04-29 · [解读](https://aisafetyhot.com/items/o4xw9x82l9u51pr3dv731swku)
29. **[Surgical Repair of Insecure Code Generation in LLMs](https://arxiv.org/abs/2604.16697v1)**  
   研究者发现大语言模型生成不安全代码并非知识缺陷，同一批模型在被直接询问时能正确识别并解释漏洞，作者将这一差距称为 Format-Reliability Gap。 · Gustavo Sandoval … Siddharth Garg · arXiv 2604.16697 · 2026-04-17 · [解读](https://aisafetyhot.com/items/lqggaszdy1oagqjpjdsm863is)
30. **[Leave My Images Alone: Preventing Multi-Modal Large Language Models from Analyzing Images via Visual Prompt Injection](https://arxiv.org/abs/2604.09024v1)**  
   研究者提出用户侧图像保护方法 ImageProtector，在分享前向图像嵌入近乎不可察觉的扰动，作为针对多模态大语言模型（MLLM）的视觉提示注入攻击，使对手用 MLLM 分析受保护图像时模型持续生成拒答回复。 · Zedian Shao … Neil Zhenqiang Gong · arXiv 2604.09024 · 2026-04-10 · [解读](https://aisafetyhot.com/items/qisbg33dv7cyqkvcnxo7xj3vv)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 30 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [隐私与数据泄露](daily-papers/topics/privacy.md) 11 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
