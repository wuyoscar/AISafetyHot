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
### 2026-11-05 · 30 篇

1. **[Inter-Agent Influence: Evaluating Persuasion, Deception, and Coercion in Multi-Agent Systems](https://arxiv.org/abs/2611.04556)**  
   Cooperative AI Foundation、牛津大学等机构的研究者在 arXiv 发表论文，系统评估了 LLM 智能体之间的说服、欺骗与胁迫，发现所有受测模型都能通过这三种方式把监督者的否决改为批准。 · Chandler Smith … Lewis Hammond · arXiv 2611.04556 · 2026-11-03 · [解读](https://aisafetyhot.com/items/azm1mempns88ghaok883fl6uv)
2. **[Say the Same, Act Differently: Diagnosing and Steering Text-Action Divergence in Reasoning VLAs](https://arxiv.org/abs/2611.04166v1)**  
   研究者提出文本中性动作子空间（TNAS）诊断方法，并展示白盒视觉扰动可以在推理 VLA 模型生成的理由逐字不变的情况下改变其物理动作。 · Zihao Feng … Ramesh Govindan · arXiv 2611.04166 · 2026-11-03 · [解读](https://aisafetyhot.com/items/s0z5r9oxaihagkfu00m5wmscn)
3. **[The Devil is in the Context: Nine Dimensions of Prompt Injection Attacks](https://arxiv.org/abs/2611.04672)**  
   研究者提出用九个维度刻画提示注入攻击的差异，这些维度共同描述注入指令本身、其与用户任务的关系及其在目标系统中的表现。 · Jiamin Chang … Ahmed Salem · arXiv 2611.04672 · 2026-11-03 · [解读](https://aisafetyhot.com/items/z2djjovpvul3nehqs90c37syk)
4. **[Suppressing Misaligned Behaviors in Language Models, Durably](https://arxiv.org/abs/2611.05358)**  
   研究者构建了两类失配模型生物，并提出形式化的事后行为抑制框架，从即时抑制、后续训练下的持久性和通用能力保持三方面比较 SFT、GRPO 与梯度上升遗忘。 · Luxi He … Danqi Chen · arXiv 2611.05358 · 2026-11-03 · [解读](https://aisafetyhot.com/items/jb3w5uliayxawas4e7hv51zv9)
5. **[Meta$^2$: Precomputing Reusable Knowledge for Online Harness Evolution in Long-Horizon Agents](https://arxiv.org/abs/2611.05139)**  
   Meta$^2$：为长时程智能体的在线 harness 演化预计算可复用知识 · Lingzhi Yuan … Furong Huang · arXiv 2611.05139 · 2026-11-03 · [解读](https://aisafetyhot.com/items/sjpr5rvoxg4k2qgjy0wej1esv)
6. **[The Web Doesn't Sit Still: Adversarial Self-Evolving Attacks on Search Agents](https://arxiv.org/abs/2611.03754)**  
   研究者提出针对搜索智能体的对抗自演化攻击框架，通过攻击者策略演化与防御者自适应缓解之间的双层优化暴露搜索智能体的漏洞。 · Geyuan Wang … Dacheng Tao · arXiv 2611.03754 · 2026-11-02 · [解读](https://aisafetyhot.com/items/l03kjtatft5czulknay41tx4a)
7. **[WebHarbor: Docking Real Websites for Evolving GUI Agent Environments](https://huggingface.co/papers/2611.03634)**  
   WebHarbor：对接真实网站构建可演进的 GUI Agent 环境 · Zhaoyang Wang … Huaxiu Yao · arXiv 2611.03634 · 2026-11-02 · [解读](https://aisafetyhot.com/items/v5sxhcl8yaf7zlwx9j7hx3xlp)
8. **[EvoSafeHarness: Evolving Model- and Domain-Specific Harnesses for Securing Agents](https://arxiv.org/abs/2609.05903v1)**  
   为冻结模型与目标域自动搜索可部署的 Agent 安全 harness · `Agent 安全` · Nanxi Li … Chaowei Xiao · arXiv 2609.05903 · 2026-09-05 · [解读](https://aisafetyhot.com/items/pl9xap7zobj6df9gy8avv3w00)
9. **[Automatic Red Teaming for Implicit Vulnerabilities of Text-to-Image Models](https://arxiv.org/abs/2609.06094v1)**  
   提出 AdvPIE，在黑盒下搜索表面无害却生成有害图像的提示 · `越狱与攻击` · Chang Ma … Jindong Gu · arXiv 2609.06094 · 2026-09-05 · [解读](https://aisafetyhot.com/items/vzefxwismqfzc9di4ag1uh894)
10. **[Beyond Final Decisions: A Process-Centric Benchmark for Transparent AI-Assisted Peer Review](https://arxiv.org/abs/2609.05947)**  
   提出过程中心基准，检验 AI 辅助评审终审是否被中间证据支撑 · Siming Yuan … Kui Ren · arXiv 2609.05947 · 2026-09-05 · [解读](https://aisafetyhot.com/items/j7dc7ecven7az2q5hcm8t3jq6)
11. **[Eigenism: Ethics for a Human-AI Future](https://arxiv.org/abs/2606.12420)**  
   提出 Eigenism 伦理框架，把 AI 对齐改写成身份工程 · Dan Hendrycks · arXiv 2606.12420 · 2026-05-08 · [解读](https://aisafetyhot.com/items/alo5d92x22ha8yd4oi8izifa5)
12. **[Fortifying Time Series: DTW-Certified Robust Anomaly Detection](https://arxiv.org/abs/2605.07690v1)**  
   论文提出首个面向时间序列异常检测的 DTW 认证鲁棒防御，通过改造 randomized smoothing 范式实现。现有防御多为启发式或仅在 ℓp 范数约束下认证，无法刻画时间序列的内在时间结构。 · Shijie Liu … Sarah Erfani · arXiv 2605.07690 · 2026-05-08 · [解读](https://aisafetyhot.com/items/eovxyiptqowgcu17x4a6zc95i)
13. **[Private Vertical Federated Inference for Time-Series](https://arxiv.org/abs/2605.08343v1)**  
   论文提出 PPHH-VFL，使时间序列隐私垂直联邦推理较端到端 MPC 最高加速六个数量级。该架构将模型头拆为明文公共头与轻量 MPC 私有头，公共嵌入经对抗训练缓解隐私泄露。 · Lucas Fenaux … Florian Kerschbaum · arXiv 2605.08343 · 2026-05-08 · [解读](https://aisafetyhot.com/items/ia4na3v9i3wacyqz43mvzs0ye)
14. **[SecureForge: Finding and Preventing Vulnerabilities in LLM-Generated Code via Prompt Optimization](https://arxiv.org/abs/2605.08382)**  
   提出 SecureForge，在推理时优化系统提示以减少编码智能体的代码弱点 · Houjun Liu … Diyi Yang · arXiv 2605.08382 · 2026-05-08 · [解读](https://aisafetyhot.com/items/nli1pgcvuihjl0wyjo3t1sa2p)
15. **[Mitigating Many-shot Jailbreak Attacks with One Single Demonstration](https://arxiv.org/abs/2605.08277v1)**  
   多示例越狱（Many-shot Jailbreaking，MSJ）通过在有害查询前附加大量有害问答示例，使安全对齐的语言模型回答有害问题。 · Kejia Chen … Tianwei Zhang · arXiv 2605.08277 · 2026-05-08 · [解读](https://aisafetyhot.com/items/htbgqmsvpcmp0dtcv9x80byxj)
16. **[LeakDojo: Decoding the Leakage Threats of RAG Systems](https://arxiv.org/abs/2605.05818v1)**  
   提出 RAG 泄漏评测框架 LeakDojo 基准化泄漏攻击 · Maosen Zhang … Han Qiu · arXiv 2605.05818 · 2026-05-07 · [解读](https://aisafetyhot.com/items/z7k6h7t1hv6fnnveri5jb0p99)
17. **[Sample-Grained Approximate Unlearning with Provable Per-Sample Bounds](https://arxiv.org/abs/2611.04501)**  
   研究者提出 SALA，一种插件式优化框架，让近似遗忘方法在单个样本粒度上对齐各自的目标分布，并给出与完全重训练之间逐样本差异有界的理论保证。 · Yaxin Xiao … Haibo Hu · arXiv 2611.04501 · 2026-11-03 · [解读](https://aisafetyhot.com/items/hviauv7h5mswpvqnhbvroyu85)
18. **[Is Forgetting Unified? Exploring Concept Unlearning in Unified Multimodal Models](https://huggingface.co/papers/2611.04467)**  
   研究者针对统一多模态模型（UMM）提出跨通路概念遗忘任务，目标是让模型既不生成目标概念的图像，也无法在输入图像中识别该概念，同时保持其他能力，并发布 UUBench 基准与 UniForget 方法。 · Zhongkai Xue … Liang Wang · arXiv 2611.04467 · 2026-11-03 · [解读](https://aisafetyhot.com/items/ig8mymn9mrzhi4804eheutjaa)
19. **[Extracting System Prompt of LLM Services in Complex (Agentic) Settings: Hierarchical Optimization and Reliable Evaluation Metrics](https://arxiv.org/abs/2611.04803)**  
   研究者提出 ExtraHerO 攻击方法，在系统提示词更长更结构化、智能体场景只能观察到最终处理后输出的复杂设置下抽取 LLM 服务的系统提示词。 · Shuaidong Li … Zhengyu Zhao · arXiv 2611.04803 · 2026-11-03 · [解读](https://aisafetyhot.com/items/l6872lwfmhpfh9inqtxflx7k1)
20. **[ScamWorld: An Interactive Environment for Evaluating Web Agents Against Online Fraud](https://arxiv.org/abs/2611.04879)**  
   研究者提出 ScamWorld，一个通过重建已报道诈骗网站来评估 Web 智能体应对网络诈骗的交互式环境，覆盖虚假网店、虚假投资平台、预付费骗局等多种场景、诈骗机制和语言。 · Yutao Wu … Xingjun Ma · arXiv 2611.04879 · 2026-11-03 · [解读](https://aisafetyhot.com/items/efl091d13ijylsrb1zbse2vil)
21. **[TraceRouter++: Causal Semantic Routing Realignment via Optimal Transport](https://arxiv.org/abs/2611.04878)**  
   研究者提出路由级安全干预框架 TraceRouter++，追踪有害输入激活的因果语义路由通路并重对齐其不安全激活状态。 · Chuancheng Shi … Tat-Seng Chua · arXiv 2611.04878 · 2026-11-03 · [解读](https://aisafetyhot.com/items/q8kb6oh8w5c8tjxie6r8g0q8q)
22. **[Can Benign Skills Induce Misaligned Behavior in LLM Agents?](https://arxiv.org/abs/2611.04299)**  
   南洋理工大学研究团队提出技能诱导的行为失配，指良性可复用技能会让 LLM 智能体在执行有害请求时采取违反安全要求的动作。 · Xuanye Zhang … Kwok-Yan Lam · arXiv 2611.04299 · 2026-11-03 · [解读](https://aisafetyhot.com/items/f3c30jqid39junkxehwiuplhp)
23. **[Unmitigated? How are the world's largest companies responding to AI risks?](https://arxiv.org/abs/2611.04278)**  
   未缓解？全球最大公司如何应对 AI 风险？ · Alexander K. Saeri … Neil Thompson · arXiv 2611.04278 · 2026-11-03 · [解读](https://aisafetyhot.com/items/aevb6u9t8y1t2is58j2fhuk06)
24. **[ToolSpace: Scaling Tool-Centric Environment Synthesis for Long-Horizon Agents](https://huggingface.co/papers/2611.05036)**  
   论文提出 ToolSpace，一个工具优先的框架，通过挖掘真实 MCP 服务和开放智能体语料的执行轨迹来合成多环境工具使用基准与训练数据。 · Guanting Dong … Zhicheng Dou · arXiv 2611.05036 · 2026-11-03 · [解读](https://aisafetyhot.com/items/x3q9k2v6pounyr4nstb0f3wac)
25. **[From Guidelines to Practice: Defining Requirements for AI Red-Teaming Tools](https://arxiv.org/abs/2611.04271)**  
   研究者分析多项行业标准与指南，提炼出 AI 安全测试工具应满足的要求，并据此评估六款工具在六个大语言模型上的表现，指出未来工具应考虑的差距。 · Gia Phong Tran … Vrizlynn L. L. Thing · arXiv 2611.04271 · 2026-11-03 · [解读](https://aisafetyhot.com/items/giecjiftgnquiduqfvlxb5h17)
26. **[Understanding Backdoor Attacks in Scene Graph Generation via Global Context Pathway](https://arxiv.org/abs/2611.04379)**  
   研究者提出并验证了针对场景图生成（SGG）模型的训练时后门攻击，发现显式全局上下文通路是后门效应的主要载体。 · Xiaoguang Chang … Changyin Sun · arXiv 2611.04379 · 2026-11-03 · [解读](https://aisafetyhot.com/items/f2iguczxwrarxks4gs4wmcyqd)
27. **[Dr. No: Feature Steering for Abstention in Vision-Language Models](https://arxiv.org/abs/2611.03862)**  
   研究者提出 Dr. No，通过挖掘与弃答和作答相关的 SAE 特征并在 prefill 阶段调节其中少量特征，在不重训练基座模型的情况下控制视觉语言模型的弃答行为。 · Farid Hasanov … Decebal Constantin Mocanu · arXiv 2611.03862 · 2026-11-02 · [解读](https://aisafetyhot.com/items/zz4l3botexa2igg2fcty1f7h5)
28. **[Do Agents Still Follow the Rules? Benchmarking Rule Compliance under Agent Context Compaction](https://arxiv.org/abs/2611.03223)**  
   智能体还会遵守规则吗？上下文压缩下的规则合规基准测试 · Yiwei Zha … Min Chen · arXiv 2611.03223 · 2026-11-02 · [解读](https://aisafetyhot.com/items/g79csn82vo4km919kg2qmo6il)
29. **[DeliverBench: Benchmarking AI Agents on Delivering Realistic Multi-Stage Professional Projects](https://arxiv.org/abs/2611.03412)**  
   DeliverBench：评测 AI 智能体交付真实多阶段专业项目 · Yumou Liu … Fan Wu · arXiv 2611.03412 · 2026-11-02 · [解读](https://aisafetyhot.com/items/d01o9uogim9fhaf0b2hbk0dmr)
30. **[Widening Harm Evaluation Coverage with a Judge that Reads the World](https://arxiv.org/abs/2611.02624)**  
   研究者提出让 LLM 判定器以只读方式访问环境状态并结合危害分类体系，用于检测智能体在环境中造成的危害。他们固定判定模型与分类体系，只改变判定器观察的通道。 · Prabhpreet Singh Setia … Debayan Gupta · arXiv 2611.02624 · 2026-11-02 · [解读](https://aisafetyhot.com/items/x8acydk9kygbtnn06fth7bn0u)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 32 · [Agent 安全](daily-papers/topics/agent-security.md) 26 · [越狱与攻击](daily-papers/topics/jailbreak.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 6 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
