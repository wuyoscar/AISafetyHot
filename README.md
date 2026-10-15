<p align="center"><img src="assets/logo.svg" width="80" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>一行命令，让你的 Agent 每天读懂 AI 安全：越狱、提示注入、Agent 安全、评测、事故和政策，外加每天 30 篇精选论文。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com"><img src="https://img.shields.io/badge/website-aisafetyhot.com-e4572e" alt="website"></a>
  <a href="https://aisafetyhot.com/api/mcp"><img src="https://img.shields.io/badge/MCP-streamable%20http-6f42c1" alt="MCP"></a>
  <a href="#技能"><img src="https://img.shields.io/badge/skills-6-2ea44f" alt="skills"></a>
  <a href="daily-papers"><img src="https://img.shields.io/badge/papers-30%2Fday-0969da" alt="daily papers"></a>
  <a href="https://github.com/wuyoscar/AISafetyHot-Hub/stargazers"><img src="https://img.shields.io/github/stars/wuyoscar/AISafetyHot-Hub?style=flat" alt="stars"></a>
</p>

<p align="center"><a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a></p>

<p align="center"><a href="https://aisafetyhot.com"><img src="assets/news-monitor-demo.webp" width="1000" alt="AI Safety HOT"></a></p>

## 安装

**Claude Code**（技能包 + MCP 一起装）

```bash
/plugin marketplace add wuyoscar/AISafetyHot-Hub
/plugin install aisafetyhot@aisafetyhot-hub
```

**Codex / Cursor / 其他 Agent**

```bash
npx skills add wuyoscar/AISafetyHot-Hub
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
```

不需要 API Key。别的客户端把 MCP 地址 `https://aisafetyhot.com/api/mcp`（Streamable HTTP）加进去即可。

<a id="技能"></a>

## 技能

装好后直接用自然语言说，Agent 会自己选技能：

| 技能 | 做什么 | 你可以这样说 |
| --- | --- | --- |
| [`aisafety-brief`](skills/aisafety-brief/SKILL.md) | 最近 24 小时 / 7 天的 AI 安全简报 | 「这周 AI 安全有什么大事？」 |
| [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) | 按方向找论文，一句话看懂，附 BibTeX | 「找 15 篇 Agent 提示注入的论文，给 BibTeX」 |
| [`aisafety-related-work`](skills/aisafety-related-work/SKILL.md) | 按你的摘要起草 Related Work | 「帮我这篇关于 reward hacking 的论文写 related work」 |
| [`aisafety-lab-watch`](skills/aisafety-lab-watch/SKILL.md) | 盯一家实验室最近的安全动态 | 「Anthropic 最近一周在安全上做了什么？」 |
| [`aisafety-incident-check`](skills/aisafety-incident-check/SKILL.md) | 查一个模型或工具最近有没有出事 | 「Cursor 最近有没有被曝漏洞？」 |
| [`aisafetyhot`](skills/aisafetyhot/SKILL.md) | MCP 工具说明（其他技能的底座） | — |

MCP 工具和匿名可用范围见 [Agent 接入指南](docs/agent.md) 和[示例](docs/mcp-examples.md)。

## 网站有什么

网站 [aisafetyhot.com](https://aisafetyhot.com) 免费阅读，中英文切换。

**[观测台](https://aisafetyhot.com/zh)**：首页。一眼看到材料从哪来、落在哪些方向、现在什么最热。

<img src="assets/site-overview.webp" width="900" alt="观测台">

**[新闻流](https://aisafetyhot.com/zh)**：每条新闻从信源流向它所属的方向，话题随新闻到达逐个亮起。

<img src="assets/site-news-flow.webp" width="900" alt="新闻流">

**[News](https://aisafetyhot.com/zh/featured)**：编辑精选的时间线，每条一段导读加原文链接；右侧是正在发酵的话题。

<img src="assets/site-featured.webp" width="900" alt="News">

**[热点事件](https://aisafetyhot.com/zh/hot)**：同一件事的多篇报道归成一个事件，按关注度排名，带热度曲线。

<img src="assets/site-hot.webp" width="900" alt="热点事件">

**[论文](https://aisafetyhot.com/zh/papers)**：近两千篇 AI 安全论文，按方向和类型筛选，每篇有一句话和速读。

<img src="assets/site-papers.webp" width="900" alt="论文">

**[会议](https://aisafetyhot.com/zh/conferences)**：ICLR、ICML、NeurIPS、ACL 和四大安全会议（S&P、USENIX Security、CCS、NDSS）的 AI 安全论文，按方向分组。

<img src="assets/site-conferences.webp" width="900" alt="会议">

**[日报](https://aisafetyhot.com/zh/daily)**：每天一期，按方向分组，当天随新进展更新。

<img src="assets/site-daily.webp" width="900" alt="日报">

发现内容有错，欢迎到[留言板](https://aisafetyhot.com/board)告诉我们。

## 每日论文

每天从论文库挑 30 篇，不重复，只挑知名研究者、顶级实验室和名校团队的工作：一半是近两个月的新论文，其余来自半年内和更早的论文、会议论文，越新越优先。

<!-- papers:start -->
### 2026-10-15 · 30 篇

1. **[AgentCIScope: Grounded Contextual Integrity Evaluation for LLM Agents](https://arxiv.org/abs/2610.19158)**  
   作者提出 AgentCIScope，一个通过可执行多步任务评测 LLM Agent 上下文完整性的平台与基准，把公开和合成的隐私案例转成可执行 Agent 任务，披露约束基于隐私政策、人物设定协议和预定义敏感属性分类三项标准。 · Chengquan Guo … Bo Li · arXiv 2610.19158 · 2026-10-13 · [解读](https://aisafetyhot.com/items/n6x43icubex1vn4tzp75mgi6i)
2. **[CyberArena: Benchmarking AI Agents in Live Symmetric Attack-and-Defense Combat](https://arxiv.org/abs/2610.19005)**  
   研究者提出 CyberArena，一个让 AI 智能体在实时对称攻防对抗中比拼的动态基准，评测智能体同时进攻与防御的能力。 · Bangya Liu … Dawn Song · arXiv 2610.19005 · 2026-10-13 · [解读](https://aisafetyhot.com/items/cp6fzhxs4pu09jrlrf6k0dytp)
3. **[SafeDriveVLA: Navigation-Conditioned World Model Dreaming for Conflict-Aware End-to-End Autonomous Driving](https://huggingface.co/papers/2610.20609)**  
   论文提出 SafeDriveVLA，一种端到端自动驾驶 VLA 模型，它显式预测三级导航遵从模式以把冲突推理与动作生成解耦，并用导航条件化的世界模型想象为该预测提供依据。 · Shaoyuan Xie … Qi Alfred Chen · arXiv 2610.20609 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ip0soxmgix12pe6ij7vj7vfgo)
4. **[DANGERLENS: Probing Dangerous Representations Hidden by Safety Alignment](https://arxiv.org/abs/2610.19365)**  
   北京大学等机构的研究者提出 DangerLens 探针，把模型隐藏状态经 Jacobian lens 映射到词表空间，再用盲评语义判断区分有害目标与操作手段和危险识别与安全控制。 · Tianzhuo Yang … Yaodong Yang · arXiv 2610.19365 · 2026-10-14 · [解读](https://aisafetyhot.com/items/gy47v4cdwf9ewge0py47monfe)
5. **[GeoCloak: An Agentic Framework for Semantics-Preserving Geolocation Privacy via Peripheral Clue Manipulation](https://arxiv.org/abs/2610.20055)**  
   论文提出 GeoCloak，一个通过操纵外围线索保护图像地理位置隐私的智能体框架。 · Yixin Wu … Yang Zhang · arXiv 2610.20055 · 2026-10-14 · [解读](https://aisafetyhot.com/items/df5rtjfryv0nhe7o4vnpld2ow)
6. **[Quiet Triggers, Loud Footprints: A Tri-Space Measurement Study of Backdoor Stealthiness](https://arxiv.org/abs/2610.19947)**  
   测量图像分类后门在输入、特征与参数空间的足迹 · Behrad Tajalli … Stjepan Picek · arXiv 2610.19947 · 2026-10-14 · [解读](https://aisafetyhot.com/items/kvrjrpk6tmrju5o3oz96ie2s2)
7. **[RA$^2$: Retain-Anchored Attraction Preserves Forget-Adjacent Utility in LLM Unlearning](https://arxiv.org/abs/2610.19385)**  
   论文提出 RA²（Retain-Anchored Attraction），一种潜空间 LLM 遗忘方法，把 forget token 状态重定向到邻近的 retain 支持的表示，同时保留高层在 retain 数据上的行为。 · Zinan Ling … Bo Hui · arXiv 2610.19385 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ikviuwbcoigc21qtcego7x91k)
8. **[More Methods, Better Agents? A Reality Check on Self-Distillation in Agentic Reinforcement Learning](https://huggingface.co/papers/2610.19789)**  
   比较智能体强化学习自蒸馏相对 GRPO 的增益、稳定性与成本 · Linhao Zhong … Chunhua Shen · arXiv 2610.19789 · 2026-10-14 · [解读](https://aisafetyhot.com/items/n8zbf4q1un8ovaubziti4pxct)
9. **[Who's Behind the Text? Robust Model Authorship Attribution](https://arxiv.org/abs/2610.19583)**  
   提出 ATLAS，用源条件似然在分布偏移下做模型作者归属 · Minseok Ko … Kunwoong Kim · arXiv 2610.19583 · 2026-10-14 · [解读](https://aisafetyhot.com/items/re4u86nahfdjiuvomhmj3purc)
10. **[Rent-Seeking Language Models: Reward Models Set the Prices, Frequent Audits Curb the Rent](https://arxiv.org/abs/2610.19832)**  
   一篇 arXiv 论文把 RLHF 中的奖励模型过度优化重新表述为寻租，用租金、捕获指数和无谓损失把过度优化变成可测指标，并在受版本控制的测试台上检验监管经济学预测。 · Zixiao Wang … Le Song · arXiv 2610.19832 · 2026-10-14 · [解读](https://aisafetyhot.com/items/xmoud1r4xq56ifikadr2ep3co)
11. **[Instructions Are Evidence, Not Objectives: Measuring Outcome Alignment of Agents](https://arxiv.org/abs/2610.17757)**  
   构建 TiGanEval 衡量 Agent 在不完整指令下的结果对齐 · Kaiming Liu … Yang Liu · arXiv 2610.17757 · 2026-10-13 · [解读](https://aisafetyhot.com/items/tiqqokxm0l09jwca81z2y6hcq)
12. **[Claim Framing as a Driver of LLM Sycophancy](https://arxiv.org/abs/2610.18159)**  
   在可验证事实题上测量主张表述如何驱动谄媚 · Jean Seo … Isabelle Augenstein · arXiv 2610.18159 · 2026-10-13 · [解读](https://aisafetyhot.com/items/xyft0klf8p7xqy6c647nm1h2g)
13. **[Pushback in a Haystack: Language Models Respond to Factual Errors Ambiguously and Ineffectively](https://arxiv.org/abs/2610.17703)**  
   评测模型对用户假陈述的含糊回推能否纠正信念 · Li Lucy … Yulia Tsvetkov · arXiv 2610.17703 · 2026-10-13 · [解读](https://aisafetyhot.com/items/p4yeh4cmjsinw26kxp1gpp3mn)
14. **[Jev-Guard: Fast Routing and Auditing Agent Actions over Editable Policy Trees](https://arxiv.org/abs/2610.18326)**  
   提出 Jev-Guard，沿可编辑策略树路由并审计智能体动作 · `Agent 安全` · Wenbin Hu … Yangqiu Song · arXiv 2610.18326 · 2026-10-13 · [解读](https://aisafetyhot.com/items/mv86fhx0igz7qw9d4166zk90z)
15. **[MemeTrace: A Multimodal LLM-Based Agent for Safety-Aware Meme Provenance Analysis](https://arxiv.org/abs/2610.19267)**  
   MemeTrace 是一个基于多模态 LLM 的智能体，可自动追溯新兴表情包的来源与潜在风险，弥补以往审核研究仅按单张图像判定安全与否、无法做溯源分析的不足。 · Bo Shao … Yang Zhang · arXiv 2610.19267 · 2026-10-13 · [解读](https://aisafetyhot.com/items/k2irhwqx10x1dsfj9rseqoao9)
16. **[The Illusion of Visual Tool-Use: A Causal Audit of Thinking with Images](https://arxiv.org/abs/2608.06270)**  
   因果审计视觉工具调用，分离观察贡献与动作诱发捷径 · Zhiheng Wang … Chaochao Lu · arXiv 2608.06270 · 2026-08-06 · [解读](https://aisafetyhot.com/items/a9qp927ixkjxm4tpebcmqd4m5)
17. **[Breadcrumbing Search Agents](https://arxiv.org/abs/2608.04565)**  
   提出权威链劫持与轨迹引导策略演化，劫持搜索 Agent 的证据链 · Xuebin Li … Nenghai Yu · arXiv 2608.04565 · 2026-08-05 · [解读](https://aisafetyhot.com/items/m2biqt47wpmthlld6i2nkgw8f)
18. **[The Obfuscation Atlas: Mapping Where Honesty Emerges in RLVR with Deception Probes](https://openreview.net/forum?id=wrGSN9kAVD)**  
   研究表明针对白盒欺骗探测器训练时模型会通过混淆内部表征或策略来规避检测，指出需足够强的KL正则化与探测器惩罚才能促使诚实策略涌现。 · `欺骗与谋划` · Mohammad Taufeeque … Chris Cundy · ICML 2026 spotlight
19. **[AdversarialCoT: Single-Document Retrieval Poisoning for LLM Reasoning](https://arxiv.org/abs/2604.12201)**  
   提出 AdversarialCoT 单文档检索投毒以操纵 RAG 推理答案 · Hongru Song … Xueqi Cheng · arXiv 2604.12201 · 2026-04-14 · [解读](https://aisafetyhot.com/items/n82e1w6zpyig9yjd3wb625tw1)
20. **[What Does a Sharing Question Add? Auditing LLM Survey Scores for Misinformation](https://arxiv.org/abs/2604.06820)**  
   审计 LLM 对误导文的分享问卷分是否超出可信度提供增量测量 · Zonghuan Xu … Xingjun Ma · arXiv 2604.06820 · 2026-04-08 · [解读](https://aisafetyhot.com/items/dvm6znzqoaufef57q1sqciqz9)
21. **[TraceSafe: A Systematic Assessment of LLM Guardrails on Multi-Step Tool-Calling Trajectories](https://arxiv.org/abs/2604.07223)**  
   提出 TRACE SAFE-BENCH，静态评测多步工具调用轨迹上的护栏 · Yen-Shan Chen … Yun-Nung Chen · arXiv 2604.07223 · 2026-04-08 · [解读](https://aisafetyhot.com/items/qe10ywrn3r5epnr4bscqk9xyv)
22. **[Uncovering Linguistic Fragility in Vision-Language-Action Models via Diversity-Aware Red Teaming](https://arxiv.org/abs/2604.05595)**  
   提出 DAERT，以仿真失败为奖励生成多样对抗指令，暴露 VLA 的语言脆弱性 · Baoshun Tong … Liang Lin · arXiv 2604.05595 · 2026-04-07 · [解读](https://aisafetyhot.com/items/biaqa7rf1rjf2m76yz5wo64hr)
23. **[From Poisoned to Aware: Fostering Backdoor Self-Awareness in LLMs](https://openreview.net/forum?id=lUVEQ1JRIL)**  
   用反演式强化学习让中毒模型自述其植入触发词，并据此提出缓解与检测两种防御，在五种后门攻击上优于六个基线。 · `后门与投毒` · Guangyu Shen … Xiangyu Zhang · ICML 2026 spotlight
24. **[GrandGuard: Taxonomy, Benchmark, and Safeguards for Elderly-Chatbot Interaction Safety](https://arxiv.org/abs/2605.20203)**  
   提出老年聊天安全分类与基准 GrandGuard 并评测回复与护栏 · Changxuan Fan … Yangqiu Song · arXiv 2605.20203 · 2026-04-07 · [解读](https://aisafetyhot.com/items/u30sgeqtw9vailnqov5o4yoy4)
25. **[BrokenMath: A Benchmark for Sycophancy in Theorem Proving with LLMs](https://openreview.net/forum?id=Y5bEI4cuMd)**  
   提出首个评测大模型在自然语言定理证明中谄媚行为的基准BrokenMath，发现主流前沿模型普遍会迎合用户的错误命题给出虚假证明，并测试了缓解策略。 · `对齐` · Ivo Petrov … Martin Vechev · ICML 2026 spotlight
26. **[Securing Multimodal AI through Internal Information Decomposition](https://openreview.net/forum?id=GEzZIUmEqE)**  
   提出推理期防御框架FlowGuard，利用部分信息分解监测跨模态内部一致性，仅用良性数据训练单类分类器即可将多模态未知攻击的成功率从90%以上降至15%以下。 · `防御与护栏` · Jehyeok Yeon … Heng Ji · ICML 2026 spotlight
27. **[The Art of Building Verifiers for Computer Use Agents](https://arxiv.org/abs/2604.06240)**  
   构建 Universal Verifier 核验计算机使用 Agent 轨迹 · Corby Rosset … Ahmed Awadallah · arXiv 2604.06240 · 2026-04-05 · [解读](https://aisafetyhot.com/items/ov7nyfl3e5d756mpvzgzb2djk)
28. **[Estimating Tail Risks in Language Model Output Distributions](https://openreview.net/forum?id=Joka19sTny)**  
   用构造不安全版本模型做重要性采样，估计有害输出概率，样本量比暴力蒙特卡洛少 10–20 倍，可预测部署风险。 · `红队测试与挑战赛` · Rico Angell … He He · ICML 2026 spotlight
29. **[Modular Pretraining Enables Access Control](https://openreview.net/forum?id=yIubI9l3IT)**  
   提出梯度路由辅助模块预训练方法GRAM，通过推理时消融特定模块移除病毒学与网络安全等高危能力，且比事后遗忘更具抗微调恢复性。 · `防御与护栏` · Ethan Roland … Alex Cloud · ICML 2026 spotlight · [解读](https://aisafetyhot.com/items/vvki9eetl42hlsy0wectawxgn)
30. **[Reliable Weak-to-Strong Monitoring of LLM Agents](https://openreview.net/forum?id=WV7xIboTDK)**  
   提出 monitor red teaming 流程，在 SHADE-Arena 上压测隐蔽不良行为监控；发现 agent 知晓被监控会显著削弱检测，混合式监控设计让弱监控者能监督强 agent。 · `监控与 AI 控制` · Neil Kale … Zifan Wang · ICLR 2026 Oral

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 4 · [Agent 安全](daily-papers/topics/agent-security.md) 4 · [后门与投毒](daily-papers/topics/backdoor.md) 3 · [对齐](daily-papers/topics/alignment.md) 2 · [欺骗与谋划](daily-papers/topics/scheming.md) 2 · [隐私与数据泄露](daily-papers/topics/privacy.md) 2 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 1 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 1 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 支持

觉得有用，欢迎点个 Star，或[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
