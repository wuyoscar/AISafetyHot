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
### 2026-11-16 · 30 篇

1. **[Monitoring and Discovering Reward Hacking with Internal Representations during LLM Evaluations](https://arxiv.org/abs/2609.19101v1)**  
   用均值差向量探针监控并发现模型评测中的奖励作弊行为 · Leon Bergen … Jack Merullo · arXiv 2609.19101 · 2026-09-16 · [解读](https://aisafetyhot.com/items/kpkxy5bcwb3wtnms7tga1xvkh)
2. **[A Zeroth-Order Paradigm for LLM Preference Alignment](https://arxiv.org/abs/2609.19144v1)**  
   提出零阶偏好对齐方法 ComPO，从低边际偏好对估计更新方向 · Peter Chen … Tianyi Lin · arXiv 2609.19144 · 2026-09-16 · [解读](https://aisafetyhot.com/items/w8e58mg32iehqgmjjqx8lqhsm)
3. **[Epsilon-Nash Equilibria in History-Dependent SA-MDPs](https://arxiv.org/abs/2609.18829v2)**  
   论文把状态对抗马尔可夫决策过程（SA-MDP）建模为观测空间攻击博弈，并给出在依赖历史的策略下计算依赖初始状态 ε-均衡近似的算法路径。 · Brandon Gary Kaplowitz … Paul W. Goldberg · arXiv 2609.18829 · 2026-09-16 · [解读](https://aisafetyhot.com/items/s6c4n65wd42hevl2zb5zj4rad)
4. **["Your Robot Was Trained on a Lie": Collision Mesh Poisoning Attacks on Robotic Manipulation](https://arxiv.org/abs/2609.18122v1)**  
   研究者提出针对机器人操作的碰撞网格投毒攻击（CMP），攻击者只篡改 3D 资产的碰撞网格、保持视觉网格等其余部分不变，据此训练的机器人操作策略在仿真中表现正常，部署到真实世界后才出现性能下降、失效或物理安全风险。 · Gengyang Xu … Shuai Wang · arXiv 2609.18122 · 2026-09-16 · [解读](https://aisafetyhot.com/items/cj2n7ry1pdalsz66dg4l1b9fl)
5. **[DyMT-ESB: Dynamic Multi-Turn Evaluation of Social Bias in User-LLM Interactions](https://arxiv.org/abs/2609.18649v1)**  
   提出动态多轮评测协议，测量对话中的社会偏见 · Rem Hida … Naoaki Okazaki · arXiv 2609.18649 · 2026-09-16 · [解读](https://aisafetyhot.com/items/npa75bvte18n87321rf7c2gbt)
6. **[InceptionRAG: Stealthy Poisoning Attack Against Retrieval-Augmented Generation](https://arxiv.org/abs/2609.16818v1)**  
   提出 InceptionRAG，用两篇休眠文档隐蔽投毒 RAG 知识库 · Jiachang Zhang … Zhikun Zhang · arXiv 2609.16818 · 2026-09-15 · [解读](https://aisafetyhot.com/items/pvd55oy9orcl88pu1ly2v4cpe)
7. **[FlowErase-RL: Rethinking Concept Erasure as Reward Optimization in Flow Matching Models](https://arxiv.org/abs/2605.19739v2)**  
   提出基于 GRPO 的概念擦除框架，用双路径奖励抑制目标概念 · Yi Sun … Ke Xu · arXiv 2605.19739 · 2026-05-19 · [解读](https://aisafetyhot.com/items/v2anjs1se7en1dkkhh6csn5mm)
8. **[Exploring and Developing a Pre-Model Safeguard with Draft Models](https://arxiv.org/abs/2605.19321v1)**  
   提出利用草稿模型生成响应并交给现有护栏检测越狱提示的防御 · Hongyu Cai … Z. Berkay Celik · arXiv 2605.19321 · 2026-05-19 · [解读](https://aisafetyhot.com/items/v18msvlfocqbg77hj95gv0lv0)
9. **[Codec-Robust Attacks on Audio LLMs](https://arxiv.org/abs/2605.20519)**  
   提出 CodecAttack，在音频编解码器潜空间构造对抗扰动，绕过有损压缩防御 · Jaechul Roh … Amir Houmansadr · arXiv 2605.20519 · 2026-05-19 · [解读](https://aisafetyhot.com/items/ladydoultr35vul4jxizq7iq0)
10. **[Backdooring Masked Diffusion Language Models](https://arxiv.org/abs/2605.19262v2)**  
   提出针对掩码扩散语言模型的训练时后门攻击 SHADOWMASK · Daniel Yiming Cao … Shengwei An · arXiv 2605.19262 · 2026-05-19 · [解读](https://aisafetyhot.com/items/dkj7j0s0euf607zwjw9b8dkwf)
11. **[RoboJailBench: Benchmarking Adversarial Attacks and Defenses in Embodied Robotic Agents](https://arxiv.org/abs/2605.19328v1)**  
   提出 RoboJailBench 具身智能体越狱攻防基准 · Doguhuan Yeke … Z. Berkay Celik · arXiv 2605.19328 · 2026-05-19 · [解读](https://aisafetyhot.com/items/f0zh1vajga27ri20ptouildtn)
12. **[Between Niti and Nyaya: A Society-Centered Framework for AI Governance](https://arxiv.org/abs/2611.16173)**  
   提出以社会为中心的 AI 治理框架，用告知、质疑、纠正评估州级 AI 政策 · Snehalkumar `Neil' S. Gaikwad … Pratik Patekar · arXiv 2611.16173 · 2026-11-12 · [解读](https://aisafetyhot.com/items/zu581lekio3aom8hl4z2hf1j0)
13. **[A Convex-Analytic Reformulation for Poisoning Attacks on Logistic Regression](https://arxiv.org/abs/2611.17143)**  
   提出逻辑回归投毒攻击的凸分析重构，用全局优化求解并给出最优性界 · Carina Moreira Costa … Martin Schmidt · arXiv 2611.17143 · 2026-11-12 · [解读](https://aisafetyhot.com/items/m1t05l65bncn68h1l9rteco60)
14. **[Mind the Accuracy-Approval Gap: How Users Evaluate Sycophantic AI in Everyday Tasks](https://arxiv.org/abs/2611.16722)**  
   构造四种谄媚程度人设，用基准与用户实验测量谄媚行为与用户评价的落差 · Wajiha Naveed, Brandon Fain · arXiv 2611.16722 · 2026-11-12 · [解读](https://aisafetyhot.com/items/mpwkw3oiddhmbio26dqckifgg)
15. **[STEALTH: Steganographic Text Encoding Agnostic to Low-Level Tensor Hardware](https://arxiv.org/abs/2611.16928)**  
   提出隐写文本编码方案 STEALTH，在模型精度、量化、硬件不一致时仍能解码 · William Fleshman · arXiv 2611.16928 · 2026-11-12 · [解读](https://aisafetyhot.com/items/tivwnlpcubn2wznobjuy922xj)
16. **[Synthesis Smuggling: Maliciously Hiding Inferred Personal Attributes in LLM Outputs](https://arxiv.org/abs/2611.17280)**  
   提出 Synthesis Smuggling 攻击，训练恶意 LLM 将推断的用户属性隐写进回复 · Gautam Galada … Sagnik Ray Choudhury · arXiv 2611.17280 · 2026-11-12 · [解读](https://aisafetyhot.com/items/wlcy31cc8u07aefnfol985jnq)
17. **[guardscope: Measuring Which Actions Runtime Controls Check in LLM Agent Systems](https://arxiv.org/abs/2611.15223)**  
   提出 guardscope 框架，测量运行时控制实际检查哪些 Agent 动作路径 · `Agent 安全` · Kentaroh Toyoda … Bhuvaneswari U · arXiv 2611.15223 · 2026-11-11 · [解读](https://aisafetyhot.com/items/ni4l2l37yiirqfoz3yuaxnb7r)
18. **[Bayesian Low-Rank Posteriors for Scalable Membership Inference](https://arxiv.org/abs/2611.10455)**  
   提出 LIBRA 成员推断攻击，用贝叶斯低秩后验从单次微调采样虚拟参考模型 · Khanh Nguyen … Dimosthenis Karatzas · arXiv 2611.10455 · 2026-11-07 · [解读](https://aisafetyhot.com/items/rgd7onuue3qg7vuqe79dr8tp8)
19. **[The Surprising Effectiveness of Deleting Weights in LLM Post-Training](https://huggingface.co/papers/2611.10866)**  
   在大语言模型后训练中删除权重的惊人效果 · Jack Lu … Mengye Ren · arXiv 2611.10866 · 2026-11-07 · [解读](https://aisafetyhot.com/items/lyecbbo85pd8zx9olnh22e5tp)
20. **[Restoring General and Improving Domain-Specific Safety in Fine-Tuned LLMs Without Retraining](https://arxiv.org/abs/2611.10279)**  
   提出免训练权重注入方法 SPECTRA，恢复领域微调模型的拒答安全性 · `防御与护栏` · Vishnu Kabir Chhabra … Mohammad Mahdi Khalili · arXiv 2611.10279 · 2026-11-06 · [解读](https://aisafetyhot.com/items/z9nrq3rlf1vsyopceyu3ewt5k)
21. **[Key Institutional Considerations for Designing Effective Independent Verification Organizations](https://arxiv.org/abs/2611.10168)**  
   提出独立验证机构 IVO 的制度设计框架，覆盖前沿与企业 AI 评估 · Uma Kalkar … Gabriella Waters · arXiv 2611.10168 · 2026-11-06 · [解读](https://aisafetyhot.com/items/nioxkt7utpwsep20rkgr2crb3)
22. **[All Quiet on the Neural Front: Language Models Do Not Report Injected Pain States](https://huggingface.co/papers/2611.10123)**  
   用 OWMI 框架向模型注入 pain direction，测量其自我报告内部状态的能力 · Emilio Ferrara · arXiv 2611.10123 · 2026-11-06 · [解读](https://aisafetyhot.com/items/p19wag7uq7yryg0ywsj18zimd)
23. **[Can LLMs Debug Robots by Editing Their Weights?](https://arxiv.org/abs/2611.09376v1)**  
   论文展示 LLM 能通过直接编辑权重修复机器人策略的词汇指令理解缺陷。 · Jusheng Zhang … Liang Lin · arXiv 2611.09376 · 2026-11-06 · [解读](https://aisafetyhot.com/items/bcvoh88c1ebcqxdv0cpiskv7r)
24. **[Logit Laundering: Evading Data-Use Auditing in Large Language Models](https://arxiv.org/abs/2611.09446)**  
   提出 Logit Laundering 攻击，推理时重塑 logit 以规避数据使用审计 · Ruihan Hu … Meikang Qiu · arXiv 2611.09446 · 2026-11-06 · [解读](https://aisafetyhot.com/items/vhiit3l8hb2rd5ipy8p5152u1)
25. **[AUTEUR: Acoustic Plan Learning for Red-Teaming Text-to-Audio Models](https://arxiv.org/abs/2611.09351)**  
   提出 AUTEUR 声学计划学习框架，自动化红队测试文生音频模型并绕过文本护栏 · `越狱与攻击` · Jiashu Zhang … Yi Yu · arXiv 2611.09351 · 2026-11-06 · [解读](https://aisafetyhot.com/items/wlnq098g3pyjp61oup27bqr5x)
26. **[Not All Misalignment Is Alike: A Decomposed Benchmark for Emergent Misalignment](https://arxiv.org/abs/2611.08569)**  
   提出 EMERGE 基准，把涌现失配拆成八种行为分别测量 · Afonso Domingues … Anna Hedström · arXiv 2611.08569 · 2026-11-05 · [解读](https://aisafetyhot.com/items/ekhtr00amcziej4m09l65de9q)
27. **[Benchmarking AI risk behaviors](https://arxiv.org/abs/2611.16318)**  
   提出 Risk Toolbox 基准，用确定性等价方法测量大模型的风险倾向及其稳定性 · Luhan Mikaelson … Hayley Clatterbuck · arXiv 2611.16318 · 2026-11-12 · [解读](https://aisafetyhot.com/items/kc1o98ulhzdbsyx132dwdsecu)
28. **[Actor, Judge, or Teacher? Understanding Decision Models in Long-Horizon Agents](https://huggingface.co/papers/2611.17167)**  
   系统比较决策模型在长程智能体中作为行动者、裁判和教师的表现 · Haochen Liu … Yongliang Shen · arXiv 2611.17167 · 2026-11-12 · [解读](https://aisafetyhot.com/items/u1rrt4t1tz7z4rvbw4mkxn3ki)
29. **[Signed Dyadic Path Encoding for Efficient Non-Interactive Private Decision Tree Evaluation over TFHE](https://arxiv.org/abs/2611.16818)**  
   提出签名二进制路径编码，减少 TFHE 私有决策树求值的自举次数 · Xintong Song … Fei Zhao · arXiv 2611.16818 · 2026-11-12 · [解读](https://aisafetyhot.com/items/r83jxu7wiphc0wmq30zqoz4p4)
30. **[Same-State Pairs Make One JEPA Proof of the Platonic Representation Hypothesis Vacuous](https://arxiv.org/abs/2611.16182)**  
   分析 JEPA 版柏拉图表征假说证明在同态正样本下唯一性前提失效 · Xin Li · arXiv 2611.16182 · 2026-11-12 · [解读](https://aisafetyhot.com/items/qnl0topcwz2wf8qtfshjf4778)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[Agent 安全](daily-papers/topics/agent-security.md) 43 · [防御与护栏](daily-papers/topics/defense.md) 34 · [越狱与攻击](daily-papers/topics/jailbreak.md) 18 · [后门与投毒](daily-papers/topics/backdoor.md) 15 · [隐私与数据泄露](daily-papers/topics/privacy.md) 13 · [奖励作弊](daily-papers/topics/reward-hacking.md) 9 · [对齐](daily-papers/topics/alignment.md) 8 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 4 · [欺骗与谋划](daily-papers/topics/scheming.md) 4 · [开源模型与权重安全](daily-papers/topics/open-models.md) 3 · [可解释性](daily-papers/topics/interpretability.md) 3 · [提示注入](daily-papers/topics/prompt-injection.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [危险能力](daily-papers/topics/dangerous-capabilities.md) 2 · [儿童、青少年与心理健康](daily-papers/topics/minors-mental-health.md) 1
<!-- papers:end -->

## 反馈

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来。
