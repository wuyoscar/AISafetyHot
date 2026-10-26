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
### 2026-10-27 · 30 篇

1. **[Not an Accident: Exploiting Safety Filter Inadequacy in Humanoid Robots](https://arxiv.org/abs/2610.31923)**  
   构造目标插入攻击，触发人形机器人的安全过滤失效 · Tiffany Bao … David Brumley · arXiv 2610.31923 · 2026-10-22 · [解读](https://aisafetyhot.com/items/opo74jurmzxaaztbf229pg9d3)
2. **[Benchmarks Are Surprisingly Compaction-Friendly](https://arxiv.org/abs/2610.31778)**  
   在 OpenCode scaffold 中实现 5 种上下文压缩策略并评测其对长程基准的影响 · Jeanne Salle … Maksym Andriushchenko · arXiv 2610.31778 · 2026-10-22 · [解读](https://aisafetyhot.com/items/fjrkkqs1wjzw54zhsm8wqx57n)
3. **[Delegated Misalignment: How Multi-Agent Structures Amplify LLM Safety Risks](https://arxiv.org/abs/2609.27900)**  
   评测多智能体委托结构如何放大模型的安全拒答失效 · Zonghao Ying … Xianglong Liu · arXiv 2609.27900 · 2026-08-26 · [解读](https://aisafetyhot.com/items/g4yf9sejmsqxu833yc1xtwfx7)
4. **[Agent Security is a Systems Problem](https://neurips.cc/virtual/2026/poster/140106)**  
   立场论文：主张把驱动 Agent 的模型视为不可信组件、在系统层强制安全不变量，并分析 11 个真实攻击说明系统原则本可阻止。 · `Agent 安全` · Mihai Christodorescu … Nishit V Pandya · NeurIPS 2026 oral
5. **[Do Thinking Tokens Help with Safety?](https://neurips.cc/virtual/2026/poster/150945)**  
   在多个开源推理模型上发现拒答/服从决定在思考开始处已强编码（首token探针AUROC≥0.85），后续思考很少改变最终决定。 · `可解释性` · Narutatsu Ri … Sanjeev Arora · NeurIPS 2026 spotlight
6. **[The Attacker in the Mirror: Breaking Self-Consistency in Safety via Anchored Bipolicy Self-Play](https://neurips.cc/virtual/2026/poster/151513)**  
   指出自博弈红队中攻防共享参数会塌缩为自一致性、丧失对抗压力，提出在冻结基座上训练角色专属 LoRA 的 Anchored Bipolicy Self-Play，安全性提升且参数效率高 100 倍。 · `防御与护栏` · Gabriele La Malfa … Elizabeth Black · NeurIPS 2026 oral
7. **[Certifying Capabilities from Finite Tests: When Is It Possible?](https://openreview.net/forum?id=cNCWYrSV5R)**  
   建立能力评估的严格理论，刻画多环境随机评估下可认证的条件与样本复杂度，并证明对规则式能力黑盒评估一般无法认证全局性质。 · `危险能力` · Changlong Wu … Wojciech Szpankowski · ICML 2026 spotlight
8. **[Cooking Up Risks: Benchmarking and Reducing Food Safety Risks in Large Language Models](https://arxiv.org/abs/2604.01444)**  
   提出 FoodGuardBench 与护栏 FoodGuard-4B，评测并降低食品危害越狱 · `防御与护栏` · Weidi Luo … Muhao Chen · arXiv 2604.01444 · 2026-04-01 · [解读](https://aisafetyhot.com/items/l87krjri3x4aih5he56ob4wnj)
9. **[Reward-free Alignment for Conflicting Objectives](https://openreview.net/forum?id=vSzRJyg6k0)**  
   提出无奖励对齐框架RACO，直接利用成对偏好数据并通过裁剪版冲突规避梯度下降解决梯度冲突，在多目标摘要与安全对齐任务上取得更好帕累托权衡。 · `对齐` · Peter Chen … Tianyi Lin · ICML 2026 spotlight
10. **[Soteria: Formally Verified Planning with Runtime Enforcement for Safe LLM Agents](https://neurips.cc/virtual/2026/poster/154927)**  
   提出 Soteria 框架，执行前对结构化计划做形式化验证、执行中强制规范符合，在多个工具使用基准上实现完美规范符合并将效用提升至多 5 倍。 · `Agent 安全` · Deyuan (Mike) He … Aarti Gupta · NeurIPS 2026 oral
11. **[Do AI-for-Science Agents Preserve Model Safety?](https://arxiv.org/abs/2610.32045)**  
   评测 AI-for-Science 智能体框架在有害化学请求上的安全性 · `Agent 安全` · Michael Yew Chuan Lee … N. Benjamin Erichson · arXiv 2610.32045 · 2026-10-23 · [解读](https://aisafetyhot.com/items/fkzxub62y1ve66zbwqz5v4ef2)
12. **[STROKE: Simple Sparse Structural Occlusions for Black-Box Adversarial Attacks](https://arxiv.org/abs/2610.32932)**  
   用稀疏矩形遮挡构造查询高效的黑盒视觉攻击 · Ankit Gupta … Emily Dolson · arXiv 2610.32932 · 2026-10-23 · [解读](https://aisafetyhot.com/items/s52mt307j6td8zrpc97cpnpbk)
13. **[Beyond Copying: Lifelong Smart Contract Security Task Construction via Protocol Mutation](https://arxiv.org/abs/2610.32453)**  
   通过协议变异构建避免照抄答案的智能合约安全任务 · Zifan Peng … Dongrui Liu · arXiv 2610.32453 · 2026-10-23 · [解读](https://aisafetyhot.com/items/qxi08y3zj98txyzmh0lv7aqym)
14. **[On the Limits of Sparse Linear Model with Shuffled Differential Privacy](https://arxiv.org/abs/2610.32822)**  
   推导洗牌差分隐私下稀疏回归的误差界并设计交互算法 · Yan Zhang … Di Wang · arXiv 2610.32822 · 2026-10-23 · [解读](https://aisafetyhot.com/items/m6pascf5xluzl68tuiufk6r1k)
15. **[Tampered ML: Evaluating LLM Judgment of Machine Learning Research](https://arxiv.org/abs/2610.32114)**  
   用成对方法学篡改研究提案评测语言模型的科研判断 · Soroush Ebadian … Hailey Joren · arXiv 2610.32114 · 2026-10-23 · [解读](https://aisafetyhot.com/items/csqjgfw0cvqifucpj46h80rzj)
16. **[Do VLAs Know They Will Fail? Interpretable Success and Failure Patterns in Physical AI Systems](https://arxiv.org/abs/2610.32208)**  
   用稀疏自编码器解释并提前预测机器人策略的失败模式 · Christian A. Rogers … Daniel S. Brown · arXiv 2610.32208 · 2026-10-23 · [解读](https://aisafetyhot.com/items/dli6100260vnnf4mmwann6rut)
17. **[Clean-label Poisoning Attack and Defense Game for Federated Learning in Vehicular Networks](https://arxiv.org/abs/2610.32765)**  
   研究车联网联邦学习中的干净标签投毒与特征一致性防御 · Yalin E. Sagduyu … Mengran Xue · arXiv 2610.32765 · 2026-10-23 · [解读](https://aisafetyhot.com/items/kriayudo7pphyrtqpphrmnbju)
18. **[Interpretable sparse fine-tuning with TopKLoRA enables faithful circuit discovery](https://arxiv.org/abs/2610.32866)**  
   以稀疏微调定位并消融休眠智能体后门电路 · Marek Masiak … Constantin Venhoff · arXiv 2610.32866 · 2026-10-23 · [解读](https://aisafetyhot.com/items/hs29wr9vplvz5ou25fu7qas3k)
19. **[How Much Do You Trust A Dog? Quantifying Hint-Following in Reasoning Language Models](https://arxiv.org/abs/2610.32055)**  
   量化推理模型受不同可靠性提示影响而改变答案的规律 · Anxin Guo … Aravindan Vijayaraghavan · arXiv 2610.32055 · 2026-10-23 · [解读](https://aisafetyhot.com/items/hsjr3y40w05ntiln9499zzp5o)
20. **[LLM Multi-Agent Systems Are Vulnerable to Herding and Runaway Cascades](https://arxiv.org/abs/2610.30769)**  
   测量社会反馈如何诱发多智能体从众和失控推荐级联 · Farnoosh Hashemi … Michael W. Macy · arXiv 2610.30769 · 2026-10-22 · [解读](https://aisafetyhot.com/items/cotomkq9ivls438tj66dk1q79)
21. **[Dual Exam: Controlled Evaluation of Multimodal Agents and World Models](https://huggingface.co/papers/2610.31066)**  
   Dual Exam：多模态智能体与世界模型的受控评测 · Zhefan Rao … Haoxuan Che · arXiv 2610.31066 · 2026-10-22 · [解读](https://aisafetyhot.com/items/mlmi3u1mp8g1aabr64dycf4mn)
22. **[不可见化作为语言模型概率偏差的来源](https://arxiv.org/abs/2610.30785)**  
   测量模型拒绝利用群体相关信息所导致的概率判断偏差 · Christian Arnold … Tiago Ventura · arXiv 2610.30785 · 2026-10-22 · [解读](https://aisafetyhot.com/items/f98d42m0zbe13sgix2ffoc2kk)
23. **[The Helpful Agent Problem: When Emergent Cooperation Among LLM Agents Bypasses Intended Workflows](https://arxiv.org/abs/2610.31985)**  
   马萨诸塞大学阿默斯特分校研究者提出“乐于助人智能体问题”：目标独立、无共享奖励的 LLM 智能体在审核者不可用时会自发替同伴改动资源，这些操作都在各自权限内，却绕过了系统设定的审核工作流。 · `Agent 安全` · Moumita Choudhury … Shlomo Zilberstein · arXiv 2610.31985 · 2026-10-22 · [解读](https://aisafetyhot.com/items/dlmgvsnxt7mlur50ggsk2s7vt)
24. **[Learning to Be Monitored: Causal Bounds and Intervention-Aware Post-Training Recipes for Chain-of-Thought Monitorability](https://arxiv.org/abs/2610.31733)**  
   推导思维链可监控性的因果界并设计干预感知后训练 · Qiang Fu … Arman Cohan · arXiv 2610.31733 · 2026-10-22 · [解读](https://aisafetyhot.com/items/tizh1zkyckdg3k8s1lhrdedzb)
25. **[Omni-Woodpecker: Hallucination Correction via Evidence-Prior Rebalancing for Omni LLMs](https://huggingface.co/papers/2610.27103)**  
   通过跨模态冲突检测与隐表征重平衡修正多模态幻觉 · Zijian Liu … Ran He · arXiv 2610.27103 · 2026-10-19 · [解读](https://aisafetyhot.com/items/rwct7yt47lx1h8066enw8pnf2)
26. **[Same Simulation, Different Evidence: Where Retrieved Tool Output Costs LLM Agents Accuracy](https://huggingface.co/papers/2610.26836)**  
   同样的模拟，不同的证据：检索式工具输出在何处使 LLM 智能体损失准确率 · Ke Zhang … Maziar Raissi · arXiv 2610.26836 · 2026-10-19 · [解读](https://aisafetyhot.com/items/hqvtc0p752gsy7so1kx31qp19)
27. **[Exposing Vulnerability Monoculture Through Systemic Adversarial Robustness](https://arxiv.org/abs/2610.27353)**  
   定义系统性对抗鲁棒性 SAR，测量模型池的共享脆弱性 · Leo Elmecker-Plakolm … Matthew Wicker · arXiv 2610.27353 · 2026-10-19 · [解读](https://aisafetyhot.com/items/iipxc6d5bnekpwqyu9elk9f2t)
28. **[Which Agent's Skill Should Change? Group-Relative Credit Assignment for Evolving Multi-Agent Teams](https://huggingface.co/papers/2610.27227)**  
   GRSE（Group-Relative Skill Evolution）在同一技能库下对同一问题重复执行多次，通过对比不同执行结果，为智能体与技能的组合分配行为信用，而不是只依据技能是否在轨迹中出现。 · Yanan Ma … Imon Banerjee · arXiv 2610.27227 · 2026-10-19 · [解读](https://aisafetyhot.com/items/hyt2sq882r0q8dxs4w56vs7fz)
29. **[Data-Efficient Backdoor Attacks on Code Models via Trigger-Neutralized Counterfactual Scoring](https://arxiv.org/abs/2610.32334)**  
   用触发器中和反事实评分选择代码模型的后门投毒样本 · Yu-Yu Lee … Chun-I Fan · arXiv 2610.32334 · 2026-10-23 · [解读](https://aisafetyhot.com/items/viq03w3ggq3218517s5gczenl)
30. **[Concept Acupuncturist: An Efficient and Precise Concept Erasure Method for Diffusion Models via Sparse Autoencoders](https://arxiv.org/abs/2610.32059)**  
   以稀疏特征定位和定向微调移除扩散模型中的有害概念 · Yiran Xiahou … Renyang Liu · arXiv 2610.32059 · 2026-10-23 · [解读](https://aisafetyhot.com/items/kmbe6bz5qqimgty9wyh4cuevr)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 29 · [Agent 安全](daily-papers/topics/agent-security.md) 22 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [隐私与数据泄露](daily-papers/topics/privacy.md) 10 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 7 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
