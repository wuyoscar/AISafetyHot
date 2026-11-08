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
### 2026-11-09 · 30 篇

1. **[Editing the Goal: Per-Token SAE Steering and Its Depth Limits in $\pi_{0.5}$](https://arxiv.org/abs/2611.00602)**  
   编辑目标：π0.5 中的逐 token SAE 引导及其深度限制 · Rocio Perales Valdes, Animesh Garg · arXiv 2611.00602 · 2026-10-31 · [解读](https://aisafetyhot.com/items/bfvsi0dhoz1nlq7883bizzr3l)
2. **[Illusion: Safeguarding Topology Confidentiality in LLM Multi-Agent Systems via Behavior-Preserving Obfuscation](https://arxiv.org/abs/2611.00923)**  
   Illusion 是 LLM 多智能体系统的主动拓扑混淆防御：注入假边与假消息向攻击者呈现欺骗性拓扑，并保持输出分布等价与任务精度不降。 · Yiu-Fai Cheung … Hao Wang · arXiv 2611.00923 · 2026-10-31 · [解读](https://aisafetyhot.com/items/zlji8hz7ymfehoqobp1tq1fgl)
3. **[Story Imprinting: AI Assistants Absorb Traits from Human Characters They Resemble](https://arxiv.org/abs/2609.10883v1)**  
   展示人类角色故事微调会使助手吸收相似角色的行为与偏好 · Jorio Cocola … Owain Evans · arXiv 2609.10883 · 2026-09-09 · [解读](https://aisafetyhot.com/items/xatc4dh591s05zhtduhsttrih)
4. **[AI Safety: Not Optional, Not Later](https://arxiv.org/abs/2609.10630)**  
   提出结合 Scientist AI 监督与系统级控制的智能体保障架构 · `Agent 安全` · Qinghua Lu, Yoshua Bengio · arXiv 2609.10630 · 2026-09-09 · [解读](https://aisafetyhot.com/items/vipgdzy1kthne54yhj2vq6zlh)
5. **[Distributed and Private Textual Data Synthesis from Embeddings](https://arxiv.org/abs/2609.10104v2)**  
   论文提出一种无需可信第三方、只需用户轻量参与的分布式差分隐私（DP）文本数据合成方案。 · Ergute Bao … Xiaokui Xiao · arXiv 2609.10104 · 2026-09-09 · [解读](https://aisafetyhot.com/items/u5j0553xgh9nmjswlsd2gl2dl)
6. **[Understanding the Security Boundary of Obfuscation-based On-Device LLM Protection](https://arxiv.org/abs/2609.10117v2)**  
   提出 Collapse，从端侧混淆暴露视图抽取高效用替代模型 · Hanyi Zhou … Zhuotao Liu · arXiv 2609.10117 · 2026-09-09 · [解读](https://aisafetyhot.com/items/vmxmoptucydlswknkdt6sru2j)
7. **[SoK: Privacy Attacks on Machine Learning via Explainable AI](https://arxiv.org/abs/2609.10627v1)**  
   系统比较解释获取路径下的抽取、成员推断与反演 · Abdullah Caglar Oksuz … Erman Ayday · arXiv 2609.10627 · 2026-09-09 · [解读](https://aisafetyhot.com/items/vub6afz5d5njx5jgw328shwg0)
8. **[Privacy-Preserving Split Learning for Federated LLM Fine-Tuning](https://arxiv.org/abs/2609.09794v1)**  
   提出学习式混淆-恢复方案，防止分割联邦微调中激活泄露输入 · Heng Jin … Y. Thomas Hou · arXiv 2609.09794 · 2026-09-09 · [解读](https://aisafetyhot.com/items/o64iq7pzfg8b13qkvi9ffdqxn)
9. **[No-Box Vulnerability Analysis: Description-only Detection of Indirect Prompt Injection Vulnerabilities in MCP Servers](https://arxiv.org/abs/2609.10854v2)**  
   提出 MCPSEC，仅凭工具元数据无盒检测 MCP 间接提示注入漏洞 · Zehua Zhang … Adam Doupé · arXiv 2609.10854 · 2026-09-09 · [解读](https://aisafetyhot.com/items/bxc3gr38nsn04j2ta3a2u630m)
10. **[DuplexJail: Spoken Interruption Attacks on Full-Duplex Speech Models](https://arxiv.org/abs/2609.09420v2)**  
   提出通过语音打断时机实施的全双工语音模型越狱攻击 · Jaechul Roh … Andrea Fanelli · arXiv 2609.09420 · 2026-09-08 · [解读](https://aisafetyhot.com/items/xq7j2qx3bb1vfdgv5lhg797h1)
11. **[Do Androids Dream of Breaking the Game? Systematically Auditing AI Agent Benchmarks with BenchJack](https://arxiv.org/abs/2605.12673)**  
   提出 BENCHJACK，审计 Agent 基准中的奖励作弊缺陷 · `Agent 安全` · Hao Wang … Dawn Song · arXiv 2605.12673 · 2026-05-12 · [解读](https://aisafetyhot.com/items/x9uv4026trhf79ft7lw4j0nx9)
12. **[Attacks and Mitigations for Distributed Governance of Agentic AI under Byzantine Adversaries](https://arxiv.org/abs/2605.12364v1)**  
   研究者针对智能体 AI 治理方案 SAGA 依赖集中式信任点 Provider、易受恶意 Provider 破坏的缺陷，分析并执行了 Provider 失陷后的多种具体攻击，可破坏智能体可归因性、窃取隐私数据并绕过访问控制。 · Matthew D. Laws … Cristina Nita-Rotaru · arXiv 2605.12364 · 2026-05-12 · [解读](https://aisafetyhot.com/items/d41dyig1n29vmtjb6h9poxdqo)
13. **[No More, No Less: Task Alignment in Terminal Agents](https://arxiv.org/abs/2605.12233v1)**  
   不多不少：终端智能体的任务对齐 · Sina Mavali … Lea Schönherr · arXiv 2605.12233 · 2026-05-12 · [解读](https://aisafetyhot.com/items/vlh82j047zao72e2b6v3j8807)
14. **[SkillSafetyBench: Evaluating Agent Safety under Skill-Facing Attack Surfaces](https://arxiv.org/abs/2605.12015v3)**  
   SkillSafetyBench：评估技能攻击面下的 Agent 安全 · Chang Jin … Xingcheng Xu · arXiv 2605.12015 · 2026-05-12 · [解读](https://aisafetyhot.com/items/h1m7hk3hzih0vzwzv5ihloks8)
15. **[CoT-Guard: Small Models for Strong Monitoring](https://arxiv.org/abs/2605.12746v1)**  
   研究者提出 CoT-Guard，一个 4B 参数的小型思维链监控器，用于检测代码生成任务中被注入的隐藏目标。现有 4B 至 8B 小模型即使能读取思维链，也常把隐藏目标误判为用户请求的一部分。 · Nirav Diwan … Gang Wang · arXiv 2605.12746 · 2026-05-12 · [解读](https://aisafetyhot.com/items/jqtka46rigl0xfm738jyzi10t)
16. **[REALISTA: Realistic Latent Adversarial Attacks that Elicit LLM Hallucinations](https://arxiv.org/abs/2605.12813v2)**  
   研究者提出 REALISTA，一种通过语义等价改写诱导大语言模型幻觉的潜空间对抗攻击框架，并在先前现实类攻击失效的自由回复设置下成功攻击大型推理模型。 · Buyun Liang … René Vidal · arXiv 2605.12813 · 2026-05-12 · [解读](https://aisafetyhot.com/items/fm38fbmdde7vz5s25ngft2ecv)
17. **[Reconstruction of Personally Identifiable Information from Proprietary Data in Supervised Fine-Tuned Models](https://arxiv.org/abs/2605.12264v2)**  
   研究者提出覆盖感知解码算法 COVA，在基于前缀的攻击下从经专有数据监督微调的大语言模型中定向重建特定用户的个人身份信息（PII），在多个数据集上的重建效果均优于基线解码方法。 · Sae Furukawa, Alina Oprea · arXiv 2605.12264 · 2026-05-12 · [解读](https://aisafetyhot.com/items/a104mpgvedeocmvqk8d14lay4)
18. **[MATRA: Modeling the Attack Surface of Agentic AI Systems -- OpenClaw Case Study](https://arxiv.org/abs/2605.10763v1)**  
   研究者提出 MATRA，一个面向智能体 AI 系统的威胁建模框架，用于系统评估已知 LLM 威胁在具体部署中会转化为哪些实际风险。 · Tim Van hamme … Dinil Mon Divakaran · arXiv 2605.10763 · 2026-05-11 · [解读](https://aisafetyhot.com/items/j2zyyyt3pyhn4bxzh3dj9za92)
19. **[Comment and Control: Hijacking Agentic Workflows via Context-Grounded Evolution](https://arxiv.org/abs/2605.11229v1)**  
   约翰斯·霍普金斯大学等机构的研究者提出 JAW 框架，用于检测并利用 GitHub Actions 和 n8n 上的智能体工作流劫持漏洞。 · Neil Fendley … Yinzhi Cao · arXiv 2605.11229 · 2026-05-11 · [解读](https://aisafetyhot.com/items/qmzoukuvjz65g1za4jt4dmkvj)
20. **[LoRA-Patch: Defending Against Backdoored LoRA Adapters via Directional Steering](https://arxiv.org/abs/2611.03752v1)**  
   研究者提出针对 LoRA 适配器的轻量级后门防御方法 LoRA-Patch，通过逐层导向重新对齐适配器方向来抑制触发器激活的后门行为，无需修改基座模型权重。 · Shengyan Huo … Yige Li · arXiv 2611.03752 · 2026-11-02 · [解读](https://aisafetyhot.com/items/y67uwogpycv0zwdnw16iifi39)
21. **[Switch-SWE: Do Coding Agents Hold Focus When Switching Between Unfinished Tasks?](https://huggingface.co/papers/2611.02017)**  
   研究者提出 Switch-SWE 基准，用于测量编码智能体在交替推进同一代码仓库里多个未完成任务后，能否恢复此前任务的要求与部分进展。 · Shuochen Chang … Jiangtong Li · arXiv 2611.02017 · 2026-11-01 · [解读](https://aisafetyhot.com/items/rjo6od4tk9l2ayhe0dm7oo13l)
22. **[Is Your Long-Horizon Benchmark Really Deep? Measuring and Synthesizing Depth in Terminal Tasks](https://huggingface.co/papers/2611.01927)**  
   论文提出用顺序依赖深度而非轮数来衡量终端任务难度，并据此生成更难的任务集。 · Yu Jiang … Xiangliang Zhang · arXiv 2611.01927 · 2026-11-01 · [解读](https://aisafetyhot.com/items/dwniitw6tcck40twfy1jkkvmf)
23. **[CrossSWE: Benchmarking Cross-Repository Joint Development for Coding Agents](https://huggingface.co/papers/2611.01484)**  
   CrossSWE 是一个测试编码 Agent 跨仓库联合开发能力的基准，论文的评测显示当前模型难以维持跨仓库一致性。 · Silin Chen … Zhensu Sun · arXiv 2611.01484 · 2026-11-01 · [解读](https://aisafetyhot.com/items/vvrjoizv70tgkeur9cgnc9wlz)
24. **[Step-Zero Attack: Agent Safety Before Observability](https://arxiv.org/abs/2611.01953)**  
   提出 Step-Zero 攻击，绕过 Agent 对不透明载体的安全检查 · Tian Qin … Lijie Wen · arXiv 2611.01953 · 2026-11-01 · [解读](https://aisafetyhot.com/items/qg7ia7we2ixezbw69n6y16r7u)
25. **[TopoSteer: Topological Layer Selection for Activation Steering in LLMs](https://arxiv.org/abs/2611.01493)**  
   TopoSteer 提出一种基于拓扑的层选择方法，用于 LLM 激活引导，并在多个语言模型和引导任务上实现更有效的引导且无需留出验证。 · Tuc Nguyen … Thai Le · arXiv 2611.01493 · 2026-11-01 · [解读](https://aisafetyhot.com/items/zdwtd9bb91nxe2mabdodj550a)
26. **[J-Anchor: Defending Against Prefill Attacks via J-Space Selective Refusal Restoration](https://arxiv.org/abs/2611.01342)**  
   研究者提出无需训练的推理时防御方法 J-Anchor，用于对抗预填充越狱。预填充越狱会让安全对齐模型接续攻击者构造的不安全助手前缀，即使同一请求在正常解码下会被拒答。 · Running Yang … Xiaoxiao Li · arXiv 2611.01342 · 2026-10-31 · [解读](https://aisafetyhot.com/items/kbd3xtbulvbw7g6uekxp1zrj6)
27. **[AgentCap: Capability-Based Runtime Authorization for Secure LLM Agent Execution](https://arxiv.org/abs/2611.00729)**  
   研究者提出 AgentCap，一种把授权决策从模型推理中剥离的 LLM 智能体运行时授权层，通过 MCP 包装器中介每一次工具调用。 · Aravinda Kashyap Kabbinamakki Suresh, Peng Gao · arXiv 2611.00729 · 2026-10-31 · [解读](https://aisafetyhot.com/items/ul5qzfgq3jutllth3xtqrc4se)
28. **[Context-Shielded Backdoor Attack against Large Vision-Language Models](https://arxiv.org/abs/2611.01252)**  
   针对大型视觉语言模型的上下文屏蔽后门攻击 · Zhifang Zhang … Miao Xu · arXiv 2611.01252 · 2026-10-31 · [解读](https://aisafetyhot.com/items/m63gmx8tyjxlmbwj4svxiycar)
29. **[Near-Zero Token Embeddings Silently Stall Training in Gated Sequence Models](https://huggingface.co/papers/2611.04449)**  
   诊断近零嵌入行在门控模型训练中静默清零梯度的机制并提出修复 · Xin Liu … Mengyu Liu · arXiv 2611.04449 · 2026-11-03 · [解读](https://aisafetyhot.com/items/hbk50z6ija616fq0cvxd2t2c6)
30. **[Trusting Imagined Futures: Auditing Imagined Rewards for VLA Post-Training](https://arxiv.org/abs/2611.04873)**  
   TIF 用执行反馈审计视频世界模型预测的奖励，为 VLA 后训练筛选监督轨迹。 · Zicheng Kong … Zhaofeng He · arXiv 2611.04873 · 2026-11-03 · [解读](https://aisafetyhot.com/items/rc8jwzlcyzt4k3jhqvxo4s05r)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 30 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 7 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
