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
### 2026-10-17 · 30 篇

1. **[Can Capability Enhancement be Localized?](https://arxiv.org/abs/2610.21294)**  
   提出能力增强定位，用两阶段搜索找出删头即可提升任务的稀疏注意力头 · Anh Tuan Nguyen … Zico Kolter · arXiv 2610.21294 · 2026-10-15 · [解读](https://aisafetyhot.com/items/k3ztzw5mgwhzry4dr8zc9eixx)
2. **[Screwtape: Adversarial Transcript Editing for Monitor Red-Teaming](https://arxiv.org/abs/2610.20941)**  
   Redwood Research 研究者提出 Screwtape 流水线，通过改写真实 Agent 对话记录来对只看动作的监控器做红队测试。攻击者由 LLM 编辑对话记录，使 Agent 造成指定危害并反复修改，直到监控器不再标记。 · Gosha Kozhevnikov, Tyler Tracy · arXiv 2610.20941 · 2026-10-14 · [解读](https://aisafetyhot.com/items/f2splfuxjd7l6nuru9fhc76gp)
3. **[A team of Gemini 4 Argon agents beats Minecraft](https://huggingface.co/papers/2610.22319)**  
   展示通用编程智能体团队自主协作通关 Minecraft · Maxence Faldor … Roberta Raileanu · arXiv 2610.22319 · 2026-10-15 · [解读](https://aisafetyhot.com/items/s7ttl80f3815t4zgjhyvmvvro)
4. **[Explaining the Roles of Experts in Mixture-of-Experts LLMs for Personalization](https://huggingface.co/papers/2610.22127)**  
   用两阶段微调与 crosscoder 解析 MoE 专家的个性化路由 · Sekh Mainul Islam … Isabelle Augenstein · arXiv 2610.22127 · 2026-10-15 · [解读](https://aisafetyhot.com/items/fyjbfho534ccso6r5zq258yiu)
5. **[JevAgentHarness: Benchmarking, Deploying and Training Decision Models That Share Control with LLMs](https://huggingface.co/papers/2610.21412)**  
   用 JevAgentHarness 评测并训练与 LLM 共享控制的决策模型 · Kunlun Zhu … Heng Ji · arXiv 2610.21412 · 2026-10-15 · [解读](https://aisafetyhot.com/items/k37rzf8a0agz24tzkxh32wcj5)
6. **[CarryOn: A Dual-Loop Harness for Personalized and Reliable Robot Assistance](https://huggingface.co/papers/2610.21453)**  
   提出 CarryOn 双环框架，为冻结 VLA 做个性化规划与危险接触防护 · Zixuan Wang … Jiaya Jia · arXiv 2610.21453 · 2026-10-15 · [解读](https://aisafetyhot.com/items/nl5ocpwxx1lqtnlizbn3hpncg)
7. **[Resisting Harmful Instructions through Training-Free Weight Editing](https://arxiv.org/abs/2610.21189)**  
   提出免训练权重编辑，降低模型对指定不良指令的遵从 · `防御与护栏` · Ali Ebrahimpour-Boroojeny … ChengXiang Zhai · arXiv 2610.21189 · 2026-10-15 · [解读](https://aisafetyhot.com/items/s8ncf672tvvvi7j4dbeh1nqm0)
8. **[Learning Self-Orchestration in Decentralized Agent Swarms](https://huggingface.co/papers/2610.22322)**  
   提出 MPT，让去中心化 Agent 群体同时学会行动与自我编排 · Guowei Xu … Yilun Du · arXiv 2610.22322 · 2026-10-15 · [解读](https://aisafetyhot.com/items/jrrnu8ues39ytuaseypkua19n)
9. **[Multi-Reward Hacking: From Aggregation-Induced Drift to Trust-Anchored Defense](https://arxiv.org/abs/2610.21404)**  
   提出信任锚定门控 TAG，缓解多奖励投机引起的策略漂移 · `奖励作弊` · Yushu Li … Youngsuk Park · arXiv 2610.21404 · 2026-10-15 · [解读](https://aisafetyhot.com/items/dez0weqpvh7wav82u5cymrhk5)
10. **[SCARCE: Emergent Institutions in Long-Horizon Multi-Agent Coding Systems](https://arxiv.org/abs/2610.21029)**  
   研究者提出 SCARCE 框架，让多个编码智能体在长周期任务中反复协商对单一共享执行资源的访问，发现智能体会自发形成以声誉、互惠和先例为基础的持久规则，作者称之为制度行为。 · Abhinav Kumar … Sahar Abdelnabi · arXiv 2610.21029 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ie3p39yx4u40tk6wl0mkm9w0y)
11. **[A Phenomenology of Neural Geometry in Vision-Language-Action Models](https://arxiv.org/abs/2610.20840)**  
   用扫描和激活干预刻画 VLA 控制概念的实现几何 · Mozes Jacobs … Thomas Fel · arXiv 2610.20840 · 2026-10-14 · [解读](https://aisafetyhot.com/items/mpsxc1vl8apx1ac5abz2xefi8)
12. **[MAI-Gym: An Open All-in-One Platform for GUI Agent Evaluation and RL Training across Mobile and Computer Environments](https://huggingface.co/papers/2610.20939)**  
   阿里 MAI-UI 团队发布 MAI-Gym，一个覆盖移动、电脑与网页环境的 GUI Agent 评测与在线 RL 训练开源平台，并用它训练出统一 9B 模型 MAI-Gym-9B。 · Panrong Tong … Steven Hoi · arXiv 2610.20939 · 2026-10-14 · [解读](https://aisafetyhot.com/items/q8vx59ti88vfdnlucg0v6mtod)
13. **[StepSafe: Learning Timely Intervention with Context-Aware Safety Reasoning](https://arxiv.org/abs/2610.20960)**  
   用 ASPO 训练步级护栏，在智能体动作执行前及时干预 · `Agent 安全` · Siyi Gu … Arman Cohan · arXiv 2610.20960 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dk33qgs4xq8rrphdz7fip26ye)
14. **[GEO-Flag: Detecting and Measuring GEO-Optimized Web Content](https://arxiv.org/abs/2608.16824)**  
   提出 GEOFlagBench 与 IPT，检测并测量生成式引擎优化网页 · Junjie Chu … Yang Zhang · arXiv 2608.16824 · 2026-08-17 · [解读](https://aisafetyhot.com/items/hicxebr3g3zihpfzec8241h9z)
15. **[Physics of Agents: Statistical Mechanics Predicts Collective Behavior of AI Agents](https://arxiv.org/abs/2608.16578)**  
   用 Ising 式耦合规则预测语言模型智能体的集体意见演化 · Batu El … James Zou · arXiv 2608.16578 · 2026-08-17 · [解读](https://aisafetyhot.com/items/yzv5ysxofep6027m0y6bxx4ot)
16. **[How Can Rhetoric Reward-Hack AI Reviewers? Dissecting Rhetorical Sensitivity in AI-Based Peer Review](https://arxiv.org/abs/2608.08975)**  
   测量内容保留的修辞改写如何改变 AI 审稿分数 · `奖励作弊` · Ming Li … Tianyi Zhou · arXiv 2608.08975 · 2026-08-10 · [解读](https://aisafetyhot.com/items/jytib083944kip9mmvts3vcjf)
17. **[Removing Sandbagging in LLMs by Training with Weak Supervision](https://openreview.net/forum?id=J4DiM8EiMJ)**  
   SFT 与 RL 结合可在弱监督下引出 sandbagging 模型的真实能力,单独使用均不可靠;但若模型能区分训练与部署,仍会继续藏拙。 · `监控与 AI 控制` · Emil Ryd … Vivek Hebbar · ICML 2026 regular
18. **[SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety](https://openreview.net/forum?id=PJdw4VBsXD)**  
   基于安全对齐目标的闭式最优解，提出仅需一个额外超参数的轻量级安全训练方法SafeDPO，无需奖励模型即可在PKU-SafeRLHF基准上显著提升模型安全性。 · `防御与护栏` · Geon-Hyeong Kim … Moontae Lee · ICLR 2026 Oral
19. **[Mitigating Reward Hacking in RLHF via Bayesian Non-negative Reward Modeling](https://openreview.net/forum?id=DfhMMHXDuu)**  
   提出 BNRM，将非负因子分析融入 Bradley–Terry 模型，以稀疏潜因子抑制长度等偏差，缓解奖励过优化并增强分布偏移下的鲁棒性。 · `奖励作弊` · Zhibin Duan … Dandan Guo · ICML 2026 spotlight
20. **[Toward Stable Value Alignment: Introducing Independent Modules for Consistent Value Guidance](https://openreview.net/forum?id=R80JLmXXPJ)**  
   针对模型残差流中价值表征脆弱动态的问题，提出SVGT架构，通过独立的规范价值空间建模与显式行为引导Token，在保持生成流畅的同时降低超70%的有害得分。 · `对齐` · Wenhao Chen … Guojie Song · ICML 2026 spotlight
21. **[Red-Teaming NSFW Image Classifiers as Text-to-Image Safeguards](https://aclanthology.org/2026.findings-acl.506/)**  
   提出自动化红队框架，发现良性画面元素的变化可导致NSFW漏检，利用失败案例训练的提示改写模型将检测规避概率提高至多六倍。 · `红队测试与挑战赛` · Tinghao Xie … Li Chen · ACL 2026 findings
22. **[Does a Hybrid Space-Aware Randomized Defense Improve Empirical and Certified Adversarial Robustness?](https://openreview.net/forum?id=Alelgxnwgs)**  
   提出 HySCAN，在权重与特征空间同时注入随机性，认证鲁棒性最多提升约 9.6%，经验鲁棒性提升约 5%，且不降低干净准确率。 · `防御与护栏` · Joy Dhar … Pietro Lio · ICML 2026 regular
23. **[Rubric Judgments Lack Uncertainty: Conformal Weighting for LLM Evaluation](https://arxiv.org/abs/2610.21214)**  
   提出 URW，用释义模板与共形 p 值加权 rubric 判断 · Licheng Pan … Kui Ren · arXiv 2610.21214 · 2026-10-15 · [解读](https://aisafetyhot.com/items/kp0awqcdmkn3s4l20j626gy9l)
24. **[MLExpert: Towards a Generalist Agentic Model for Autonomous Machine Learning Engineering](https://huggingface.co/papers/2610.22344)**  
   提出 WIRL 与分层智能体微调，后训练自主机器学习工程模型 · Shangheng Du … Bo Zhang · arXiv 2610.22344 · 2026-10-15 · [解读](https://aisafetyhot.com/items/dqbm2tgz5yzv12kd1xlcnw6zu)
25. **[From Perception to Prediction and Intervention: Benchmarking Proactive Video Assistants in Real-Life Scenarios](https://arxiv.org/abs/2610.21568)**  
   提出 P3IBench 评测主动式视频助手的感知、预测与干预 · Boyu Cui … Zhongyu Wei · arXiv 2610.21568 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ceocbp3544nsw2l31z4577ku8)
26. **[FusionAudit: Pathway-Conditioned Robustness Auditing for Native Multimodal Models](https://arxiv.org/abs/2610.21667)**  
   提出 FusionAudit 双通路审计，只改图像翻转多模态问答答案 · Jiaming Zhang … Wei Yang Bryan Lim · arXiv 2610.21667 · 2026-10-15 · [解读](https://aisafetyhot.com/items/e56rjgbjkjll370dwls5nu0f7)
27. **[OpenGCUA: Toward a Fully Open Stack for Generalist Computer Use](https://huggingface.co/papers/2610.22200)**  
   提出 OpenGCUA，让模型自行决定计算机使用的观察、行动与组织方式 · Hanzhang Zhou … Yue Wang · arXiv 2610.22200 · 2026-10-15 · [解读](https://aisafetyhot.com/items/w6nt9seo88wj9e2rh6d9b1ncy)
28. **[Clean Data Can Still Carry Backdoors: Support-Persistent Backdoors for Model Reuse](https://arxiv.org/abs/2610.21208)**  
   提出 DAR 支撑持久后门，使干净蒸馏后的学生仍可被触发 · `后门与投毒` · Junhoo Lee … Nojun Kwak · arXiv 2610.21208 · 2026-10-15 · [解读](https://aisafetyhot.com/items/xj6g2176eqwed1j78j7yy7yjc)
29. **[DialFork: Going Beyond Factuality to Evaluate Procedural Hallucination in Conversational Agents](https://arxiv.org/abs/2610.21561)**  
   发布 DIALFORK，评测对话智能体的流程幻觉 · Sergio Burdisso … Petr Motlicek · arXiv 2610.21561 · 2026-10-15 · [解读](https://aisafetyhot.com/items/f7gkbkicrzd30j2mlza43a6e4)
30. **[MAppPrint: Robust and Real-time Mobile App Fingerprinting via Traffic Behavior Correlation Graphs](https://arxiv.org/abs/2610.22148)**  
   提出 MAppPrint，用流量行为关联图从加密流量识别移动应用 · Tao Duan … Haibo Hu · arXiv 2610.22148 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ihgy0aqvcz1bmcvru2gvgslai)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 12 · [后门与投毒](daily-papers/topics/backdoor.md) 5 · [Agent 安全](daily-papers/topics/agent-security.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [隐私与数据泄露](daily-papers/topics/privacy.md) 4 · [奖励作弊](daily-papers/topics/reward-hacking.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 2 · [越狱与攻击](daily-papers/topics/jailbreak.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 支持

觉得有用，欢迎点个 Star，或[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
