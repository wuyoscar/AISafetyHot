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
### 2026-10-25 · 30 篇

1. **[安全探针的缩放定律](https://arxiv.org/abs/2610.30678)**  
   研究者提出安全探针的缩放定律，表明探针性能可由模型规模和标注数量提前预测。 · Yuchen Wu, Jerry Wei · arXiv 2610.30678 · 2026-10-22 · [解读](https://aisafetyhot.com/items/o4ob9mj42yyzy9qyjw5wflla6)
2. **[VerifierBench: Benchmarking the Generation of Executable Verifiers for LLM Agents](https://arxiv.org/abs/2610.28679)**  
   VerifierBench：评测 LLM 智能体生成可执行验证器的基准 · Jianing Yin … Daoan Zhang · arXiv 2610.28679 · 2026-10-19 · [解读](https://aisafetyhot.com/items/lynjpqi3296gxlhaatr0jyys1)
3. **[Model Organisms of Collusion: Corrective Transfer in Untrusted Monitors](https://arxiv.org/abs/2610.30582)**  
   在 AI 控制（AI control）协议中，抓住一次共谋后仅重训监控器，就能减少但不能消除尚未被抓到的共谋。 · Juan-Pablo Rivera … John Hughes · arXiv 2610.30582 · 2026-10-22 · [解读](https://aisafetyhot.com/items/oedcvsx0j8q1sv0dli2dulg2m)
4. **[Not All Tokens Are Equal: Region-Aware Consistency Repair of Backdoors in MLLMs](https://arxiv.org/abs/2608.24354v1)**  
   提出 RACER，用区域感知一致性对抗微调去除多模态大模型后门 · Jiali Wei … Ting Liu · arXiv 2608.24354 · 2026-08-25 · [解读](https://aisafetyhot.com/items/sx7li5drana8dybvi51erfbqu)
5. **[Tripwire: Triggering Aligned Refusal via Statistically Certified Safety Neurons](https://arxiv.org/abs/2608.14392v1)**  
   提出 Tripwire，识别安全神经元并钳制激活以触发拒答 · Wei Zhao … Jun Sun · arXiv 2608.14392 · 2026-08-14 · [解读](https://aisafetyhot.com/items/gcpu2us8d40jky223k85kfwei)
6. **[Practice Makes Unsafe: Skill Misevolution in Self-Improving LLM Agents](https://arxiv.org/abs/2608.12851)**  
   提出 SkillMisevo-Bench，量化自改进 Agent 的技能误演化 · Xutao Mao … Cong Wang · arXiv 2608.12851 · 2026-08-13 · [解读](https://aisafetyhot.com/items/iep2ll4t35znwumyxpxrt88uj)
7. **[Jailbreaking Frontier Foundation Models Through Intention Deception](https://arxiv.org/abs/2604.24082)**  
   提出多轮意图欺骗越狱 iDecep，用良性意图伪装引出有害内容 · `越狱与攻击` · Xinhe Wang … Yaqi Xie · arXiv 2604.24082 · 2026-04-27 · [解读](https://aisafetyhot.com/items/lii77tpeqz6p7eqxxca99l334)
8. **[Adaptive Prompt Embedding Optimization for LLM Jailbreaking](https://arxiv.org/abs/2604.24983)**  
   提出 PEO，直接优化原提示词嵌入实现白盒越狱 · `越狱与攻击` · Miles Q. Li … Ebrahim Bagheri · arXiv 2604.24983 · 2026-04-27 · [解读](https://aisafetyhot.com/items/fd8rnnvqd3q5kg2ti6fs63hml)
9. **[Spherical Watermark: Encryption-Free, Lossless Watermarking for Diffusion Models](https://openreview.net/forum?id=2eAGrunxVz)**  
   提出免加密无损水印框架，将水印码映射到单位球面恢复高斯噪声，保持视觉保真并提升溯源性与抗攻击鲁棒性。 · `防御与护栏` · Xiaoxiao Hu … Zhenxing Qian · ICLR 2026 Oral
10. **[Jailbreaking the Matrix: Nullspace Steering for Controlled Model Subversion](https://arxiv.org/abs/2604.10326)**  
   提出 HMNS，通过注意力头掩码与零空间注入实现机制级越狱 · `越狱与攻击` · Vishal Pramanik … Sumit Kumar Jha · arXiv 2604.10326 · 2026-04-11 · [解读](https://aisafetyhot.com/items/f089wbhtzg8w53dtu6vrainbc)
11. **[Concept Removal Guidance: Evidence-Calibrated Negative Guidance for Safe Diffusion Sampling](https://openreview.net/forum?id=BSDvEh7oqy)**  
   提出免训练的 CRG 方法，每步从噪声预测估计违禁概念存在度并自适应校准负引导强度，在红队基准上降低攻击成功率同时保持正常生成质量。 · `防御与护栏` · Yoonseok Choi … Kee-Eung Kim · ICML 2026 spotlight
12. **[Verbalizing Activation Differences with Natural Language Autoencoders](https://arxiv.org/abs/2610.30934)**  
   研究显示，自然语言自编码器（NLA）能在训练设定之外泛化，在来自三个家族的四个模型上，实验对四个相关问题均给出大体肯定的证据。 · Andrea Blasi Núñez … Lukas Galke Poech · arXiv 2610.30934 · 2026-10-22 · [解读](https://aisafetyhot.com/items/u63o0ohkkml05j1fcwiqlfgwf)
13. **[Local Allow, Global Deny: Why Per-Action Authorization Does Not Compose in LLM Agents](https://arxiv.org/abs/2610.27620)**  
   刻画逐动作授权的组合失败，并用 AL-SYNTH 合成最小证人 · `Agent 安全` · Anmol Pandey … Carsten Maple · arXiv 2610.27620 · 2026-10-20 · [解读](https://aisafetyhot.com/items/un7u9wq6jn9gwwfwduloq2yc8)
14. **[More Memory, Worse Agents: Error Reproduction and Anti-Persistence in LLM Agents](https://huggingface.co/papers/2610.27406)**  
   提出 Anti-Persistence，用后丢弃抽象以限制 Agent 记忆错误再现 · Ruhan Wang … Dongruo Zhou · arXiv 2610.27406 · 2026-10-19 · [解读](https://aisafetyhot.com/items/z0geuf1q18hkgjo4ao7gdv9s2)
15. **[African Languages AI Safety Readiness Report](https://arxiv.org/abs/2610.27269)**  
   评估哪些非洲语言适合纳入 AI 安全基准 · Israel Abebe Azime … David Ifeoluwa Adelani · arXiv 2610.27269 · 2026-10-19 · [解读](https://aisafetyhot.com/items/r2gdabjjul22q8tjqbykm6l6p)
16. **[Harm Is Behavioural, Moderation Is Lexical: How Language and Culture Decide Whom Automated Safety Systems Protect and Whom They Silence](https://arxiv.org/abs/2610.31047)**  
   伤害是行为性的，审核是词汇性的：语言与文化如何决定自动化安全系统保护谁、让谁沉默 · Gabriel Lars Sabadin … Sarah Kingston · arXiv 2610.31047 · 2026-10-22 · [解读](https://aisafetyhot.com/items/q6ing53gaifgcdfmo2ads8lma)
17. **[Who Is Sycophantic to Whom? Confident LLMs, Human Deference, and the Collapse of Trust Calibration](https://arxiv.org/abs/2610.31579)**  
   展示自信但错误的 LLM 导致用户吸收假事实且信任校准崩塌 · Deepthika S … B. Sankar · arXiv 2610.31579 · 2026-10-22 · [解读](https://aisafetyhot.com/items/m4ru5r1a6zy0h6f97td9dbn8b)
18. **[Questioning Instrumental Convergence in RLVR: Checkpoint Evidence from OLMo-3](https://arxiv.org/abs/2610.31624)**  
   质疑 RLVR 中的工具性收敛：来自 OLMo-3 的检查点证据 · Barış Alparslan … Caleb Petterson · arXiv 2610.31624 · 2026-10-22 · [解读](https://aisafetyhot.com/items/i9qrmcihz21vlweo23ivgbzug)
19. **[What Lies Beyond Perception: A Partition Theory of the Limits of AI Evaluation and Oversight](https://arxiv.org/abs/2610.30803)**  
   Ahmed M. Mahran 在 arXiv 论文提出评测的划分理论，证明行为评测最多只能证明模型区分能力的下限而非上限。 · Ahmed M. Mahran · arXiv 2610.30803 · 2026-10-22 · [解读](https://aisafetyhot.com/items/otz8xlvlfhu2bjwj5x2s3eqae)
20. **[SCOPE: Compiling Natural-Language Policies into Neurosymbolic Predicate Programs](https://huggingface.co/papers/2610.31062)**  
   SCOPE 提出把自然语言策略编译成可执行的神经符号谓词程序，用于 LLM 智能体在多轮对话和工具调用轨迹上的策略执行。 · Arnon Mazza, Elad Levi · arXiv 2610.31062 · 2026-10-22 · [解读](https://aisafetyhot.com/items/hd3yw3578mkt5smm1uilpv24m)
21. **[模拟控制评估（Simulated Control Evals）](https://arxiv.org/abs/2610.31593)**  
   论文提出模拟控制评估（SCEs），用语言模型模拟工具响应来替代真实环境，从而在更多环境中开展控制评估。 · Jeffrey Olmo … Tyler Tracy · arXiv 2610.31593 · 2026-10-22 · [解读](https://aisafetyhot.com/items/m8oc7q19rn17k6etmwdmyiiwh)
22. **[From Clinical Judgment to Checkable Rules: Clinician-Led Guardrails for Mental-Health Chatbots](https://arxiv.org/abs/2610.30690)**  
   研究者提出一种临床医生主导的心理健康聊天机器人护栏，由两名临床医生定义并裁定规则库的四项安全检查，规则库经形式化验证后作用于 LLM 输出，每次判定可由一条命名规则和十六项事实复算。 · Chenhan Lyu … Amir Rahmani · arXiv 2610.30690 · 2026-10-22 · [解读](https://aisafetyhot.com/items/um8nxo5fn0dhmnoy8n4dwxqzb)
23. **[TESSA: A Governance-Oriented Custom GPT for SME Guidance under the EU AI Act: Design, Implementation, and Evaluation](https://arxiv.org/abs/2610.30822)**  
   TESSA：为中小企业提供欧盟《人工智能法案》指导的治理导向 Custom GPT 的设计、实现与评估 · Chalisa Veesommai Sillberga … Pekka Abrahamssona · arXiv 2610.30822 · 2026-10-22 · [解读](https://aisafetyhot.com/items/ugxu9yeti9t2xd319kuizg9ae)
24. **[Verus-Insight: Towards Explainable Artifact Detection in AI-Generated Videos](https://huggingface.co/papers/2610.30866)**  
   Verus-Insight 将 AI 生成视频的伪影检测拆解为检查规划、证据验证与证据聚合三项能力，用人类锚定的全流程监督和渐进式能力训练检测器。 · Zhuoran Zhang … Wenjing Yang · arXiv 2610.30866 · 2026-10-22 · [解读](https://aisafetyhot.com/items/yxykao3xoajll0lum48rss2di)
25. **[What Does AI Success Look Like? A Mixed-Methods Analysis of Supranational AI Governance Instruments](https://arxiv.org/abs/2610.31030)**  
   AI 成功是什么样子？超国家 AI 治理文件的混合方法分析 · Delaram Golpayegani … Dave Lewis · arXiv 2610.31030 · 2026-10-22 · [解读](https://aisafetyhot.com/items/px5wfwn8112f43p92n73gapek)
26. **[Faithful Latent Harm Monitors Work No Better Than the Models Own Behaviour at a Matched False Alarm Rate](https://arxiv.org/abs/2610.30727)**  
   分析忠实潜空间危害监控器是否优于模型自身拒答行为 · Abhishek Mishra … Suyash Maniyar · arXiv 2610.30727 · 2026-10-22 · [解读](https://aisafetyhot.com/items/m7zd6qg6r4kt175ik46imr3n8)
27. **[VERA: A Responsible AI Dashboard for Assessing LLM Deployments in Light of the EU AI Act](https://arxiv.org/abs/2610.31588)**  
   研究者发布开源、可自托管的负责任 AI 评估面板 VERA，用于依据欧盟《人工智能法案》评估大语言模型部署，已在一家欧洲大型银行投入使用。 · Robin Quériaux … Jérôme Lebecq · arXiv 2610.31588 · 2026-10-22 · [解读](https://aisafetyhot.com/items/nh39vqsy4glxrfi1uzn2n0i6u)
28. **[Disentangling Robustness and Sycophancy in Multilingual LLMs](https://arxiv.org/abs/2610.30696)**  
   研究者提出 SC-matrix，将模型在无压力下能否答对（能力）与受压后能否坚持正确答案（谄媚）交叉诊断，用以区分多语言 LLM 同意用户错误前提时究竟是谄媚还是该语言能力不足。 · Rhitabrat Pokharel, Ameeta Agrawal · arXiv 2610.30696 · 2026-10-22 · [解读](https://aisafetyhot.com/items/tva77tmm3vyckta6qll59r2xf)
29. **[Harmful Responses Are Jailbreak Templates: Transferring Autoregressive Jailbreaks to Diffusion Language Models](https://arxiv.org/abs/2610.31331)**  
   研究者提出 RMT-Jailbreak 框架，可将自回归模型上的越狱攻击迁移到扩散大语言模型（dLLM）。 · Jinwei Gan … Qing Gu · arXiv 2610.31331 · 2026-10-22 · [解读](https://aisafetyhot.com/items/hxga976s05g0ladwppanf1r1h)
30. **[Conflicted Records: Typed Adversarial Contracts for Auditable LLM Output Quality Enforcement](https://arxiv.org/abs/2610.29669)**  
   论文提出 BiasGuard-D：跨模型家族的两个对抗角色交换类型化声明文档，三模型仲裁团多数表决，实现可审计的 LLM 输出质量管控。 · Kardelen Subasi, Jarosław A. Chudziak · arXiv 2610.29669 · 2026-10-21 · [解读](https://aisafetyhot.com/items/tsmyeminndmdr92oef37srb38)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 25 · [Agent 安全](daily-papers/topics/agent-security.md) 18 · [越狱与攻击](daily-papers/topics/jailbreak.md) 10 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [隐私与数据泄露](daily-papers/topics/privacy.md) 6 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
