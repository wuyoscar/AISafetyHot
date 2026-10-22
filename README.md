<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>追踪 AI 安全新闻、论文与事件。一站阅读，也能接入你的 Agent。</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/zh"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-6-2ea44f" alt="6 Agent skills"></a>
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

连接 MCP，再安装技能，就可以直接用自然语言查动态、找研究线索、追踪实验室或事件。

**Claude Code** · 安装技能包与 MCP

```bash
/plugin marketplace add wuyoscar/AISafetyHot-Hub
/plugin install aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
npx skills add wuyoscar/AISafetyHot-Hub
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
```

**Cursor / 其他 Agent** · 用 `npx skills add wuyoscar/AISafetyHot-Hub` 安装支持的技能，再在客户端添加 MCP 地址 `https://aisafetyhot.com/api/mcp`，选择 Streamable HTTP。

近期 News 简报无需 API Key。历史查询与完整论文解读等需要只读授权，具体范围和接入方法见 [Agent 指南](docs/agent.md)；网站可直接阅读。

<a id="skills"></a>
<a id="技能"></a>

### 六个技能，按需要使用

| 技能 | 用途 | 可以这样问 |
| --- | --- | --- |
| [`aisafety-brief`](skills/aisafety-brief/SKILL.md) | 近期安全简报 | 这周 AI 安全有什么大事？ |
| [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) | 查找论文与引用线索 | 找 Agent 提示注入相关论文。 |
| [`aisafety-related-work`](skills/aisafety-related-work/SKILL.md) | 从研究问题整理相关工作 | 根据这份摘要，整理 reward hacking 的相关工作。 |
| [`aisafety-lab-watch`](skills/aisafety-lab-watch/SKILL.md) | 追踪一家实验室 | Anthropic 最近一周有哪些安全进展？ |
| [`aisafety-incident-check`](skills/aisafety-incident-check/SKILL.md) | 查找事件与漏洞报道 | Cursor 最近有哪些安全事件？ |
| [`aisafetyhot`](skills/aisafetyhot/SKILL.md) | MCP 工具与查询说明 | 查看工具、筛选和分页用法。 |

[查看调用示例](docs/mcp-examples.md)

## 每日论文与公开归档

[每日论文](daily-papers)从论文库中每天挑选 30 篇，跨日去重，兼顾近期研究与较早的重要工作；保留原始发表日期、原文和站内阅读链接。也可以按[研究方向](daily-papers/topics)浏览。

| 归档 | 内容 |
| --- | --- |
| [daily-papers](daily-papers) | 每日论文推荐与方向索引 |
| [daily](daily) · [English](en) | 已公开的日报归档 |
| [papers](papers) | 按日期导出的论文 Markdown、JSON 与 BibTeX |
| [archive](archive) | 年度索引 |

<!-- papers:start -->
### 2026-10-23 · 30 篇

1. **[Monitorability Is Trainable: Post-Training for Chain-of-Thought Monitorability](https://arxiv.org/abs/2610.29734)**  
   研究者提出一种无监督后训练目标，通过最大化思维链与模型输出之间的互信息来提升思维链可监控性。 · Usman Anwar … David Krueger · arXiv 2610.29734 · 2026-10-21 · [解读](https://aisafetyhot.com/items/j97xe5i3748k1mb3r73ztmvyv)
2. **[Automating ML for Science: Can Frontier Agents Climb Scientific Hills in the Wild?](https://huggingface.co/papers/2610.28763)**  
   面向科学的 ML 自动化：前沿 Agent 能否在真实环境中攀登科学高坡？ · Ming Zhong … Matthew Jagielski · arXiv 2610.28763 · 2026-10-20 · [解读](https://aisafetyhot.com/items/sqm3j08raxacsy5t0vzvrco60)
3. **[Unintended Side Effects of Value Training in LLMs](https://arxiv.org/abs/2610.29922)**  
   研究者在四个指令微调大语言模型上发现，针对特定价值维度的训练会对未训练的价值、风险偏好、社会认知和安全特性产生非预期副作用。 · Siddhesh Pawar … Isabelle Augenstein · arXiv 2610.29922 · 2026-10-21 · [解读](https://aisafetyhot.com/items/ctibwa9s4gsab886b8mkap69o)
4. **[ToM2Vec: Continuous Theory-of-Mind Tokens for Multi-Agent Coordination](https://huggingface.co/papers/2610.29934)**  
   研究者提出 ToM2Vec，用固定预算的连续推理 token 让 LLM 智能体学习抽象的伙伴心理状态表示，以改善多智能体协作。 · Nithin Sivakumaran … Elias Stengel-Eskin · arXiv 2610.29934 · 2026-10-21 · [解读](https://aisafetyhot.com/items/c0mvtfdr4zekrm4ykvem0sp9g)
5. **[CertMoE: Robustness Certification for Mixture-of-Experts LLMs via Routing-Aware Smoothing](https://arxiv.org/abs/2610.29395)**  
   论文提出 CertMoE，一个面向 MoE 大语言模型的路由感知鲁棒性认证框架，作者称这是首个在认证中显式考虑输入诱导路由动态的框架。 · Qingyue Wang … Shuai Wang · arXiv 2610.29395 · 2026-10-21 · [解读](https://aisafetyhot.com/items/mg5tdtxq74m0ytdjrq96xgesk)
6. **[Beyond Binary Labels: Diagnostic Evaluation of LLM Safety with Prompt-Level Rubrics](https://arxiv.org/abs/2610.29225)**  
   研究者提出 DiagSafe 诊断评测框架，用提示词级评分细则取代二元安全/不安全标签来评估 LLM 安全，细则基于全球适用的 AI 安全政策，从安全（针对具体危害并设豁免以抑制误报）和有用性（独立评估指令完成度）两个维度给出明确标准。 · Hongyu Li … Renfen Hu · arXiv 2610.29225 · 2026-10-21 · [解读](https://aisafetyhot.com/items/xpuplbsdbl5vml8g7d37rlsqu)
7. **[Building Auditable AI Text Detectors with Sparse Autoencoders](https://arxiv.org/abs/2610.30006)**  
   研究者提出一套流程，把微调的神经 AI 文本检测器改造成基于人类可读概念的分类器。 · Liam Dugan … Chris Callison-Burch · arXiv 2610.30006 · 2026-10-21 · [解读](https://aisafetyhot.com/items/pa4ytq5l29fnnaim6mkmjoyep)
8. **[Back Up Before You Regret: Measuring Backup Awareness and Automating Backup in Coding Agents](https://arxiv.org/abs/2610.28934)**  
   在后悔之前先备份：测量编码 Agent 的备份意识并自动化备份 · Xu Li … Weiyan Shi · arXiv 2610.28934 · 2026-10-20 · [解读](https://aisafetyhot.com/items/kv7tda8vo0aqk4ps8a5639mie)
9. **[Out-of-Distribution Detection in Continual Learning](https://arxiv.org/abs/2610.25901)**  
   提出 TA-KAN 与几何引导分数，检测无回放持续学习中的分布外样本 · Nimeshika Udayangani … Sarah Erfani · arXiv 2610.25901 · 2026-10-19 · [解读](https://aisafetyhot.com/items/ddn1ngmcm2hdfhro2k0062qjo)
10. **[Agent World Model in the Wild: Computer-Use Agent Environment Synthesis](https://huggingface.co/papers/2610.26828)**  
   研究者提出 WildAWM，一个完全由开源模型驱动的流水线，用于合成可控的计算机使用环境与任务，通过交互训练通用计算机使用 Agent（CUA），以避免直接在真实计算机系统上训练带来的安全风险。 · Zhaoyang Wang … Huaxiu Yao · arXiv 2610.26828 · 2026-10-19 · [解读](https://aisafetyhot.com/items/dkvtdsoale0qrjk5sh9ossdjg)
11. **[Physical AI: Concepts, Techniques, and Challenges](https://arxiv.org/abs/2610.27045)**  
   给出 physical AI 的闭环干预定义并整理技术版图与挑战 · Weinan Zhang … Bowen Zhou · arXiv 2610.27045 · 2026-10-19 · [解读](https://aisafetyhot.com/items/v4v44vugz73znc4l6vci0lhar)
12. **[AdLift: Lifting Adversarial Perturbations to Safeguard 3D Gaussian Splatting Assets Against Instruction-Driven Editing](https://openreview.net/forum?id=RL565ePGHR)**  
   提出 AdLift，将有界 2D 对抗扰动提升为 3D 高斯防护，通过 Lifted PGD 优化，跨任意视角有效且不可感知地防御指令驱动的 2D 与 3DGS 编辑。 · `防御与护栏` · Ziming Hong … Tongliang Liu · ICML 2026 spotlight
13. **[LLM Fingerprinting via Semantically Conditioned Watermarks](https://openreview.net/forum?id=t38nZqqi3Z)**  
   提出用语义域触发、弥散于回复中的统计水印替代固定查询-应答式指纹，隐蔽且能抵御微调、量化等常见部署操作，用于验证模型所有权。 · `开源模型与权重安全` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
14. **[Security--Fidelity Tradeoffs: The Hidden Cost of Prompt Injection Defense](https://openreview.net/forum?id=vTJmIhNvC3)**  
   提出SecFid基准区分执行、处理与忽略注入三种行为，在1168个样本和48种配置上没有模型或防御能同时兼顾安全与保真：最高保真96.5%时安全仅47.8%，最安全防御达99.3%安全但保真只有71.0%–73.9%。 · `提示注入` · Mitchell Hermon … Haohan Wang · ICML 2026 spotlight
15. **[Trojan-Speak: Bypassing Constitutional Classifiers with No Jailbreak Tax via Adversarial Finetuning](https://arxiv.org/abs/2603.29038)**  
   提出 Trojan-Speak，用编码微调绕过宪法分类器并保留能力 · Bilgehan Sel … Jerry Wei · arXiv 2603.29038 · 2026-03-30 · [解读](https://aisafetyhot.com/items/sug41b9edsf28aq2ynkeyfil2)
16. **[Differentially Private Sparse Reward Estimation with Preference Feedback](https://arxiv.org/abs/2610.30099)**  
   针对 RLHF 依赖敏感偏好数据、存在用户信息泄露风险的问题，论文研究差分隐私稀疏奖励估计，作者称给出了 Bradley-Terry-Luce 模型下从成对偏好反馈进行此类估计的首个综合理论框架，并为 Sample-DP 与 Label-DP 两种设置设计高效算法。 · Meng Ding … Di Wang · arXiv 2610.30099 · 2026-10-21 · [解读](https://aisafetyhot.com/items/avikxx747ses83u2fqr2goj9i)
17. **[Memory-Centric Continual Learning for AI Agents](https://huggingface.co/papers/2610.29357)**  
   记忆中心持续学习（MCCL）主张以能否改进未来行为、而非仅能否检索来评判智能体记忆，把被动缓存变为行为改进的主动驱动。 · Dongfang Li … Min Zhang · arXiv 2610.29357 · 2026-10-21 · [解读](https://aisafetyhot.com/items/wrr22oza0shpgl34qvdasoqk8)
18. **[WRDO: Weighted Refusal Direction Optimization in Aligned Language Models](https://arxiv.org/abs/2610.29555)**  
   研究者提出 WRDO（加权拒绝方向优化），通过学习到的聚合权重把多个按提示词计算的拒绝方向合成为复合方向，用于对齐大语言模型的拒答干预。 · Grigoriy Evseev … Aleksandr Beznosikov · arXiv 2610.29555 · 2026-10-21 · [解读](https://aisafetyhot.com/items/ocx60g1uzsqp68it48qdchxcu)
19. **[RubricOpt: Self-Revision of Semantic Rubrics for Preference Optimization](https://arxiv.org/abs/2610.29491)**  
   RubricOpt 让策略在偏好优化中自我修订语义评分标准，并用确定性门控核验证据引用与固定语义锚点。策略诊断无评分标准输出，保留已覆盖要求并修改未解决反复失败的条款。 · Wei Chen … Zhou Wang · arXiv 2610.29491 · 2026-10-21 · [解读](https://aisafetyhot.com/items/pidxf3pkhpyws43y557w33tp0)
20. **[Characterizing and Defending Utility-Hijacking in Instruction-Tuning Data Selection](https://arxiv.org/abs/2610.29886)**  
   中山大学与华为的研究者提出针对指令微调数据选择器的效用劫持（utility-hijacking）投毒攻击，并给出无需内容检测器或投毒标签的防御 CONCERT。 · Yahao Ren … Jiawei Duan · arXiv 2610.29886 · 2026-10-21 · [解读](https://aisafetyhot.com/items/ul4mo8svawyf1hbxqy3zu7gj3)
21. **[Situating Vulnerability: An Ethical Governance Framework for Anthropomorphic AI Interaction](https://arxiv.org/abs/2610.29304)**  
   针对大语言模型拟人化交互带来的风险，论文提出以“脆弱性情境”取代“脆弱群体”作为伦理治理单元。 · Hanhui Xu … Mengyue Wu · arXiv 2610.29304 · 2026-10-21 · [解读](https://aisafetyhot.com/items/swz2qstrgte5pyrurku7b7ebr)
22. **[Evolving with Open Worlds: Towards Recursive Self-Improvement for Future Forecasting](https://huggingface.co/papers/2610.29784)**  
   与开放世界共同演化：迈向未来预测的递归自我改进 · Zhipeng Chen … Wayne Xin Zhao · arXiv 2610.29784 · 2026-10-21 · [解读](https://aisafetyhot.com/items/urx2vabfeb5fo34t6uli06q6t)
23. **[Mitigating Reward Hacking in Realistic Scenarios Through Representation Engineering](https://arxiv.org/abs/2610.29129)**  
   研究者研究在工具调用、长上下文等真实场景中监测和缓解奖励作弊，对三种方法得到的 Steering direction 施加动态干预。 · Austin Meek … Steven Basart · arXiv 2610.29129 · 2026-10-21 · [解读](https://aisafetyhot.com/items/vetciiqv27xk28a7i9nlyd6rd)
24. **[Multimodal Embodied Agents: A Unified Capability-centric Perspective from Computer-Use to Robot-Use](https://huggingface.co/papers/2610.30108)**  
   PAPAV 框架将多模态具身智能体的核心能力归纳为感知、预期、规划、执行、验证五项，据此比较计算机使用与机器人使用场景的差异。 · Yanzhe Chen … Mike Zheng Shou · arXiv 2610.30108 · 2026-10-21 · [解读](https://aisafetyhot.com/items/aq782ihfquzkus7kba29hqp78)
25. **[Proof-Carrying Contracts: Commitments AI Agents Cannot Break](https://arxiv.org/abs/2610.28484)**  
   论文提出 Proof-Carrying Contracts（PC2）框架，要求智能体在请求执行操作前提交机器可检验证明，由 Airlock 执行系统核验证明并控制操作入口。证明需表明该操作在模型允许的情形中保持约定约束。 · Carlo Ciliberto … Enrico Tassi · arXiv 2610.28484 · 2026-10-20 · [解读](https://aisafetyhot.com/items/q6uwud7ss4034ty4xb46vpouq)
26. **[NetGuise: Adversarial Traffic Generation for Early-Stage Classifier Evasion](https://arxiv.org/abs/2610.27456)**  
   提出 NetGuise，在包级整形约束下定向规避早阶段流量分类器 · Binghui Wu … Mohan Gurusamy · arXiv 2610.27456 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ni3vu8bor5g4877nnickmz2hs)
27. **[Act on Your Behalf, Beyond Your Authorization: Benchmarking LLM Agent Authorization Alignment](https://arxiv.org/abs/2610.27548)**  
   提出 AUTHORIZATION BENCH，评测 Agent 是否越出授权范围 · `Agent 安全` · Zhiping Zhang … Tianshi Li · arXiv 2610.27548 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ir5vlj7aettc0527ng2bz6bxg)
28. **[LIFT: Scoped Constraints for Evaluating and Training Instruction Following](https://arxiv.org/abs/2610.28819)**  
   研究者提出 Lift-Bench 指令遵循基准，要求模型根据给定主题和结构化大纲起草文档，约束限定在特定文档章节，包含可验证与评判式两类约束，并配有训练集 Lift-Train。 · Eran Goldstein … Daniel Gissin · arXiv 2610.28819 · 2026-10-20 · [解读](https://aisafetyhot.com/items/f9su4xtqmxrixo7i2kru887xm)
29. **[MMEnterprise-Bench: Evaluating Enterprise Agents over Evolving Multimodal Records](https://huggingface.co/papers/2610.27911)**  
   提出 MMEnterprise-Bench 评测企业智能体在演化多模态记录上的问答 · Seohyun Lee … Hyunwoo J. Kim · arXiv 2610.27911 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ajbd013lursuu0prc5l03zed6)
30. **[RSI Control: Can AI Models Perform Covert Sabotage in the Self-Improvement Process?](https://arxiv.org/abs/2610.27735)**  
   提出 RSI Control Arena，评测自我改进中的隐蔽破坏与监控检出 · Kaiwen Zhou, Udari Madhushani Sehwag · arXiv 2610.27735 · 2026-10-20 · [解读](https://aisafetyhot.com/items/xecv3hoxtsd5djmvm5fvaqr8q)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 22 · [Agent 安全](daily-papers/topics/agent-security.md) 15 · [后门与投毒](daily-papers/topics/backdoor.md) 9 · [隐私与数据泄露](daily-papers/topics/privacy.md) 6 · [越狱与攻击](daily-papers/topics/jailbreak.md) 6 · [奖励作弊](daily-papers/topics/reward-hacking.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [开源模型与权重安全](daily-papers/topics/open-models.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1 · [提示注入](daily-papers/topics/prompt-injection.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
