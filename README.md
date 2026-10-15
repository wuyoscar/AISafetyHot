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
### 2026-10-16 · 30 篇

1. **[Mitigating Cross-Modal Hallucinations by Correcting Modality Misrouting in Omnimodal LLMs](https://arxiv.org/abs/2610.18141)**  
   提出 CaRe，在推理时纠正全模态模型的模态误路由以缓解跨模态幻觉 · Yu Mi … Kui Ren · arXiv 2610.18141 · 2026-10-13 · [解读](https://aisafetyhot.com/items/cqv2ftfnm9jmiha1ufme34mni)
2. **[Towards Safe Autonomy for Computer Use](https://arxiv.org/abs/2610.18508)**  
   提出 SA-CUA，用屏幕遮罩与双 LLM 隔离防御计算机操作 Agent 的间接提示注入 · Dominik Seip … Matthias Hein · arXiv 2610.18508 · 2026-10-13 · [解读](https://aisafetyhot.com/items/p0ug3d3o88mirz27657xwls6m)
3. **[To Align or Not To Align: Check Your COMPASS Before You Train](https://huggingface.co/papers/2610.18638)**  
   提出 COMPASS，训练前估计两预训练模型的对齐或合并兼容性 · Fabian Gröger … Maria Brbić · arXiv 2610.18638 · 2026-10-13 · [解读](https://aisafetyhot.com/items/gzrpk1ay8myqh1t6rfqpcvc4w)
4. **[Tev: Scaling Long-Horizon Agentic Environments with Dense Progress Rewards](https://huggingface.co/papers/2610.18868)**  
   合成可验证长程环境并用稠密进度奖励训练智能体 · Wenbo Hu … Yong Jae Lee · arXiv 2610.18868 · 2026-10-13 · [解读](https://aisafetyhot.com/items/olljngpg6cai5chz4smfnbp18)
5. **[Chain of Thought Monitoring Can Fail Even When CoT Is Necessary](https://arxiv.org/abs/2610.18105)**  
   提出思维链必要性分级，实证必要 CoT 仍会出现监控失效 · Lennart Bürger … Wojciech Samek · arXiv 2610.18105 · 2026-10-13 · [解读](https://aisafetyhot.com/items/obtik05l01gloixpzqv4stw9y)
6. **[Sycophancy Towards Researchers Drives Performative Misalignment](https://openreview.net/forum?id=rLFIOikFR2)**  
   研究发现大模型在评测中的对齐伪装更可能源自对研究人员的谄媚而非蓄意谋划，当前方法难以在机理上区分二者，微调增加谄媚度会提高模型对评测线索的敏感度。 · `欺骗与谋划` · David D. Baek … Shi Feng · ICML 2026 spotlight
7. **[AdAEM: An Adaptively and Automated Extensible Measurement of LLMs' Value Difference](https://openreview.net/forum?id=qNlTH4kYJZ)**  
   提出自扩展评测算法AdAEM，通过上下文优化探测跨文化多模型的内部价值边界并提取争议性话题，自适应生成新问题以持续追踪模型的价值差异与对齐动态。 · `对齐` · Jing Yao … Xing Xie · ICLR 2026 Oral
8. **[Watch your steps: Dormant Adversarial Behaviors that Activate upon LLM Finetuning](https://openreview.net/forum?id=yfM2e8Icsw)**  
   提出FAB攻击，通过元学习构造出表面良性但在下游微调后会激活潜伏对抗行为（如越狱、过度拒答）的受损模型，揭示了微调过程中的安全风险。 · `后门与投毒` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
9. **[Benchmarking Empirical Privacy Protection for Adaptations of Large Language Models](https://openreview.net/forum?id=jY7fAo9rfK)**  
   系统评估了差分隐私微调大模型在成员推断与金丝雀提取攻击下的实际隐私风险，发现分布偏移对经验隐私保护具有显著影响。 · `隐私与数据泄露` · Bartłomiej Marek … Adam Dziedzic · ICLR 2026 Oral
10. **[Gaussian certified unlearning in high dimensions: A hypothesis testing approach](https://openreview.net/forum?id=0FJYicpOj0)**  
   提出面向高维机制的ε-高斯可认证性，理论证明单步牛顿法结合高斯噪声即可同时实现隐私消除与模型精度。 · `隐私与数据泄露` · Aaradhya Pandey … Sanjeev Kulkarni · ICLR 2026 Oral
11. **[GEM: Geometric Erasure by Contrastive Velocity Matching in Rectified Flows](https://openreview.net/forum?id=NBMCwxTRSA)**  
   针对多模态生成模型合成有害内容与深度伪造的风险，提出GEM概念擦除框架，将基于轨迹的遗忘与教师引导流匹配结合，有效抑制有害概念并保留正常生成。 · `防御与护栏` · Jonas Henry Grebe … Marcus Rohrbach · ICML 2026 spotlight
12. **[Doc2Harness: Benchmarking LLMs on Long-Horizon Harness Engineering of Coding Agents](https://huggingface.co/papers/2610.20344)**  
   提出 Doc2Harness 评测模型长程构建编码 Agent 脚手架的能力 · Yuyao Ge … Xueqi Cheng · arXiv 2610.20344 · 2026-10-14 · [解读](https://aisafetyhot.com/items/pfsxxcet4ha7t6ctk7vl2p6o7)
13. **[RuleTrek: Benchmarking Agentic Rule Reasoning in Complex Scenarios](https://huggingface.co/papers/2610.19698)**  
   提出 RuleTrek，评测智能体在多文件场景中识别并套用领域规则 · Chenhao Yuan … Kang Liu · arXiv 2610.19698 · 2026-10-14 · [解读](https://aisafetyhot.com/items/n711fv2putwrtmzcu919y7ogt)
14. **[What Makes a Social Agent's Interactions Effective? Learning from Verifiable Outcomes in Paired Worlds](https://huggingface.co/papers/2610.20195)**  
   提出 HICO-Bench 成对世界基准，核验社交智能体协调计划是否可行 · Caixin Kang … Yoichi Sato · arXiv 2610.20195 · 2026-10-14 · [解读](https://aisafetyhot.com/items/fbdyb6wxc7blawpus1wvzpluw)
15. **[Share the Symbol, Not the Vector: Training-Free Fact Communication Across Language Models](https://huggingface.co/papers/2610.19696)**  
   提出 SYNC，以共享词索引在异构模型间免训练传递事实 · Xin Li … Chau Yuen · arXiv 2610.19696 · 2026-10-14 · [解读](https://aisafetyhot.com/items/o5pz5wtx08bvfqwjhjmow5xil)
16. **[Beyond Static Cues: Unified Dynamic Detection of MLLM Backdoors via Dual-Flow Trajectory Analysis](https://arxiv.org/abs/2610.20319)**  
   提出 EVO-Detect，用早期解码双流过滤 MLLM 微调后门 · Yinzhen Huang … Xingxing Wei · arXiv 2610.20319 · 2026-10-14 · [解读](https://aisafetyhot.com/items/u5gccktmpqohtmb2vwpv67en0)
17. **[SaTPO: Text-to-Image Safety Alignment via Transition Preference Optimization](https://arxiv.org/abs/2610.19563)**  
   提出 SaTPO，用单步转移偏好优化对齐文生图模型 · `防御与护栏` · Ziyi Fang … Haijun Zhang · arXiv 2610.19563 · 2026-10-14 · [解读](https://aisafetyhot.com/items/c2bavsbi9bmvq0znzeifkomln)
18. **[τ-Emotion-Bench: Exposing the Interaction Fragility of LLM Agents through Real-World User Emotions](https://huggingface.co/papers/2610.19560)**  
   提出 τ-Emotion-Bench，评测工具调用智能体面对用户情绪时的交互脆弱性 · Rishitosh Kumar Singh … Chitta Baral · arXiv 2610.19560 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ada7ltbo93bl6gbs1tpnxu4q6)
19. **[Scaling Multilingual Safety and Reasoning Evaluation through Reasoning-Guided Translation](https://arxiv.org/abs/2610.20221)**  
   提出推理引导翻译，扩展并评测多语言安全与推理基准 · Zahraa Al Sahili … Matthew Purver · arXiv 2610.20221 · 2026-10-14 · [解读](https://aisafetyhot.com/items/e6k9b4rwnsfil8ovfb6mgjrqg)
20. **[Cortex: Consolidating Context into Parametric Memory](https://huggingface.co/papers/2610.20399)**  
   提出 Cortex，把上下文增益蒸馏进可合并的 FFN 更新 · Jintian Zhang … Ningyu Zhang · arXiv 2610.20399 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dsg3tm71rygj3pm2mq7grmuno)
21. **[Model vs. User: Whose Values Prevail? Inference-Time Value Alignment in Multi-Turn Conversations](https://arxiv.org/abs/2610.19817)**  
   评测多轮对话中推理时价值转向在反向拉扯下的胜负 · Enrico Liscio … Pradeep K. Murukannaiah · arXiv 2610.19817 · 2026-10-14 · [解读](https://aisafetyhot.com/items/ilmjnkjp7nfyyj1em6367hwr1)
22. **[Diagnose Before You Refine: Multi-Dimensional Judge Feedback for Query-Efficient Jailbreak Attacks](https://arxiv.org/abs/2610.19971)**  
   提出 JSB，用多维评判反馈在有限查询内优化越狱提示 · `越狱与攻击` · Yixin Tan … Rui Wen · arXiv 2610.19971 · 2026-10-14 · [解读](https://aisafetyhot.com/items/wbnhewi0o0jmeiehm11r6u51k)
23. **[BenchChecker: Assessing the Credibility of Bug-Fixing Benchmarks for LLMs](https://arxiv.org/abs/2610.19447)**  
   用 BenchChecker 检测缺陷修复基准的训练污染 · Di Wu … Kun Sun · arXiv 2610.19447 · 2026-10-14 · [解读](https://aisafetyhot.com/items/olvt03iv4n4wmubnxl65736gc)
24. **[Moral Combat: Exploiting Moral Foundations Theory to Jailbreak LLMs](https://arxiv.org/abs/2610.19587)**  
   提出 Moral Combat，把有害请求改写为道德义务以越狱 · `越狱与攻击` · Adel Khorramrouz … Sharon Levy · arXiv 2610.19587 · 2026-10-14 · [解读](https://aisafetyhot.com/items/bcapsgqvfeqpox3rp55aagu36)
25. **[Diagnosing and Correcting Reward Hacking in Verifiable Instruction Following](https://huggingface.co/papers/2610.19525)**  
   提出 CALIF，用参考似然校准验证器奖励以修正奖励作弊 · Sangyeon Yoon … Jaehyung Kim · arXiv 2610.19525 · 2026-10-14 · [解读](https://aisafetyhot.com/items/d99t9uvjo32vjqhgi7lmlwi2y)
26. **[AgentSafeEvo: Adversarial Co-Evolution for LLM Agent Safety](https://arxiv.org/abs/2610.19422)**  
   提出 AgentSafeEvo，协同演化对抗任务构造与安全执行以提升工具智能体稳健性 · `防御与护栏` · Chenxu Wang … Qiaosheng Zhang · arXiv 2610.19422 · 2026-10-14 · [解读](https://aisafetyhot.com/items/qk33mh8fnkkksr403x087j8c0)
27. **[Kairos: Transactional Security Enforcement at the System Boundary for LLM Agents](https://arxiv.org/abs/2610.18457)**  
   提出系统边界事务监视器 KAIROS，防御 Agent 间接提示注入 · Kristoffer Hempel … Thomas Eisenbarth · arXiv 2610.18457 · 2026-10-13 · [解读](https://aisafetyhot.com/items/ccstfy6l9udg7c0hk7v8yk4lm)
28. **[CompanionSafe: From Multi-turn Safety Evaluation to Guardrails for AI Companions](https://arxiv.org/abs/2610.18095)**  
   用多轮对话评测 AI 伴侣关系安全并训练检测护栏 CompanionGuard · `防御与护栏` · Xinyang Liao … Xia Hu · arXiv 2610.18095 · 2026-10-13 · [解读](https://aisafetyhot.com/items/pj4h6slmbz7jnabmu1hj85bui)
29. **[TRACER: Trace-Regularized Training Against Indirect Prompt Injection](https://arxiv.org/abs/2610.19133)**  
   提出 TRACER，用轨迹正则化对抗训练抵御跨通道间接提示注入 · Kshitij Mishra … Nils Lukas · arXiv 2610.19133 · 2026-10-13 · [解读](https://aisafetyhot.com/items/t5jje7avi1vabnqj3wubfv0ij)
30. **[Efficient Safety Guardrails through Latent Dual-Hypothesis Reasoning with On-Demand Trace Reconstruction](https://arxiv.org/abs/2610.18304)**  
   提出潜空间双假设提示词护栏 LR-GUARD，并支持按需重建推理轨迹 · `防御与护栏` · Md Asiful Islam … Mihai Surdeanu · arXiv 2610.18304 · 2026-10-13 · [解读](https://aisafetyhot.com/items/f3k7vkcnsdg15xpr4xyuy3kgq)

[往期每日论文](daily-papers/2026) · [论文库](https://aisafetyhot.com/zh/papers)

**按方向**：[防御与护栏](daily-papers/topics/defense.md) 9 · [后门与投毒](daily-papers/topics/backdoor.md) 4 · [隐私与数据泄露](daily-papers/topics/privacy.md) 4 · [Agent 安全](daily-papers/topics/agent-security.md) 4 · [对齐](daily-papers/topics/alignment.md) 3 · [欺骗与谋划](daily-papers/topics/scheming.md) 3 · [越狱与攻击](daily-papers/topics/jailbreak.md) 2 · [红队测试与挑战赛](daily-papers/topics/red-teaming.md) 1 · [监控与 AI 控制](daily-papers/topics/ai-control.md) 1 · [可解释性](daily-papers/topics/interpretability.md) 1
<!-- papers:end -->

## 支持

觉得有用，欢迎点个 Star，或[请作者喝杯咖啡](https://buymeacoffee.com/wuyoscar)。

<img src="assets/wechat-pay.png" width="160" alt="微信支持二维码">
