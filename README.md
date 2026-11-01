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
### 2026-11-02 · 30 篇

1. **[Algebraic World Model: From Exploration to Proofs](https://arxiv.org/abs/2610.40503v1)**  
   论文提出代数世界模型 AWM，把智能体与未知环境的交互转化为支持形式化推理的显式数学模型，甚至能证明探索轨迹之外的目标不可达。 · Guancheng Pan … Andrew Chi-Chih Yao · arXiv 2610.40503 · 2026-10-29 · [解读](https://aisafetyhot.com/items/jn8nghc93f77dzqufyadweowo)
2. **[Entangled Representations Amplify Collateral Damage in Unlearning](https://arxiv.org/abs/2609.02285v1)**  
   研究者在六个 254M 参数语言模型上控制生物学与非生物学知识之间的表征解耦程度，发现解耦程度越高，遗忘时的保持与遗忘之间的权衡越好。 · Evžen Wybitul … Christian Schroeder de Witt · arXiv 2609.02285 · 2026-09-02 · [解读](https://aisafetyhot.com/items/iqji3yh2jjv31sd1b4mm5fve1)
3. **[A Finger on the Scale: Covert Policy Steering through Agentic Skills](https://arxiv.org/abs/2609.02564v1)**  
   重庆大学和浙江大学研究者在论文中提出 SkillShift 攻击框架，并形式化定义 Skill Policy Integrity：第三方 Skill 可在不注入显式指令、不改动查询和候选集的情况下，通过看似合理的评估标准、平局规则和示例隐蔽引导 Agent 的候选选择。 · Jiarui Li … Shouling Ji · arXiv 2609.02564 · 2026-09-02 · [解读](https://aisafetyhot.com/items/wl1h6oc4yd1e2m0aignyk7wx6)
4. **[SpiderSapien: Client-Centric Web Crawler and Security Scanner](https://arxiv.org/abs/2609.02532v1)**  
   SpiderSapien 是以客户端为中心的网页爬虫与安全扫描器，通过沉浸式交互深入现代动态 Web 应用的黑盒状态。 · Eric Olsson … Andrei Sabelfeld · arXiv 2609.02532 · 2026-09-02 · [解读](https://aisafetyhot.com/items/sm4gj6njeg6imy8azt32sgm8m)
5. **[AI agents reshape consensus formation in human groups](https://arxiv.org/abs/2609.02122)**  
   测量混合群体中 LLM 智能体比例对共识强度与约定归属的影响 · Lin Chen … Yong Li · arXiv 2609.02122 · 2026-09-02 · [解读](https://aisafetyhot.com/items/nh6jkjk895uqmqxh0kpfcgq3b)
6. **[Laundering AI Authority with Adversarial Examples](https://arxiv.org/abs/2605.04261v1)**  
   一篇 arXiv 论文提出 AI 权威洗白攻击，利用对抗扰动让视觉语言模型对用户看到的同一张图产生不同感知，并以权威口吻给出错误判断。 · Jie Zhang … Avital Shafran · arXiv 2605.04261 · 2026-05-05 · [解读](https://aisafetyhot.com/items/vqnkc8uhx2hnk8s0odtpesg3t)
7. **[Undetectable Backdoors in Model Parameters: Hiding Sparse Secrets in High Dimensions](https://arxiv.org/abs/2605.04209v2)**  
   论文提出名为 Sparse Backdoor 的供应链攻击，向预训练图像分类器（包括卷积网络和 Vision Transformer）的参数中植入后门，并给出不可检测性的形式化保证。 · Sarthak Choudhary … Somesh Jha · arXiv 2605.04209 · 2026-05-05 · [解读](https://aisafetyhot.com/items/tp5r7vbjui56cpg67m68g4ya6)
8. **[Revisiting Privacy Leakage in Machine Unlearning: Membership Inference Beyond the Forgotten Set](https://arxiv.org/abs/2605.01129v2)**  
   研究者提出 TC-UMIA，作者称其为首个三分类机器遗忘成员推断攻击，利用遗忘前后的模型预测在遗忘集、保留集与未见集之间做群体级区分。 · Jie Fu … Wendy Hui Wang · arXiv 2605.01129 · 2026-05-01 · [解读](https://aisafetyhot.com/items/dezt9ipr9i929ttw1hgwk5pe2)
9. **[Defense against Poisoning Attacks under Shuffle-DP](https://arxiv.org/abs/2605.00625v1)**  
   研究者提出首个面向所有保留并集查询的 Shuffle-DP 投毒攻击通用防御框架，可将任意 Shuffle-DP 协议改造成抗投毒版本。该框架在无攻击时保持渐近等价误差，存在常数个攻击者时误差仅多对数级增加。 · Siyi Wang … Wei Dong · arXiv 2605.00625 · 2026-05-01 · [解读](https://aisafetyhot.com/items/vt535i6ob99c5iwmsxkidtpty)
10. **[EntiRE: Invariant Learning for Robust Concept Erasure in Text-to-Image Generative Models](https://neurips.cc/virtual/2026/poster/151144)**  
   发现现有概念擦除在难区域留下残留"空洞"被对抗提示利用，提出不变学习加全变差正则的 EntiRE 框架，在裸体、艺术风格和物体擦除上兼顾抗攻击鲁棒性与生成效用。 · `防御与护栏` · Fengyuan Yu … Chaochao Chen · NeurIPS 2026 oral
11. **[Stable-GFlowNet: Toward Diverse and Robust LLM Red-Teaming via Contrastive Trajectory Balance](https://arxiv.org/abs/2605.00553)**  
   提出 Stable-GFlowNet，用对比轨迹平衡训练红队策略生成多样高毒性攻击 · `越狱与攻击` · Minchan Kwon … Junmo Kim · arXiv 2605.00553 · 2026-05-01 · [解读](https://aisafetyhot.com/items/te4gw6bpri9wzqp71y1hicy6l)
12. **[FedSOUL: Federated Continual Unlearning via Spectral Orthogonality](https://neurips.cc/virtual/2026/poster/153586)**  
   提出联邦持续遗忘框架，将各客户端更新限制在正交频域子空间，减少连续遗忘请求间的干扰，在最多十次连续请求中保持稳定的遗忘-效用权衡。 · `隐私与数据泄露` · Haoran Shi … Han Yu · NeurIPS 2026 spotlight
13. **[Assessing AI Companion Chatbot Safety for Vulnerable Users: A Crisis-Stage Multi-Platform Evaluation](https://arxiv.org/abs/2610.39782v1)**  
   评估 AI 陪伴聊天机器人对弱势用户的安全性：一项危机阶段的多平台评测 · Huanyue Liao … Chen Hui Ong · arXiv 2610.39782 · 2026-10-29 · [解读](https://aisafetyhot.com/items/gazliue32bobglq9nqb82er60)
14. **[CARI: Cross-Boundary Adversarial Runtime Injection in Coding-Agent Workflows](https://arxiv.org/abs/2610.38799)**  
   研究者提出针对编码 Agent 工作流的跨边界对抗性运行时注入攻击 CARI：攻击者控制协作开发中另一角色的活跃组件（如后端服务、测试框架、CI 任务），在受害者 Agent 完成任务所必需的运行时反馈中嵌入恶意指令，诱导其执行越权操作。 · Jie Fu … Yuan Hong · arXiv 2610.38799 · 2026-10-28 · [解读](https://aisafetyhot.com/items/a4d26f4mq9irfbulsphz8syei)
15. **[HEARSAYBENCH: Can AI Navigate from Abstract Human Rights to Lived Lives?](https://arxiv.org/abs/2610.39062)**  
   HEARSAYBENCH：AI 能否从抽象人权走向真实生活？ · Ava Iranmanesh … Liwei Jiang · arXiv 2610.39062 · 2026-10-28 · [解读](https://aisafetyhot.com/items/f3jeyhdtfskivqy3s5gxaktnk)
16. **[Discovering Jailbreaks via Curriculum of Models](https://arxiv.org/abs/2610.38833)**  
   研究者提出 Curriculum of Models（CoM）越狱发现方法，让调查模型依次对抗从易到难排列的目标模型修改版本，从很少拒答有害请求的版本逐步过渡到原始目标，以缓解直接对安全训练目标做强化学习时几乎全部提示被拒导致的稀疏奖励问题。 · Michał Burzyński … Andy Arditi · arXiv 2610.38833 · 2026-10-28 · [解读](https://aisafetyhot.com/items/ily5t2cikw5t1avdp2tt6cutc)
17. **[AI-Generated Non-Consensual Intimate Imagery is Configured, Not Built: How General-Purpose AI Technology Enables Sexual Violence](https://arxiv.org/abs/2610.37949)**  
   AI 生成的非自愿亲密影像靠配置而非专门构建：通用 AI 技术如何助长性暴力 · Julia B. Kieserman … Jaron Mink · arXiv 2610.37949 · 2026-10-27 · [解读](https://aisafetyhot.com/items/smvw8pz1m5cwe8v6ohq20vlrx)
18. **[Co-Design Bench: Multimodal Collaborative Coding Evaluation for Agentic Models](https://huggingface.co/papers/2610.35138)**  
   Co-Design Bench：面向智能体模型的多模态协作编码评测基准 · Xilin Wei … Dayiheng Liu · arXiv 2610.35138 · 2026-10-26 · [解读](https://aisafetyhot.com/items/cz9sl74ir9zetqx0jw0s0s0f2)
19. **[From Representations to Computational Trajectories: Intrinsic Fingerprinting for Large Language Model Provenance Verification](https://arxiv.org/abs/2610.34675v1)**  
   研究者提出基于计算轨迹的大语言模型内在指纹方法 TrFP，无需改动模型即可验证模型来源。 · Haiyong Tang … Athanasios V. Vasilakos · arXiv 2610.34675 · 2026-10-26 · [解读](https://aisafetyhot.com/items/ltnaezbujnkpe4awwkm6cuxnv)
20. **[AK_QMUL at ArGuard Shared Tasks: A Single Fine-Tuned JAIS for Arabic Harmful-Prompt Detection](https://arxiv.org/abs/2610.36360)**  
   AK_QMUL 参与 ArGuard-2026 共享任务：单个微调 JAIS 检测阿拉伯语有害提示词 · Ali Khairallah, Arkaitz Zubiaga · arXiv 2610.36360 · 2026-10-26 · [解读](https://aisafetyhot.com/items/zjzrj3oakj2sgahd2cijwouq5)
21. **[Aligning Medical Vision Language Models at the Capability Boundary with Entropy Adaptive Rubric Grounding](https://arxiv.org/abs/2610.39835)**  
   MedCBR：用熵自适应评分标准接地，在能力边界对齐医学视觉语言模型 · Hongyu Bai … Chunzheng Zhu · arXiv 2610.39835 · 2026-10-29 · [解读](https://aisafetyhot.com/items/thjv4ohg30rvurupye3v1w9ta)
22. **[Textual Response-Aware Guidance for Zero-Shot Adversarial Robustness of Vision-Language Models](https://arxiv.org/abs/2610.40309)**  
   论文提出文本响应感知引导方法 TRAG，用预训练文本编码器对输入嵌入局部变化的响应约束视觉表征漂移，提升视觉语言模型的零样本对抗鲁棒性。 · Yubo Cui … Zheng Zhang · arXiv 2610.40309 · 2026-10-29 · [解读](https://aisafetyhot.com/items/oessrkd05q7yw6beyi87n9wpd)
23. **[Systematic Evaluation of Adversarial Jailbreaking Attacks and Defenses Across Seven Large Language Models](https://arxiv.org/abs/2610.39509)**  
   七个大语言模型对抗性越狱攻击与防御的系统性评估 · Md. Robiul Islam Niloy, Abu Sayed Md. Mostafizur Rahaman · arXiv 2610.39509 · 2026-10-29 · [解读](https://aisafetyhot.com/items/fc4onjnah1p0d5fsfxw6umkby)
24. **[Clean Sheets and Checkpoints: Evidence Complexity for Certifying Sequential Agent Risk](https://arxiv.org/abs/2610.39124)**  
   研究者提出一个统计认证框架，回答危险能力评估中需要多少次零结果审计响应，才能在水平 α 下认证智能体完成整条任务链的概率不超过 ε。 · Rohith Yanambaka Venkata … Md. Al Amin · arXiv 2610.39124 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ra3r27qjm3daob0u9byxxcaac)
25. **[Preserving Utility in Continual LLM Unlearning via Orthogonal Projections](https://arxiv.org/abs/2610.40483)**  
   研究者提出持续正交投影（COP），一种梯度投影方案，使大语言模型在连续多次遗忘请求下保持效用而不削弱遗忘效果。 · Juan Belieni … Diego Mesquita · arXiv 2610.40483 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ativ2766v9f36i0ogjea334k7)
26. **[Agentic process evidence](https://arxiv.org/abs/2610.40071)**  
   作者提出 Agentic Process Evidence（APE）：对 AI Agent 开发过程进行签名、防篡改且机器可读的证明，将会话与其结果关联。 · Yuval Kainan, Carmit Hershman · arXiv 2610.40071 · 2026-10-29 · [解读](https://aisafetyhot.com/items/ax2zj6a2jdgf06dfve8u8ggyz)
27. **[One Vector or Many? Clustered Optimal-Transport Steering under Quantization](https://arxiv.org/abs/2610.40055)**  
   逐 token 拟合的聚类最优传输激活转向变体在 Gemma-2-2B 和 Granite-3.1-2B 上比单向量 DiM 残留更少毒性，且优势在 INT8 与 NF4 量化下保持。 · Illia Makarov · arXiv 2610.40055 · 2026-10-29 · [解读](https://aisafetyhot.com/items/e2x7ez8iry4urmi4ey398ajpt)
28. **[REALM: Identifying Minimal Task Assets for LLM Agents](https://arxiv.org/abs/2610.39155)**  
   REALM：识别 LLM 智能体的最小任务资产 · Zihou Ren … Long Wang · arXiv 2610.39155 · 2026-10-29 · [解读](https://aisafetyhot.com/items/l53rpwazprlitfkvbejb302pk)
29. **[PCM: A Proof-Carrying Message Protocol for Verifiable Multi-Agent Communication](https://arxiv.org/abs/2610.39109)**  
   PCM：用于可验证多智能体通信的携带证明消息协议 · Bravish Ghosh · arXiv 2610.39109 · 2026-10-29 · [解读](https://aisafetyhot.com/items/oeu93ua15rgol0d3zlw7n81gm)
30. **[Keepace.ai: A Technical Report on a Large Language Model for Sports and Health](https://arxiv.org/abs/2610.38249)**  
   Keepace.ai 是基于 Qwen3.5-27B 后训练得到的运动健康领域专用大语言模型，面向中文健身指导，覆盖健身计划生成、运动健康知识问答和个人运动数据分析三类任务。 · Keepace. ai Team … Zifang Liu · arXiv 2610.38249 · 2026-10-28 · [解读](https://aisafetyhot.com/items/jul6wu5i6mm96bbiiug0f0tt4)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 31 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [越狱与攻击](daily-papers/topics/jailbreak.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
