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
### 2026-10-20 · 30 篇

1. **[Behavioral Couplings: From Formation to Behavioral Emergence in Language Models](https://arxiv.org/abs/2610.23847)**  
   检验文档共现训练能否形成行为耦合并诱发未训练失齐行为 · Dongyoon Hahm … Kimin Lee · arXiv 2610.23847 · 2026-10-16 · [解读](https://aisafetyhot.com/items/m78i4nc8zk2tl80yzhqt2vik1)
2. **[GatewayBench: Unified Capability and Security Evaluation Platform for MCP Gateways](https://arxiv.org/abs/2610.23449)**  
   用 GATEWAYBENCH 评测 MCP 网关的任务完成、开销与抗注入能力 · Yitian Zheng … Bo Li · arXiv 2610.23449 · 2026-10-16 · [解读](https://aisafetyhot.com/items/v1k6knr2ktrjiahaj17irwi1t)
3. **[Many Biases, One Circuit: Post-Training Tunes a Pretrained Cue-Routing Mechanism](https://arxiv.org/abs/2610.22937)**  
   用因果干预追踪多种提示偏置共享的预训练线索路由回路 · Prakhar Gupta … Zhijing Jin · arXiv 2610.22937 · 2026-10-16 · [解读](https://aisafetyhot.com/items/p90c11quu2j68pi9kjyp20cvo)
4. **[The Reliance Hypothesis: Chain-of-Thought Faithfulness Rises as Language Resource Level Falls](https://arxiv.org/abs/2610.22841)**  
   检验依赖假说，关联语言资源水平与思维链忠实性 · Lucas Resck … Anna Korhonen · arXiv 2610.22841 · 2026-10-16 · [解读](https://aisafetyhot.com/items/nqu7qhwi3iww4u43d321yngcw)
5. **[LEMON: Equivariant Learning over Attention Maps for Zero-Shot Misbehavior Monitoring on New LLMs](https://arxiv.org/abs/2610.22723)**  
   提出注意力等变监控器 LEMON，零样本监测幻觉与越狱 · `防御与护栏` · Guy Bar-Shalom … Haggai Maron · arXiv 2610.22723 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ovvtanex4ex50foane563p5zl)
6. **[Auditing Chinese Web-scale Corpora via Sampled BPE Token Statistics](https://arxiv.org/abs/2608.10678v2)**  
   提出 SAMPLED-BPE，对中文网页语料做抽样 BPE 的 token 级污染审计 · Qingjie Zhang … Han Qiu · arXiv 2608.10678 · 2026-08-11 · [解读](https://aisafetyhot.com/items/l3q1gggb3buwqb2v96c7qk2ds)
7. **[Concept Removal for Frontier Image Generative Models](https://openreview.net/forum?id=s7NR3XGdwq)**  
   用 transcoder 替换模型内部瓶颈层，使特定概念特征可被关闭；在 SD3.5、Flux、Infinity 上取得领先的概念移除效果，并对对抗提示保持鲁棒。 · `防御与护栏` · Aditya Kumar … Franziska Boenisch · ICML 2026 regular
8. **[Multiple Turns, Short Horizons: Measuring Effective-Horizon Compression in Jailbreaks](https://arxiv.org/abs/2610.22928)**  
   测量多轮越狱的有效视界压缩，并用短查询后缀重放续攻 · `越狱与攻击` · Zhipeng Wei … N. Benjamin Erichson · arXiv 2610.22928 · 2026-10-16 · [解读](https://aisafetyhot.com/items/xkmz0kgr6d8yttxlsa8zs4he6)
9. **[Interpreting SSL Representations for Spoof Detection: a WavLM Study](https://arxiv.org/abs/2610.23526)**  
   逐层探测 SSL 语音表征，分析各层对欺骗语音的编码 · Mohamed Mallat … Anthony Larcher · arXiv 2610.23526 · 2026-10-16 · [解读](https://aisafetyhot.com/items/pctljddhh0xm2i247zrdvna1d)
10. **[From Approval to Abuse: Privilege Escalation Attacks on Harness-Protected Coding Agents](https://arxiv.org/abs/2610.22987)**  
   提出用对抗仓库内容诱导编码 Agent 申请可重用权限并静默越权的攻击 · `Agent 安全` · Xianglin Yang … Jiaheng Zhang · arXiv 2610.22987 · 2026-10-16 · [解读](https://aisafetyhot.com/items/wb676773yg4qnifhc3h2s47ll)
11. **[Stealthy Poisoning Attacks via Reused KV Cache of Reasoning](https://arxiv.org/abs/2610.22873)**  
   提出 R2ECAP，借推理 KV 缓存残留对共享缓存实施隐蔽投毒 · L. Zhu … S. Szyller · arXiv 2610.22873 · 2026-10-16 · [解读](https://aisafetyhot.com/items/n379z8tppevqx9fming04vx0s)
12. **[ShadowFPT: Backdooring Federated Prompt Tuning via Shadow Triggers](https://arxiv.org/abs/2610.22871)**  
   提出 ShadowFPT，用影子触发器在联邦提示微调中植入定向后门 · `后门与投毒` · Kun Zhai … Xingjun Ma · arXiv 2610.22871 · 2026-10-16 · [解读](https://aisafetyhot.com/items/tl0z3j1aupwtk5bf9736kehki)
13. **[Reasoning Models Can Control Their Chains of Thought When They Tell Themselves To](https://arxiv.org/abs/2610.23257)**  
   评测推理模型在自我指令下控制思维链的能力 · Uriel Dolev … Yoav Goldberg · arXiv 2610.23257 · 2026-10-16 · [解读](https://aisafetyhot.com/items/ud8dymf914u4s943nn62cco1j)
14. **[Trapped in Your Story: Evaluating Narrative-Induced Sycophancy in Large Language Models](https://arxiv.org/abs/2610.23525)**  
   构建叙事匹配基准，评测模型向用户立场偏移的谄媚 · Runtai Yang … Guangtao Zhai · arXiv 2610.23525 · 2026-10-16 · [解读](https://aisafetyhot.com/items/wq9d2ixe92ckvm57cir7ppdjq)
15. **[OwlSight: A Panoramic Monitor for Chain-of-Thought Reasoning](https://arxiv.org/abs/2610.23670)**  
   提出用 Factor 条件化小模型的思维链监测器 OwlSight · Lewen Yan … Jing Shao · arXiv 2610.23670 · 2026-10-16 · [解读](https://aisafetyhot.com/items/v2j2auhmrqvbzzk3axfhwzcwg)
16. **[What It Is, Not What It Says: Securing Agentic Browsing Interactions with Web Semantics](https://arxiv.org/abs/2610.22697)**  
   提出 INTACT，用网页语义与虚拟隔离限制浏览智能体越权操作 · Umar Iqbal · arXiv 2610.22697 · 2026-10-15 · [解读](https://aisafetyhot.com/items/eok59nm2tbngljm4zmc6ss7fy)
17. **[SciΠvot: Benchmarking Principal-Investigator Judgment at Pivotal Moments of Scientific AutoResearch Agents](https://huggingface.co/papers/2610.21082)**  
   评测科学 AutoResearch 智能体在关键节点识别人类纠正计划的判断 · Youran Sun … Haizhao Yang · arXiv 2610.21082 · 2026-10-15 · [解读](https://aisafetyhot.com/items/lgzycss5c1h9690scooib0j50)
18. **[Has GPT-6-Astra Achieved Embodied Intelligence?](https://huggingface.co/papers/2610.22471)**  
   评测固定权重通用模型在操作导航基准与真机上的具身能力 · SenseNova … Jing Zuo · arXiv 2610.22471 · 2026-10-15 · [解读](https://aisafetyhot.com/items/zee4p7ou9yrpzrk2rsmyql2cy)
19. **[Refusal Is Not Robustness: Measuring Harmful Reachability in Autoregressive Language Models](https://arxiv.org/abs/2610.22754)**  
   提出 BCA 与 GAS，测量拒答下有害延续的可达概率 · Parv Kapoor … Eunsuk Kang · arXiv 2610.22754 · 2026-10-15 · [解读](https://aisafetyhot.com/items/dry6ppyk0dnjuj26yy7yp749z)
20. **[Progressive Misalignment Can Emerge from Benign Recursive Self-Distillation](https://arxiv.org/abs/2610.22467)**  
   揭示良性递归自蒸馏导致安全模型渐进式失齐 · Karim Abdel Sadek … Fanny Yang · arXiv 2610.22467 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ujwh1kjbpakh2acmxnmy3vh92)
21. **[The Model Knows Better: Defending Medical Multi-Agent Systems Against Prompt Injection](https://arxiv.org/abs/2610.22594)**  
   提出免训练防御，核验病历临床判断以抵御医疗多智能体提示注入 · Fardin Ahsan Sakib … Ozlem Uzuner · arXiv 2610.22594 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ehzutnactkaccdebiba96k7tg)
22. **[RedDarwin: Evolving Jailbreak Skills against Frontier LLMs](https://arxiv.org/abs/2610.23726)**  
   提出 REDDARWIN，将越狱方法演化为可执行技能以攻击前沿 LLM · `越狱与攻击` · Zhouyuan Ma … Xingjun Ma · arXiv 2610.23726 · 2026-10-14 · [解读](https://aisafetyhot.com/items/wd5x5gztipurgec9y4eaq1ksu)
23. **[Safe-FCL: Continual Risk Awareness and Fine-Grained Safety Aggregation for Federated Continual Learning of LLMs](https://arxiv.org/abs/2610.19968)**  
   提出 Safe-FCL，在联邦持续学习中识别并抑制演变的恶意更新 · Shuaijie Ma … Zhaoxia Yin · arXiv 2610.19968 · 2026-10-14 · [解读](https://aisafetyhot.com/items/lkox31msmz7q8obcwsf3jr6dv)
24. **[Monitor-Validity Failures: LLM Safety Evidence Paths at Evolving Framework Boundaries](https://arxiv.org/abs/2610.23362)**  
   用 canary contract 检验 LLM 框架的监控证据路径 · Junchi Liao · arXiv 2610.23362 · 2026-10-16 · [解读](https://aisafetyhot.com/items/lwl9mxcxyulyxapqbx44qce6g)
25. **[Trojan Horse: Automated Repository Poisoning against Coding Agents](https://arxiv.org/abs/2610.23109)**  
   提出 TROJANFORGE，对编码 Agent 做自动化代码仓库投毒 · Xiao Yang … Chenfu Bao · arXiv 2610.23109 · 2026-10-16 · [解读](https://aisafetyhot.com/items/ywsjr23dx77p1wq7vdiminlyc)
26. **[Rethinking GRPO for Large Reasoning Model Safety Alignment](https://arxiv.org/abs/2610.23085)**  
   提出 Beacon，用 SSR 与 SUDA 改进推理模型的 GRPO 安全对齐 · `防御与护栏` · Jiawei Chen … Zhaoxia Yin · arXiv 2610.23085 · 2026-10-16 · [解读](https://aisafetyhot.com/items/c00tegsmue8goswm3ywr4vu7s)
27. **[Beyond Surface Cues: Robust LLM-Generated Korean Text Detection](https://arxiv.org/abs/2610.22940)**  
   提出韩语基准 KOLING 与检测器 KOLINGPROBE 并评测文本区分 · SungHo Kim, SangKeun Lee · arXiv 2610.22940 · 2026-10-16 · [解读](https://aisafetyhot.com/items/inr0geqr7tmsp8nuadf9q5p5d)
28. **[Conformal Policy Selection: When to Deploy AI Decisions for Targeted Intervention](https://arxiv.org/abs/2610.22930)**  
   提出 Conformal Policy Selection，控制定向部署入选集的错误发现率 · Junyu Cao … Mingzhang Yin · arXiv 2610.22930 · 2026-10-16 · [解读](https://aisafetyhot.com/items/s8v50l2vafob375h7mq2uzzdq)
29. **[GRAD: Graph-Structured Antibody Defense for LLM Agents](https://arxiv.org/abs/2610.22828)**  
   提出 GRAD，用执行图检测智能体的记忆投毒与分解攻击 · Tianqi Song … Zheng Wang · arXiv 2610.22828 · 2026-10-16 · [解读](https://aisafetyhot.com/items/if2wcchyxxj8vzl68j80qpeyg)
30. **[SemPurify: Semantics-Aware Data Purification for Black-box Backdoor Defense](https://arxiv.org/abs/2610.23589)**  
   提出 SemPurify，用多层语义引导图像修复做黑盒后门净化 · Jiawei Yu … Jian Liu · arXiv 2610.23589 · 2026-10-16 · [解读](https://aisafetyhot.com/items/lh18aofwv77r0odkr6y0ngq2w)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 19 · [Agent 安全](daily-papers/topics/agent-security.md) 8 · [后门与投毒](daily-papers/topics/backdoor.md) 6 · [隐私与数据泄露](daily-papers/topics/privacy.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [奖励作弊](daily-papers/topics/reward-hacking.md) 4 · [越狱与攻击](daily-papers/topics/jailbreak.md) 4 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 支持

觉得有用，欢迎点个 Star，或[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
