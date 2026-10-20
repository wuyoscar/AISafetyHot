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
### 2026-10-21 · 30 篇

1. **[Safety Mid-Training: Internalizing LLM Safety as a Foundational Capability](https://arxiv.org/abs/2610.26809)**  
   提出 safety mid-training，在预训练与后训练之间内化安全 · `防御与护栏` · Zhengyue Zhao … Chaowei Xiao1 · arXiv 2610.26809 · 2026-10-19 · [解读](https://aisafetyhot.com/items/wfp2wlfdgxteanseiqx23rc24)
2. **[Towards Robust Model Organisms for Eliciting Latent Knowledge](https://arxiv.org/abs/2610.26698)**  
   训练选择性隐瞒漏洞的沙袋模型生物并评测其抗诱导性 · Lennart Finke … Mary Phuong · arXiv 2610.26698 · 2026-10-19 · [解读](https://aisafetyhot.com/items/q3ls1kh1jec8sgbzdit34vl5e)
3. **[Training Natural Schemers: RL Can Amplify Oversight-Conditional Behavior](https://arxiv.org/abs/2610.26551)**  
   检验只奖励合规的强化学习是否放大监督条件化谋划 · Bart Jaworski … Victoria Krakovna · arXiv 2610.26551 · 2026-10-19 · [解读](https://aisafetyhot.com/items/fcrbp7ewnbfdvu0zoewtnoia8)
4. **[CUA-Lite: An Open Platform for Computer Use Agents](https://arxiv.org/abs/2610.26071)**  
   提出 CUA-Lite 平台，统一计算机使用智能体的环境、数据与评测训练 · Zhanhui Zhou … Dawn Song · arXiv 2610.26071 · 2026-10-19 · [解读](https://aisafetyhot.com/items/z19vammwycrhfmvkqn931mp19)
5. **[Towards Human-AI Complementarity for AI Safety](https://arxiv.org/abs/2610.24969)**  
   评测安全任务上的人机互补，并比较辅助与路由能否超过更优单源 · Sander Lanbo Shi … Rishub Jain · arXiv 2610.24969 · 2026-10-18 · [解读](https://aisafetyhot.com/items/e5uiu27ctfzqgxy0gom7njy2j)
6. **[Persistent Representational Misalignment Induces Vision-Language Model Failures](https://arxiv.org/abs/2610.25252)**  
   分析视觉与语言表征的线性不可对齐如何导致 VLM 失败 · Yonatan Gideoni … Yarin Gal · arXiv 2610.25252 · 2026-10-18 · [解读](https://aisafetyhot.com/items/c6dk3h316iip6hr3qsgpsacjk)
7. **[AdaExploreBench: Benchmarking LLM Agents for Proactive Exploration and Test-time Adaptation in Evolving Environments](https://huggingface.co/papers/2610.25950)**  
   提出 AdaExploreBench，评测智能体对隐规则的主动探索与漂移适应 · Rui Wang … Yangqiu Song · arXiv 2610.25950 · 2026-10-19 · [解读](https://aisafetyhot.com/items/s1vnb5ws2ionrv8geiutnj4f4)
8. **[AfriGuard: Safety and Robust Refusal For African Languages](https://arxiv.org/abs/2610.26474)**  
   提出 AFriGuard 评测非洲语言的安全分类与拒答 · Israel Abebe Azime … Julia Kreutzer · arXiv 2610.26474 · 2026-10-19 · [解读](https://aisafetyhot.com/items/dgt1da20695d04jiif20ohf90)
9. **[Where is Physical RSI capability from? An Observational Scaling Law of LLM-as-policy](https://huggingface.co/papers/2610.26848)**  
   评测具身 Agent 的物理 RSI 能力来源、缩放与经验复用 · Zekai Li … Li Yi · arXiv 2610.26848 · 2026-10-19 · [解读](https://aisafetyhot.com/items/oq7cyi8n8jhjri9olgtdxhe6z)
10. **[SPARC: Spoken Profile Authorship Recognition Corpus](https://huggingface.co/papers/2610.25265)**  
   提出 SPARC 基准，评测转写文本能否验证说话人身份与属性 · Efthymios Tsaprazlis … Shrikanth Narayanan · arXiv 2610.25265 · 2026-10-18 · [解读](https://aisafetyhot.com/items/g7ltz1gao5ual1d72rmltdu7m)
11. **[World Model Interpretability: From Decoding Representations to Understanding Latent Worlds](https://huggingface.co/papers/2610.25296)**  
   提出四阶段议程，把 JEPA 可解释性从解码表征推进到理解潜在世界 · Jize Wang … Dacheng Tao · arXiv 2610.25296 · 2026-10-18 · [解读](https://aisafetyhot.com/items/ngtz6m3eg9rycxqj6ag1yk09w)
12. **[Write Once, Check Many: Reusable Ledgers for Post-Hoc Policy Compliance Auditing of Agent Trajectories](https://arxiv.org/abs/2610.24483)**  
   提出策略无关的可复用账本，事后审计 Agent 轨迹是否违规 · `Agent 安全` · Ashwin Nagarajan … Aashiq Muhamed · arXiv 2610.24483 · 2026-10-17 · [解读](https://aisafetyhot.com/items/fjvlb327orrkqb6yw58bgjj2d)
13. **[How Much Do Activation Monitors Benefit from Original Model Computations?](https://arxiv.org/abs/2610.24613)**  
   比较激活监控从原始模型计算与改写轨迹获得的收益 · James Oldfield … Adel Bibi · arXiv 2610.24613 · 2026-10-17 · [解读](https://aisafetyhot.com/items/oj7sca04l0rlsb9j1u3yj1taz)
14. **[Defending Against Dormant Poisoning Attacks Across Language and Multimodal Agents](https://arxiv.org/abs/2610.24379)**  
   提出微调期防御 LOOKAHEAD，抑制语言与多模态智能体的休眠投毒 · Wonjun Lee … Mohit Bansal · arXiv 2610.24379 · 2026-10-17 · [解读](https://aisafetyhot.com/items/qd5lh9572h18b8cji9srpdsdd)
15. **[RATION: Towards Quantitative Risk-Based Access Control for AI Agents](https://arxiv.org/abs/2610.24311)**  
   提出 RATION，用任务级定量风险策略约束智能体工具调用 · `Agent 安全` · Yuntao Du … Ninghui Li · arXiv 2610.24311 · 2026-10-16 · [解读](https://aisafetyhot.com/items/cr3jsr0plahbtitl6tlk16pj0)
16. **[SecOPD: Mitigating Adaptive Prompt Injections by On-Policy Distillation](https://arxiv.org/abs/2608.21500)**  
   提出同策略蒸馏防御微调方法 SecOPD，抵御自适应提示注入 · Yibo Peng … Sizhe Chen · arXiv 2608.21500 · 2026-08-21 · [解读](https://aisafetyhot.com/items/as4ho4hsknempg9ysc21s35m4)
17. **[Towards Automating Data Access Permissions in AI Agents](https://sp2026.ieee-security.org/program.html)**  
   实现 AI Agent 数据访问权限的自动化 · `Agent 安全` · Yuhao Wu … Umar Iqbal · IEEE S&P 2026
18. **[Mitigating Reward Hacking in Preference Reward Models with Evolving Penalties](https://arxiv.org/abs/2610.26496)**  
   提出 Dynalize，在强化学习中用演化惩罚缓解偏好奖励模型的奖励作弊 · Afonso Baldo … Nuno M. Guerreiro · arXiv 2610.26496 · 2026-10-19 · [解读](https://aisafetyhot.com/items/ok0cqsfh0h9mimltr8k6il6ie)
19. **[Statistical Learning Theory for Direct Preference Optimization](https://arxiv.org/abs/2610.25856)**  
   用 triangle-curl 刻画 DPO 的结构失配并给出容量无关风险下界 · Joel Wills … Ding-Xuan Zhou · arXiv 2610.25856 · 2026-10-19 · [解读](https://aisafetyhot.com/items/xb0888nlm54b9enj1md3e4ym9)
20. **[A Calibrated Instrument for Detecting Disposition Drift in Language Models](https://arxiv.org/abs/2610.25735)**  
   提出校准仪器，测量语言模型微调后的行为倾向漂移 · Jerry Kaplan · arXiv 2610.25735 · 2026-10-19 · [解读](https://aisafetyhot.com/items/rev1k62b4dwv1q1neiam42vj7)
21. **[Selective Transfer through Sequence Distillation: From Benchmark Knowledge to Backdoor Behaviour](https://arxiv.org/abs/2610.26311)**  
   比较蒸馏通道对基准知识与拒答后门的选择性传递 · Jonibek Mansurov … Alham Fikri Aji · arXiv 2610.26311 · 2026-10-19 · [解读](https://aisafetyhot.com/items/zz7n6icawj4btl9byqqg9tdre)
22. **[Safety Offset Learning: When Benign Fine-Tuning Misaligns LLMs](https://arxiv.org/abs/2610.25611)**  
   提出 SAFEOFF，用良性微调把拒绝到遵从迁到有害请求 · Jesson Wang … Mengyuan Li · arXiv 2610.25611 · 2026-10-19 · [解读](https://aisafetyhot.com/items/e07cc4jlpoekr01e28vba2k4v)
23. **[Q-MALDetect: Quantum Image-Based Malware Detection and Adversarial Robustness Analysis](https://arxiv.org/abs/2610.26240)**  
   评测量子图像恶意软件检测器在梯度扰动与 NOP 插入下的鲁棒性 · Walid El Maouaki … Muhammad Shafique · arXiv 2610.26240 · 2026-10-19 · [解读](https://aisafetyhot.com/items/hpw430l4sqf9xuumpk816y821)
24. **[Risk Decomposition for Hallucination-Aware Video Sampling](https://arxiv.org/abs/2610.26069)**  
   提出视频物理幻觉的二维风险分解及免训练采样器 HA-Sampler · Chenyan Zheng … Guosheng Lin · arXiv 2610.26069 · 2026-10-19 · [解读](https://aisafetyhot.com/items/kb9h8uctzol4rg5enb7yhsehu)
25. **[Claim Laundering: When Agent Decision Models Trust Records Over Reality](https://arxiv.org/abs/2610.25947)**  
   分析智能体决策模型信记录胜过观察的内部机制，并提出 EVIGATE · Tina Khezresmaeilzadeh … Massoud Pedram · arXiv 2610.25947 · 2026-10-19 · [解读](https://aisafetyhot.com/items/w0clff85px01bvbhe3g93f6gt)
26. **[RAGLeak: Supply-Chain Privacy Backdoors in Retrieval-Augmented Generation](https://arxiv.org/abs/2610.25937)**  
   提出 RAGLeak，用投毒微调植入可逆混淆后门以泄露 RAG 检索文档 · `后门与投毒` · Yuchen Chen … Zhenyu Chen · arXiv 2610.25937 · 2026-10-19 · [解读](https://aisafetyhot.com/items/glsembbaas25wl0zhoni27a5w)
27. **[Towards Architectural-Level Safety Control: Relocating Hazardous Knowledge into Removable Experts in Mixture-of-Experts Models](https://arxiv.org/abs/2610.25791)**  
   提出 REX，将 MoE 危险知识迁入可切除专家后移除 · Cheng Jin … Qiaosheng Zhang · arXiv 2610.25791 · 2026-10-19 · [解读](https://aisafetyhot.com/items/b8iga839z4pzzjqo30w0p8cev)
28. **[Fake News, Real Crashes: Information Injection Attacks on LLM Financial Trading Agents](https://arxiv.org/abs/2610.26438)**  
   提出信息注入攻击，用公开伪造新闻改变交易智能体的下单决策 · Mengxiao Wang, Nitesh Saxena · arXiv 2610.26438 · 2026-10-19 · [解读](https://aisafetyhot.com/items/gexawmv1fyij2t9hba4gv89xd)
29. **[AnyGoal: On World Model Generalization Beyond Expert Rollouts](https://huggingface.co/papers/2610.26844)**  
   用 AnyGoal 评测世界模型在专家轨迹外的组合泛化 · Heejeong Nam … David Klindt · arXiv 2610.26844 · 2026-10-19 · [解读](https://aisafetyhot.com/items/bpi06zafwpkke805hc5i02prg)
30. **[SpanGuard: Decoupling Instruction Localization from Authorization for Lightweight IPI Defense](https://arxiv.org/abs/2610.26013)**  
   提出 SpanGuard，解耦指令定位与授权判断以防御间接提示注入 · Yinxiang Wang … Han Fang · arXiv 2610.26013 · 2026-10-19 · [解读](https://aisafetyhot.com/items/edrow0r7iy26azqnf9e42pr2x)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 20 · [Agent 安全](daily-papers/topics/agent-security.md) 11 · [后门与投毒](daily-papers/topics/backdoor.md) 7 · [隐私与数据泄露](daily-papers/topics/privacy.md) 5 · [对齐](daily-papers/topics/alignment.md) 4 · [奖励作弊](daily-papers/topics/reward-hacking.md) 4 · [越狱与攻击](daily-papers/topics/jailbreak.md) 4 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 2 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 2 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 反馈与支持

内容摘要和解读由 AI 辅助整理，关键结论请结合原文阅读。发现错误或想推荐材料，欢迎到[留言板](https://aisafetyhot.com/zh/board)交流。

觉得有用，欢迎 **Star**，方便下次回来；也可以[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
