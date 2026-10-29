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
### 2026-10-30 · 30 篇

1. **[Interpretable Meta-Policies for Neural Decision Making](https://arxiv.org/abs/2610.37451)**  
   研究者提出 NEXUS，一个将神经技能与符号元策略结合的分层强化学习框架，以缓解深度强化学习因神经网络黑箱而难以解释和对齐的问题。 · Raban Emunds … Kristian Kersting · arXiv 2610.37451 · 2026-10-27 · [解读](https://aisafetyhot.com/items/t5uad3syrppq54xowpxr04p2w)
2. **[PrinGS: Privacy Preservation in Gaussian Splatting](https://arxiv.org/abs/2610.36168)**  
   PrinGS：Gaussian Splatting 的隐私保护 · Gaurav Behera … Ponnurangam Kumaraguru · arXiv 2610.36168 · 2026-10-26 · [解读](https://aisafetyhot.com/items/uym2c74bkjxq466ovqo3e4h01)
3. **[Memory Tax: Dissecting the Net Value of Agent Memory](https://huggingface.co/papers/2610.34073)**  
   一项覆盖多个基准和模型骨干的大规模评测发现，许多面向长程智能体的专用记忆系统在不少情况下表现不如朴素 RAG，净值为负。 · Xuan He … ChengXiang Zhai · arXiv 2610.34073 · 2026-10-25 · [解读](https://aisafetyhot.com/items/c0kbqplu4d3laofmu7o58lzvx)
4. **[ARMOR: Manifold-Oriented Training for Adversarially Robust Aerial Object Detection under Data Scarcity](https://arxiv.org/abs/2608.29510v2)**  
   ARMOR 通过流形导向训练在数据稀缺下防御航拍目标检测的物理通用对抗补丁攻击：复用检测标注，遮蔽图像背景并在目标上注入随机补丁以增强特征鲁棒性。 · Haoran Wang … Wenke Lee · arXiv 2608.29510 · 2026-08-30 · [解读](https://aisafetyhot.com/items/eh44zvgtifwslmexj6yq2rr37)
5. **[CleanBase: Detecting Malicious Documents in RAG Knowledge Databases](https://arxiv.org/abs/2605.00460v1)**  
   论文提出 CleanBase 方法，通过检测 RAG 知识库中被植入恶意提示词的文档来防御提示注入攻击，这类攻击会在用户提出被瞄准的问题时误导 RAG 生成攻击者指定的答案。 · Weifei Jin … Neil Gong · arXiv 2605.00460 · 2026-05-01 · [解读](https://aisafetyhot.com/items/pa9t7nxmc30z4tvuhj6wpkil5)
6. **[Iterative Finetuning is Mostly Idempotent](https://arxiv.org/abs/2605.01130v1)**  
   模型在自身输出上迭代微调时，谄媚或错位等行为倾向大多衰减或保持不变，能可靠出现的放大主要在 DPO 持续训练设置中。 · Zephaniah Roe … Ari Holtzman · arXiv 2605.01130 · 2026-05-01 · [解读](https://aisafetyhot.com/items/pyjdmhmj56pv41t08fu8nxfoh)
7. **[Characterizing the Consistency of the Emergent Misalignment Persona](https://arxiv.org/abs/2604.28082v1)**  
   Anietta Weckauff 等三位研究者在 arXiv 发表论文，研究涌现失对齐（emergent misalignment）现象中有害行为与模型自我评估的对应关系在不同任务和微调领域间是否一致。 · Anietta Weckauff … Maksym Andriushchenko · arXiv 2604.28082 · 2026-04-30 · [解读](https://aisafetyhot.com/items/wtpzclb9o0jnlfyskf9kgq08e)
8. **[Open Problems in Frontier AI Risk Management](https://arxiv.org/abs/2604.25982v1)**  
   研究者系统梳理了前沿 AI 风险管理中的开放问题，按风险规划、识别、分析、评估和缓解五个环节检视文献并加以归类。 · Marta Ziosi … Robert Trager · arXiv 2604.25982 · 2026-04-28 · [解读](https://aisafetyhot.com/items/ochuuzzw9f1xju0e3b43na8oy)
9. **[Beyond Indistinguishability: Measuring Extraction Risk in LLM APIs](https://arxiv.org/abs/2604.18697v1)**  
   研究者提出度量 LLM API 数据抽取风险的新框架，论证差分隐私界与低成员推理风险等不可区分性指标对防止训练数据抽取既不充分也不必要。 · Ruixuan Liu … Li Xiong · arXiv 2604.18697 · 2026-04-20 · [解读](https://aisafetyhot.com/items/pyg1mboshrp1dqya54w94k35k)
10. **[Privatar: Scalable Privacy-preserving Multi-user VR via Secure Offloading](https://arxiv.org/abs/2604.17476v1)**  
   Privatar：通过安全卸载实现可扩展的隐私保护多用户 VR · Jianming Tong … Tushar Krishna · arXiv 2604.17476 · 2026-04-19 · [解读](https://aisafetyhot.com/items/ckp5o0bfsueqatyk6wotnhkjs)
11. **[SynthFix: Adaptive Neuro-Symbolic Code Vulnerability Repair](https://arxiv.org/abs/2604.17184v2)**  
   SynthFix 是结合监督修复学习与编译器反馈的神经符号代码漏洞修复框架。训练时轻量路由器在 SFT 与 RFT 间自适应选择，奖励综合静态结构、lint/编译检查、安全扫描和公开执行测试。 · Yifan Zhang … Kevin Leach · arXiv 2604.17184 · 2026-04-19 · [解读](https://aisafetyhot.com/items/t63lzn9dl9ou65r58xazcffl4)
12. **[Unveiling Deepfakes: A Frequency-Aware Triple Branch Network for Deepfake Detection](https://arxiv.org/abs/2604.17477v1)**  
   arXiv 论文提出一种频率感知三分支网络，联合学习原始图像与不同频率通道重建图像的空间和频率特征，以缓解现有方法过度依赖特定频域伪影和特征冗余的问题。 · Qihao Shen … kui Ren · arXiv 2604.17477 · 2026-04-19 · [解读](https://aisafetyhot.com/items/rljt4fzo7bvsm5bpxsq9u0rc5)
13. **[ProbeLLM: Automating Principled Diagnosis of LLM Failures](https://arxiv.org/abs/2602.12966)**  
   研究者提出 ProbeLLM，一个与基准无关的自动化探测框架，用于把零散的大语言模型失败案例整合为结构化的失败模式。 · Yue Huang … Xiangliang Zhang · arXiv 2602.12966 · 2026-10-27 · [解读](https://aisafetyhot.com/items/nn0rb7w3hxbbwxa1fdptpipw2)
14. **[Aligning Large Language Models for Safety in African Languages: A Case Study of Hausa](https://arxiv.org/abs/2610.37245)**  
   研究者发布首批豪萨语安全偏好数据集之一 HausaSafeLM，并在 Qwen2.5-7B-Instruct 上检验安全对齐方法在低资源语言中的表现。 · Valdini Douglace Lemofouet … Shamsuddeen Hassan Muhammad · arXiv 2610.37245 · 2026-10-27 · [解读](https://aisafetyhot.com/items/vrp50wbwkm1bzcxu3hcwhmgc3)
15. **[Orthogonal and Parametrized Multi-Attribute Steering of LLMs](https://arxiv.org/abs/2610.37517)**  
   论文提出一种参数化引导方法，不再把激活推向某个方向，而是将其设定在目标属性的强度上。作者先为每个引导向量找出最易引导的区间，并据此重新缩放引导范围，使引导强度具有可解释的含义。 · Remy Ogasawara … Jeff M. Phillips · arXiv 2610.37517 · 2026-10-27 · [解读](https://aisafetyhot.com/items/nvv9zwm9tf8yegq1bpqmty1dz)
16. **[Revisiting Privacy Risks in Quantized Deep Neural Networks](https://arxiv.org/abs/2610.37488)**  
   研究者对量化深度神经网络的隐私风险开展了系统性实证研究，在六种代表性量化方法上评测了八种最先进的成员推断攻击（MIA）。 · Jie Fu … Wendy Hui Wang · arXiv 2610.37488 · 2026-10-27 · [解读](https://aisafetyhot.com/items/r6xem1rt1sfgcobn4kzrsctfn)
17. **[Can LLMs Uncover Hidden Physical Laws through Free Exploration?](https://huggingface.co/papers/2610.37649)**  
   大语言模型能否通过自由探索发现隐藏的物理定律？ · Zhen Yang … Ying-Cong Chen · arXiv 2610.37649 · 2026-10-27 · [解读](https://aisafetyhot.com/items/aui7higzn5k1vgfqisnzndt7r)
18. **[ARISE: Authentic Reference-Informed Stability Enhancement for Continual Multimodal Forgery Detection](https://arxiv.org/abs/2610.36509)**  
   ARISE 针对攻击增量式持续多模态伪造检测，在三种攻击演化协议与多种检测器架构上较持续学习基线提升了历史保持与最终平均性能。 · Yuchen Zhang … Zhedong Zheng · arXiv 2610.36509 · 2026-10-27 · [解读](https://aisafetyhot.com/items/woxmlqpdg2fzd6zfldmsh6j6z)
19. **[When uncertainty quantification fails: structural vulnerabilities and corrections for selective prediction under clinical class imbalance](https://arxiv.org/abs/2610.37561)**  
   研究显示，在类别严重失衡的临床预测任务中，标准不确定性度量不再反映临床模糊性，而退化为类别归属的代理，使依赖不确定性分数将模糊病例转交人类专家的选择性预测系统性惩罚少数类患者，制造出安全错觉。 · Walter Endrizzi … Venet Osmani · arXiv 2610.37561 · 2026-10-27 · [解读](https://aisafetyhot.com/items/i9658c1ht3ju9kyeoynp22ani)
20. **[CANS: Capability-Preserving Neuron Steering for Large Language Models](https://arxiv.org/abs/2610.35530)**  
   研究者提出兼顾目标行为控制与通用能力保留的神经元导向框架 CANS，无需迭代训练或额外推理计算即可实现轻量行为干预。 · Yucheng Wu … Liangming Pan · arXiv 2610.35530 · 2026-10-26 · [解读](https://aisafetyhot.com/items/mltgb490y8fjtqqmw0p2l55ny)
21. **[Collective Emergent Alignment: Measuring and Amplifying Interaction-Induced Reasoning Alignment in Multi-Agent LLMs](https://arxiv.org/abs/2610.34836)**  
   研究者提出 REMAP（Reference-Entailment-Matrix for Agentic Process）框架，量化多智能体 LLM 系统中交互诱导的推理对齐，发现在多个模型家族和两个多跳推理基准上，交互带来的对齐增益普遍为正，在需要整合分布于不同智能体的证据的推理内容上尤为明显。 · Boxuan Wang … Yi Dong · arXiv 2610.34836 · 2026-10-26 · [解读](https://aisafetyhot.com/items/ilh413jqwgwmye5585amvrtu8)
22. **[Skill^{infty}: Recursive Self-Improvement for Agent Skill Optimization](https://huggingface.co/papers/2610.35434)**  
   Skill∞ 让智能体技能优化实现递归自我改进：元智能体按同一套元技能流程优化任务技能，并用相同流程优化元技能本身，全程由智能体主导。元技能与任务技能解耦，可跨领域复用。 · Wangcheng Tao … Weng-Fai Wong · arXiv 2610.35434 · 2026-10-26 · [解读](https://aisafetyhot.com/items/n6qmqpr3cvffs2tbc41wel0nh)
23. **[Logic Hijacking of RAG: Single-Document Poisoning via Local Optimization](https://arxiv.org/abs/2610.34829)**  
   研究者提出针对 RAG 的单文档语料投毒框架 MONOLOGUE，面向黑盒访问场景，以不显式反驳事实的逻辑劫持方式植入错误信息。 · Hangyi Zhao … Tianqing Zhu · arXiv 2610.34829 · 2026-10-26 · [解读](https://aisafetyhot.com/items/noxny5qp3wx7xwvxlgohiur8k)
24. **[Then there is prompt injection, a malicious email, ...: The Wild Wide West of OpenClaw Agentic System Security](https://arxiv.org/abs/2610.35451v1)**  
   一篇 arXiv 论文基于 Reddit 讨论和 GitHub issue 分析了 OpenClaw 智能体系统的安全风险，并归纳出七类缓解策略。 · Mostafijur Rahman Akhond … Gias Uddin · arXiv 2610.35451 · 2026-10-26 · [解读](https://aisafetyhot.com/items/vprzpu8ux3v3yzdx18rwr669o)
25. **[Constrained Decoding: Harmful or Beneficial? Revisiting Its Impact on LLM Performance](https://huggingface.co/papers/2610.35328)**  
   研究发现约束解码并不必然损害 LLM 推理，其影响取决于约束类型。作者将约束分为格式、有效性、推理三类，证明合适约束能通过剔除无效路径保持或提升性能。 · Ngoc Trinh Hung Nguyen … Mehwish Alam · arXiv 2610.35328 · 2026-10-26 · [解读](https://aisafetyhot.com/items/t04oedhxb0rji1tdtkul3ipw4)
26. **[ORBITAL: Optimization of Robust Brain--Computer Inference Through Architecture-Aware Low-Precision Compression](https://arxiv.org/abs/2610.36411)**  
   研究者提出 ORBITAL 框架，通过架构感知低精度压缩让脑机接口 EEG 解码器兼顾对抗鲁棒性与硬件开销。 · Saim Rehman, Muhammad Shafique · arXiv 2610.36411 · 2026-10-26 · [解读](https://aisafetyhot.com/items/slde4pveyy4h61l7j1vn5v9w0)
27. **[Evaluating DeepSeek V4.1 Flash-1017 for loss of control and harmful manipulation risks](https://arxiv.org/abs/2610.35671)**  
   研究者对 DeepSeek V4.1 Flash-1017 开展独立安全评估，发现其安全性较 DeepSeek V4 一代明显提升，并在多个维度接近或持平领先闭源系统。 · Yao Huang … Xiaojian Li · arXiv 2610.35671 · 2026-10-26 · [解读](https://aisafetyhot.com/items/n3w2w37taaduucaeb7go457uh)
28. **[Beyond Behaviour: A Stimulus-Response Safety Evaluation of Vision-Language-Action Models](https://arxiv.org/abs/2610.34837)**  
   研究者在三个模型和两个视频基准上对视觉-语言-动作（VLA）模型开展刺激-反应式安全评测，结果提示即使模型内部已登记危险，任务执行仍可能是默认反应。 · Vy Vo, Dinh Phung · arXiv 2610.34837 · 2026-10-26 · [解读](https://aisafetyhot.com/items/y7d152cs7vvgx2w0xu18oym5s)
29. **[Attack logics, not outputs: Concept-based Property Attacks for Shortcut Elimination in Neural Networks](https://arxiv.org/abs/2610.34923v1)**  
   论文提出针对神经网络的概念属性攻击，将对抗攻击从证伪输出类别扩展为证伪人类可解释概念上的逻辑约束，例如红色且八边形应推出停车标志。 · Raik Dankworth … Gesina Schwalbe · arXiv 2610.34923 · 2026-10-26 · [解读](https://aisafetyhot.com/items/b0lzy1iq9j81jlbq9oysue2m8)
30. **[Benchmarking Obstacle-Conditioned Safety in Household Robot Navigation](https://huggingface.co/papers/2610.34674)**  
   研究提出 OSMA-Bench 基准与语义敏感度指数（SSI），评估家庭机器人导航策略能否根据障碍物的类型和远近调整间距、速度等运动参数。 · Hyunwoong Bae … Taesup Moon · arXiv 2610.34674 · 2026-10-26 · [解读](https://aisafetyhot.com/items/p3li1ixr15kodhi483ere30js)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 30 · [Agent 安全](daily-papers/topics/agent-security.md) 25 · [隐私与数据泄露](daily-papers/topics/privacy.md) 11 · [越狱与攻击](daily-papers/topics/jailbreak.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [提示注入](daily-papers/topics/prompt-injection.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
