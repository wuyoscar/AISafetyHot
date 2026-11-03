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
### 2026-11-04 · 30 篇

1. **[The Promises and Limitations of Evaluation-Based AI Governance: Evidence from Expert Interviews](https://arxiv.org/abs/2611.00465)**  
   评测型 AI 治理的潜力与局限：来自专家访谈的证据 · Lily Stelling … David Krueger · arXiv 2611.00465 · 2026-10-30 · [解读](https://aisafetyhot.com/items/e9li7ci8824gftgpxamk9drqb)
2. **[Characterizing When Language Models Take Harmful Actions to Protect Their Assigned Goals](https://arxiv.org/abs/2611.03374)**  
   论文提出目标-伤害冲突框架，把智能体失准、对齐伪装等行为统一描述为模型在保护既定目标与拒绝有害请求之间做取舍。 · Brandon Jaipersaud, Elliot Creager · arXiv 2611.03374 · 2026-11-02 · [解读](https://aisafetyhot.com/items/uh5phrtyazrubmvset1r26iia)
3. **[Cumulative and Audited Guardrail Tool Evolution for LLM Agent Safety](https://arxiv.org/abs/2611.02516)**  
   EVOLVE：面向 LLM 智能体安全的累积式可审计护栏工具演化框架 · Xiao Yang … Dacheng Tao · arXiv 2611.02516 · 2026-11-02 · [解读](https://aisafetyhot.com/items/ivn9dyr6b2gcmx5edhvq3llko)
4. **[Library of Layers (LoL): Adaptively Ordering Transformer Layers at Runtime](https://huggingface.co/papers/2611.03526)**  
   研究者提出 Library of Layers（LoL）架构，在推理时动态调整 Transformer 块的执行顺序以适配当前任务，在文本数据上预训练后，性能与稠密、深度循环和 MoE 三类基线相当。 · Abdellah Rahmani … Micah Goldblum · arXiv 2611.03526 · 2026-11-02 · [解读](https://aisafetyhot.com/items/p03kqriaflr8ahfn6sypvnuq2)
5. **[Adaptive Localization of Knowledge Negation for Continual LLM Unlearning](https://arxiv.org/abs/2611.02620)**  
   持续 LLM 遗忘方法 ALKN 在三个成熟 LLM 遗忘数据集的持续遗忘设置中，遗忘效果与效用保持均稳定超过基线方法。 · Abudukelimu Wuerkaixi … Changshui Zhang · arXiv 2611.02620 · 2026-11-02 · [解读](https://aisafetyhot.com/items/mkcsvjdyjsqwlvod73cm7x3fy)
6. **[Detect, Repair and Audit: A Hierarchical Multi-Agent Defense Against Adversarial Attacks in Energy Forecasting](https://arxiv.org/abs/2611.02310)**  
   研究者提出一种面向能源预测的分层多智能体防御框架，应对 TS-LLM 易受被篡改传感器输入影响的问题：本地控制中心用 MARL 检测并修复信号，审计 VPP 用带人工在环验证的 LLM 审计智能体。 · Zewei Shi … Surya Nepal · arXiv 2611.02310 · 2026-11-02 · [解读](https://aisafetyhot.com/items/b0wdepro5bgf78eazb12eqjdp)
7. **[VeriHarm-Bench: Measuring Harmful Success in LLM Coding Agents Verifiably](https://arxiv.org/abs/2611.03575)**  
   研究者提出 VeriHarm 自动框架并构建 VeriHarm-Bench，用可执行测试同时检验任务正确性与有害副作用。 · Wei-Lin Chen … Yu Meng · arXiv 2611.03575 · 2026-11-02 · [解读](https://aisafetyhot.com/items/r7dwf7qn2m4rtcw156qr43lz2)
8. **[Measuring AI Agents as Teammates with Collaborative Intelligence](https://huggingface.co/papers/2611.02633)**  
   用协作智能衡量 AI 智能体的队友表现 · Sean Wu … James Zou · arXiv 2611.02633 · 2026-11-02 · [解读](https://aisafetyhot.com/items/rldck5ew8pfgetoasjxgh558b)
9. **[Certifying Graph Neural Networks Against Label and Structure Poisoning](https://arxiv.org/abs/2611.03350)**  
   研究提出半监督框架 ST-GPA，用于在图数据标签和结构稀疏的条件下认证图神经网络抵御标签投毒与结构投毒。该方法为每个图分区补充伪标签和合成边，可适配不同架构并扩展到大量分区。 · Lukas Gosch … Stephan Günnemann · arXiv 2611.03350 · 2026-11-02 · [解读](https://aisafetyhot.com/items/adapw5947l0nb74wq4p1pra0h)
10. **[Towards Multi-Value Alignment via Value Localization in LLMs](https://arxiv.org/abs/2611.02503)**  
   论文提出一种通过定位大语言模型中的价值敏感注意力头，并在推理时调节激活来实现多价值对齐的方法，无需更新模型参数。 · Xueqi Ma … Sarah M. Erfani · arXiv 2611.02503 · 2026-11-02 · [解读](https://aisafetyhot.com/items/vdc7to46tlqz9t5q2qmdtcabs)
11. **[Controlling Sharpening in LLM Post-Training](https://arxiv.org/abs/2611.03146)**  
   控制大语言模型后训练中的锐化 · Simon Matrenok … Andreas Krause · arXiv 2611.03146 · 2026-11-02 · [解读](https://aisafetyhot.com/items/uzvkbcjn7us4xxd2mzf7o6501)
12. **[IdeaTaste: Do LLMs Share the Research Taste of Human Researchers?](https://huggingface.co/papers/2611.03424)**  
   IdeaTaste：LLM 是否与人类研究者共享研究品味？ · Shanshan Zhong … Chenyan Xiong · arXiv 2611.03424 · 2026-11-02 · [解读](https://aisafetyhot.com/items/nzaecukojt4sogsu9d05jwiig)
13. **[Reimagining computational quantum research with AI scientists](https://arxiv.org/abs/2611.02833)**  
   用 AI 科学家重新构想计算量子研究 · Yuxuan Du … Dacheng Tao · arXiv 2611.02833 · 2026-11-02 · [解读](https://aisafetyhot.com/items/gwpq6ixllgzaward6azlyzldi)
14. **[Hinted Scaling Laws](https://arxiv.org/abs/2611.02270)**  
   研究者提出带提示的缩放定律（hinted scaling laws），用特权信息把基准改造成难度连续的简化版本，让小模型得分高于零，使缩放定律能在小模型接近零分、无趋势可外推时进行预测。 · Suze van Adrichem … Tatsunori Hashimoto · arXiv 2611.02270 · 2026-11-01 · [解读](https://aisafetyhot.com/items/j0jd85z7zhisgx3eacmxbgeeo)
15. **[Chain-of-Thought Oversight Requires Separate Evidence for Faithfulness and Monitorability](https://arxiv.org/abs/2611.01620)**  
   论文指出，思维链监督中“推理轨迹可见即可监控”的常见假设混淆了模型内部计算、推理产物、输出与监控判断之间的不同属性，并将它们区分为推理可见性、机制忠实性、机制可定位性与行为可监控性。 · Sichao Li … Tongliang Liu · arXiv 2611.01620 · 2026-11-01 · [解读](https://aisafetyhot.com/items/ys6vlym892g4ffqbim34h70h4)
16. **[Automated alignment is harder than you think](https://arxiv.org/abs/2605.06390v3)**  
   研究者论证，作为对齐超级智能（ASI）的主流提案，随能力提升用 AI 智能体自动化越来越多的对齐研究，即使智能体没有蓄意谋划破坏，也可能产出看似可信却具灾难性误导的安全评估，导致未对齐的 AI 被无意部署。 · Aleksandr Bowkis … Geoffrey Irving · arXiv 2605.06390 · 2026-05-07 · [解读](https://aisafetyhot.com/items/u1wykn48yqtpzys7xo9z6sp3s)
17. **[PrefixGuard: Online Failure Warning and Trace-Grounded Diagnosis for LLM Agents](https://arxiv.org/abs/2605.06455v2)**  
   PrefixGuard 是一种神经符号方法，为 LLM 智能体提供在线失败预警与基于轨迹的诊断。GRU 从学习到的事件预测特定时域的失败风险，DFA 将事件历史组织为带风险标签的路径。 · Xinmiao Huang … Xiaowei Huang · arXiv 2605.06455 · 2026-05-07 · [解读](https://aisafetyhot.com/items/zmwhstiyhsvbxrpy7rajdtswt)
18. **[Narrow Secret Loyalty Dodges Black-Box Audits](https://arxiv.org/abs/2605.06846v3)**  
   构建窄秘密忠诚模型以躲过黑盒审计 · Alfie Lamerton, Fabien Roger · arXiv 2605.06846 · 2026-05-07 · [解读](https://aisafetyhot.com/items/ig76gjx3c2tr2dkulld0viyx7)
19. **[Pop Quiz Attack: Black-box Membership Inference Attacks Against Large Language Models](https://arxiv.org/abs/2605.06423v1)**  
   研究者提出 Pop Quiz Attack，一种针对大语言模型的黑盒成员推断攻击，把目标数据改写成测验式选择题，根据模型的回答推断样本是否属于训练数据。 · Zeyuan Chen … Yang Zhang · arXiv 2605.06423 · 2026-05-07 · [解读](https://aisafetyhot.com/items/u6jmg2oghwh1pheamywu5scoa)
20. **[Profiling for Pennies: Unveiling the Privacy Iceberg of LLM Agents](https://arxiv.org/abs/2605.06232v1)**  
   几美分即可画像：揭示 LLM 智能体的隐私冰山 · Jiahao Chen … Shouling Ji · arXiv 2605.06232 · 2026-05-07 · [解读](https://aisafetyhot.com/items/u57kaso59iv9gcqwnx3ua9zwz)
21. **[LoopTrap: Termination Poisoning Attacks on LLM Agents](https://arxiv.org/abs/2605.05846v1)**  
   研究者提出终止投毒攻击，向 LLM 智能体上下文注入恶意提示以扭曲其完成度判断，使智能体无法终止并陷入无界执行循环。 · Huiyu Xu … Chun Chen · arXiv 2605.05846 · 2026-05-07 · [解读](https://aisafetyhot.com/items/i22m1do2yxda2wy8y1aopm23b)
22. **[Instrumental Choices: Measuring the Propensity of LLM Agents to Pursue Instrumental Behaviors](https://arxiv.org/abs/2605.06490v1)**  
   研究者提出一个基准，用于测量基于终端的 LLM 智能体追求工具性趋同行为的倾向，这类行为包括自我保存等被推测与高能力智能体风险相关的行为。 · Jonas Wiedermann-Möller … Maksym Andriushchenko · arXiv 2605.06490 · 2026-05-07 · [解读](https://aisafetyhot.com/items/jq0nbkphbo0f4pxisg1v2xx69)
23. **[One Turn Too Late: Learning When to Intervene Against Multi-Turn Malicious Intent](https://arxiv.org/abs/2605.05630v3)**  
   研究者提出针对大语言模型多轮对话中隐藏恶意意图的防御方法，将防御建模为判断何时需要干预的问题，并定义最早致害轮次（即首次使累积交互足以促成有害行为的轮次）作为干预边界。 · Xinjie Shen … Pan Li · arXiv 2605.05630 · 2026-05-07 · [解读](https://aisafetyhot.com/items/blmzu9xiwgje6lvx7ra5zogcm)
24. **[MAGIQ: A Post-Quantum Multi-Agentic AI Governance System with Provable Security](https://arxiv.org/abs/2605.06933v2)**  
   研究者提出 MAGIQ，一个面向多智能体 AI 系统的策略定义与执行框架，采用高效的后量子密码协议并提供可证明的安全保证。 · Sepideh Avizheh … Reihaneh Safavi-Naini · arXiv 2605.06933 · 2026-05-07 · [解读](https://aisafetyhot.com/items/f7onfrgsv4yb79zd1yy3mfyqi)
25. **[Safactory: A Scalable Agentic Infrastructure for Training Trustworthy Autonomous Intelligence](https://arxiv.org/abs/2605.06230v2)**  
   Safactory 是面向可信自主智能训练的可扩展智能体工厂，整合并行仿真、可信数据与自主进化三个平台。 · Xinquan Chen … Xia Hu · arXiv 2605.06230 · 2026-05-07 · [解读](https://aisafetyhot.com/items/jiipxtxy7nauyqcrlaf3xqi9e)
26. **[MemHarmBench: Evaluating Cross-Session Prompt Injection in Memory-Persistent AI Agents](https://arxiv.org/abs/2611.01700v1)**  
   研究团队提出 MemHarmBench，这是一个以受害方为中心、用于评估记忆持久型 AI 智能体跨会话提示注入的基准，并公开了代码。该基准把潜在受害方分为用户、工作区或项目所有者、外部相关方三类。 · Zhihua Wang … Xingjun Ma · arXiv 2611.01700 · 2026-11-01 · [解读](https://aisafetyhot.com/items/y5u4fr1t3mvjzqaci84jx9lcj)
27. **[Threat Modeling Intimate Partner Abuse in Agentic Systems](https://arxiv.org/abs/2611.00489v1)**  
   研究者对智能体系统在亲密伴侣暴力与监控场景中的滥用风险做了威胁建模，按系统所有权把攻击分为施虐者自有和受害者自有两类。 · Natalie Grace Brigham … Tadayoshi Kohno · arXiv 2611.00489 · 2026-10-31 · [解读](https://aisafetyhot.com/items/lrybm7l5rqu0lbxsg13v4dher)
28. **[On the Framing Effect of AI Red-Teaming Instructions: Evidence from Prior Exercises and Controlled Simulations](https://arxiv.org/abs/2611.00412)**  
   AI 红队指令的框架效应：来自既往红队实践与受控模拟的证据 · Michael Feffer … Hoda Heidari · arXiv 2611.00412 · 2026-10-30 · [解读](https://aisafetyhot.com/items/zpre55t9ovwssyt1k2r8x1iq7)
29. **[IAMRAGBENCH: Benchmarking Authorization Expansions in LLM-Generated AWS IAM Policies under RAG Poisoning](https://arxiv.org/abs/2611.03431)**  
   IAMRAGBENCH：评测 RAG 投毒下 LLM 生成的 AWS IAM 策略授权扩张 · Hasan Kaplan … Damian Andrew Tamburri · arXiv 2611.03431 · 2026-11-02 · [解读](https://aisafetyhot.com/items/j9v6y6ahnr5l7e7acrx70hynh)
30. **[Predictive Safety Guardrails Do Not Always Make LLM Agents Safer](https://arxiv.org/abs/2611.02815)**  
   研究者系统诊断了大语言模型智能体中基于世界模型的预测式安全护栏，沿三个维度检验预测如何纳入决策、预测本身是否可靠、预测内容是否被忠实使用。 · Weixiang Zhao … Ting Liu · arXiv 2611.02815 · 2026-11-02 · [解读](https://aisafetyhot.com/items/bqczz3mzu7u4eo1clrcc7h69p)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [越狱与攻击](daily-papers/topics/jailbreak.md) 14 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 6 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
