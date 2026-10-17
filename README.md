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
### 2026-10-18 · 30 篇

1. **[LEASH: Uncertainty-Aware Weak-to-Strong Escalation and Oversight for Computer-Use Agents](https://huggingface.co/papers/2610.22280)**  
   提出 LEASH，用弱模型隐藏状态不确定性驱动计算机使用智能体的升级与影子监督 · Qingni Wang … Xin Eric Wang · arXiv 2610.22280 · 2026-10-16 · [解读](https://aisafetyhot.com/items/c86ia3ao12xaapny3vis7ds0m)
2. **[Recursive Reward Improvement via Adversarial Meta-Prompt Evolution](https://arxiv.org/abs/2610.21040)**  
   提出 RRI，对抗检验并修补自写评分准则后再训练求解器 · Wei Dai … Sheng Zhang · arXiv 2610.21040 · 2026-10-15 · [解读](https://aisafetyhot.com/items/n6wdmvhs2xvygirkmzie7lws2)
3. **[Salesforce 等提出 A2-Failures：跨委托人 Agent 协作的 20 种失效模式，Agent 从不主动核实对方](https://arxiv.org/abs/2610.19342)**  
   提出 A2-Failures 分类法，刻画跨委托人 Agent 协作的失效模式 · `Agent 安全` · Sarath Shekkizhar … Shafiq Joty · arXiv 2610.19342 · 2026-10-14 · [解读](https://aisafetyhot.com/items/o8dsfdudrd4zonj0udj7t11py)
4. **[Learning to Read Out: Unembedding Dynamics in Language Model Pretraining](https://huggingface.co/papers/2610.21025)**  
   用参数轨迹 crosscoding 分开编码与 readout 表达 · Matteo He … Nicholas D. Lane · arXiv 2610.21025 · 2026-10-14 · [解读](https://aisafetyhot.com/items/wfybqdgs41hwt8kpj00uhdnrs)
5. **[论文：越狱评测的裁判模型一换](https://arxiv.org/abs/2610.19306)**  
   提出语义重建博弈，校正越狱评测的裁判误判 · Liam Davis … Suman Jana · arXiv 2610.19306 · 2026-10-13 · [解读](https://aisafetyhot.com/items/h6xvr7oroc52wcroeqgdww4bj)
6. **[Debate Training Reduces Reward Hacking in RLAIF](https://arxiv.org/abs/2608.17776)**  
   提出常和辩论训练，减轻弱评审下 RLAIF 的奖励作弊 · Zachary Kenton … Rohin Shah · arXiv 2608.17776 · 2026-08-18 · [解读](https://aisafetyhot.com/items/owmw1gy0d1so69sr02ruk9v6m)
7. **[KeyPooling: Measuring Where LLM API Relay Paths Collapse Prompt Cache Isolation](https://arxiv.org/abs/2608.17485)**  
   提出 KeyPooling，测量 API 中继何处瓦解提示缓存隔离 · Bowen Sun … Chaowei Xiao · arXiv 2608.17485 · 2026-08-18 · [解读](https://aisafetyhot.com/items/anp3xwwht2jptor8j4oucgdfl)
8. **[Decomposition Attacks Across Unlinkable Identities: Limits of Stateful Defenses for LLM Services](https://arxiv.org/abs/2608.17445)**  
   形式化跨不可关联身份的分解攻击并评测状态化防御边界 · Bowen Sun … Chaowei Xiao · arXiv 2608.17445 · 2026-08-18 · [解读](https://aisafetyhot.com/items/dcf4v10k77aub88bsb3wvs817)
9. **[On the Fragility of Self-Improving Agents: Variance, Task Order, and Underspecification](https://arxiv.org/abs/2608.18066)**  
   重测记忆型自改进 Agent 的运行方差与任务顺序敏感性 · Qinyuan Ye … Chien-Sheng Wu · arXiv 2608.18066 · 2026-08-18 · [解读](https://aisafetyhot.com/items/juov4akm386odvmbzar5yw86u)
10. **[Hidden in Plain Sight: Diffusion-Based Unrestricted Robotic Attacks on Vision-Language-Action Models](https://arxiv.org/abs/2608.10393)**  
   提出 DURA，用扩散模型生成自然对抗补丁操控 VLA 机器人动作 · Jiahui Han … Xia Hu · arXiv 2608.10393 · 2026-08-11 · [解读](https://aisafetyhot.com/items/x05drznkr9p3m10wpe0g7hl4d)
11. **[Leave My Images Alone: Preventing Multi-Modal Large Language Models from Analyzing Images via Visual Prompt Injection](https://aclanthology.org/2026.acl-long.72/)**  
   提出 ImageProtector,在图像中嵌入近乎不可见的扰动使 MLLM 拒答,在六个模型和四个数据集上有效,对部分对策仍具抵抗力。 · `隐私与数据泄露` · Zedian Shao … Neil Zhenqiang Gong · ACL 2026 long
12. **[PROBE: Learning to Audit Policy Compliance in Tool-Using LLM Agents](https://arxiv.org/abs/2610.22124)**  
   提出 PROBE，训练审计器探测工具 Agent 的策略违规 · Kshitij Mishra … Salem Lahlou · arXiv 2610.22124 · 2026-10-15 · [解读](https://aisafetyhot.com/items/bw6qv28qrpm7cxbzbe10eyymy)
13. **[FIRM: Fisher-Informed Retention Merging for Federated LLM Unlearning](https://arxiv.org/abs/2610.21720)**  
   提出联邦 LLM 遗忘方法 FIRM，用 Fisher 合并在不见数据时删除目标知识并维持效用 · Reeyansh Shah … Biplab Banerjee · arXiv 2610.21720 · 2026-10-15 · [解读](https://aisafetyhot.com/items/mgi2k9s41z1d6takfqu8awy8g)
14. **[In the Guise of Correction: How Framing and Cultural Adaptation Erode LLM Safety on Real-World Criminal Cases](https://arxiv.org/abs/2610.21789)**  
   构建 GUISE 基准，评测纠错表述与文化适配对犯罪协助拒答的削弱 · Mohsinul Kabir … Sophia Ananiadou · arXiv 2610.21789 · 2026-10-15 · [解读](https://aisafetyhot.com/items/hdgtfxlxf7vu8vm7mk6orfjxu)
15. **[CAT-alyzing Honesty: Continuous Adversarial Training for Transferable LLM Honesty](https://arxiv.org/abs/2610.22292)**  
   提出 CATCH，用连续对抗训练提升模型在压力下的诚实性 · Yuan-Chen Chang … Tommaso Tosato · arXiv 2610.22292 · 2026-10-15 · [解读](https://aisafetyhot.com/items/yhulqgi1hy8i9r96r6xq30hgp)
16. **[BiShield-TEE: On the (In-)Security of Unilateral Weight Obfuscation in On-Device TEE-Shielded LLM Partition](https://arxiv.org/abs/2610.21565)**  
   提出双侧混淆框架 BiShield-TEE，使端侧权重密钥恢复不再唯一 · Zhiyuan Wang … Yongheng Deng · arXiv 2610.21565 · 2026-10-15 · [解读](https://aisafetyhot.com/items/bjk706rjvh9s8s8n760thd7ip)
17. **[When Reasoning Is Not Enough: Proactive Inquiry for Cross-Modal Safety in Multimodal Large Language Models](https://arxiv.org/abs/2610.22068)**  
   提出 SAFE-PRO，以风险条件不确定性调度跨模态安全的主动澄清与路径优化 · `防御与护栏` · Wei Cai … Xuelong Li · arXiv 2610.22068 · 2026-10-15 · [解读](https://aisafetyhot.com/items/l63s1pb0o8n9x5cc49g697335)
18. **[Terminal-RSI: Recursive Self-Improving Terminal Agents via Recursive Self-Rewrite and Policy-Refine](https://huggingface.co/papers/2610.22192)**  
   提出 Terminal-RSI，用递归自我重写与策略精炼训练终端智能体 · Junyao Yang … Leowei Liang · arXiv 2610.22192 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ahtbz16ewfwa7yqpp9xznfxw4)
19. **[Selection Is Not Learning: Choosing Model Futures](https://arxiv.org/abs/2610.22029)**  
   提出 EVOHEIR，用新探针筛选自演化模型是否继承更新 · Haoyi Yang … Salem Lahlou · arXiv 2610.22029 · 2026-10-15 · [解读](https://aisafetyhot.com/items/jizdtiebeownlta9rwqy3iwuv)
20. **[Private Retrieval Augmented Generation via Random Projection](https://arxiv.org/abs/2610.22297)**  
   提出随机投影，降低 RAG 检索库敏感信息被提取的风险 · Dixi Yao … Tian Li · arXiv 2610.22297 · 2026-10-15 · [解读](https://aisafetyhot.com/items/i8e6fdwq0cusbqd19m9zzu2ry)
21. **[VALCON: Benchmarking and Enhancing Value Consistency in Large Language Models via Dual-Role Variation](https://arxiv.org/abs/2610.21304)**  
   提出 VALCON 双角色基准，评测大语言模型的价值一致性 · Junru Wu … Deyi Xiong · arXiv 2610.21304 · 2026-10-15 · [解读](https://aisafetyhot.com/items/m6qumkkc6jgco6j47h80osfly)
22. **[论文：LLM 智能体委托规模与问责的多中心治理困境](https://arxiv.org/abs/2610.21746)**  
   提出自愿委托与退出问责的博弈，并用智能体模拟多中心治理 · Arin Mukhopadhyay … Panayiotis Danassis · arXiv 2610.21746 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ubsj5b20a2fc9aippve4zgx80)
23. **[One Bias Score, Two Factors: How Mitigations Affect Option Bias in Multiple-Choice Evaluation](https://huggingface.co/papers/2610.20993)**  
   分解选择题汇合偏差为翻转率与位置偏斜，比较缓解措施各改何种行为 · Hyunjong Ok … Jaeho Lee · arXiv 2610.20993 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ha5bbugbo30ekcc81nvu46pnx)
24. **[CoRedSkill: Stealthy Skill Composition Attacks via AST-Guided Injection](https://arxiv.org/abs/2610.20049)**  
   提出 COREDSKILL，用 AST 重写把攻击链拆入多技能并规避审计 · Qichen Zhao … Jiaheng Zhang · arXiv 2610.20049 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ycc6i10uiqv3vqedgv65o9dee)
25. **[Counterfactual Neighborhood Risk Fields: Evidence-Grounded Selective Safety for Vision-Language Models](https://arxiv.org/abs/2610.20679)**  
   提出 CNRF，用反事实邻域证据对视觉语言模型做选择性防御 · `防御与护栏` · Tianshi Wang … Lei Zhu · arXiv 2610.20679 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dvuk045xsun0xt6nnbuh5tzpg)
26. **[INFUSE: A Unified Surface Benchmark for Indirect Prompt Injection in Agentic Systems](https://arxiv.org/abs/2610.20776)**  
   提出 INFUSE 基准评测终端 Agent 的间接提示注入 · Thuy Dung Nguyen … Kevin Leach · arXiv 2610.20776 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ycapq3ognwok1og5t9537o8pe)
27. **[Reading Right, Acting Wrong: Diagnosing Decision Failures of System One Models in Agent Loops](https://huggingface.co/papers/2610.18579)**  
   诊断 Agent 循环中 System One 模型读对却做错的决策失败 · Yubo Li … Rema Padman · arXiv 2610.18579 · 2026-10-13 · [解读](https://aisafetyhot.com/items/emo6gfjcc0jmtqvqpwg0wrrpo)
28. **[SWE-MISBEHAVIOR: Benchmarking and Mitigating Boundary Violations in Software Coding Agents](https://huggingface.co/papers/2610.18206)**  
   论文提出 SWE-MISBEHAVIOR，一个用于诊断编码 Agent 边界违规行为的分类与评测框架，并称其为该方向首个框架。 · Do Xuan Trong … Min-Yen Kan · arXiv 2610.18206 · 2026-10-13 · [解读](https://aisafetyhot.com/items/ec992h64qowmkachnfebrg5jn)
29. **[Are We Testing Too Much? A Survey of Benchmark Compression for Efficient Evaluation of Large Language Models](https://huggingface.co/papers/2610.18248)**  
   综述 LLM 基准压缩方法及其覆盖与可靠性风险 · Guoming Ling … Liang Lin · arXiv 2610.18248 · 2026-10-13 · [解读](https://aisafetyhot.com/items/p7f1a3fst79gjswk65k6e08di)
30. **[Evidence-First Agentic Verification](https://arxiv.org/abs/2610.17724)**  
   提出证据优先的 Agent 验证器 Sauron，核验状态与轨迹后判定准则 · Reza Sanayei … Daniel Yue Zhang · arXiv 2610.17724 · 2026-10-13 · [解读](https://aisafetyhot.com/items/vk62d6tzcfn8nittpvqw3a1sq)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 14 · [Agent 安全](daily-papers/topics/agent-security.md) 6 · [后门与投毒](daily-papers/topics/backdoor.md) 5 · [隐私与数据泄露](daily-papers/topics/privacy.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [奖励作弊](daily-papers/topics/reward-hacking.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 2 · [越狱与攻击](daily-papers/topics/jailbreak.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 支持

觉得有用，欢迎点个 Star，或[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
