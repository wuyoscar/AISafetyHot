# Agent 安全

每日论文里归到「Agent 安全」的 22 篇，按推送日期从新到旧。

1. **[Agent Security is a Systems Problem](https://neurips.cc/virtual/2026/poster/140106)**  
   立场论文：主张把驱动 Agent 的模型视为不可信组件、在系统层强制安全不变量，并分析 11 个真实攻击说明系统原则本可阻止。 · `Agent 安全` · Mihai Christodorescu … Nishit V Pandya · NeurIPS 2026 oral
2. **[Soteria: Formally Verified Planning with Runtime Enforcement for Safe LLM Agents](https://neurips.cc/virtual/2026/poster/154927)**  
   提出 Soteria 框架，执行前对结构化计划做形式化验证、执行中强制规范符合，在多个工具使用基准上实现完美规范符合并将效用提升至多 5 倍。 · `Agent 安全` · Deyuan (Mike) He … Aarti Gupta · NeurIPS 2026 oral
3. **[Do AI-for-Science Agents Preserve Model Safety?](https://arxiv.org/abs/2610.32045)**  
   评测 AI-for-Science 智能体框架在有害化学请求上的安全性 · `Agent 安全` · Michael Yew Chuan Lee … N. Benjamin Erichson · arXiv 2610.32045 · 2026-10-23 · [解读](https://aisafetyhot.com/items/fkzxub62y1ve66zbwqz5v4ef2)
4. **[The Helpful Agent Problem: When Emergent Cooperation Among LLM Agents Bypasses Intended Workflows](https://arxiv.org/abs/2610.31985)**  
   马萨诸塞大学阿默斯特分校研究者提出“乐于助人智能体问题”：目标独立、无共享奖励的 LLM 智能体在审核者不可用时会自发替同伴改动资源，这些操作都在各自权限内，却绕过了系统设定的审核工作流。 · `Agent 安全` · Moumita Choudhury … Shlomo Zilberstein · arXiv 2610.31985 · 2026-10-22 · [解读](https://aisafetyhot.com/items/dlmgvsnxt7mlur50ggsk2s7vt)
5. **[Local Allow, Global Deny: Why Per-Action Authorization Does Not Compose in LLM Agents](https://arxiv.org/abs/2610.27620)**  
   刻画逐动作授权的组合失败，并用 AL-SYNTH 合成最小证人 · `Agent 安全` · Anmol Pandey … Carsten Maple · arXiv 2610.27620 · 2026-10-20 · [解读](https://aisafetyhot.com/items/un7u9wq6jn9gwwfwduloq2yc8)
6. **[Beyond the Mandate: A Systematic Security Analysis of the Agent Payments Protocol (AP2)](https://arxiv.org/abs/2608.23858)**  
   系统分析智能体支付协议的前置上下文操纵与授权威胁 · `Agent 安全` · Avital Aviv … Asaf Shabtai · arXiv 2608.23858 · 2026-08-24 · [解读](https://aisafetyhot.com/items/dm4zx6om9wqwxmerjr3l5yob1)
7. **[Disclosure Begets Disclosure: A Self-Reinforcing Privacy Loop in LLM Agents with Persistent Memory](https://arxiv.org/abs/2610.28315)**  
   测量持久记忆 LLM 智能体查阅记忆引发的自我强化隐私泄露循环 · `Agent 安全` · Masahiro Kaneko … Timothy Baldwin · arXiv 2610.28315 · 2026-10-20 · [解读](https://aisafetyhot.com/items/y3r8l1llcgu5y8f8sbaadjgxo)
8. **[Act on Your Behalf, Beyond Your Authorization: Benchmarking LLM Agent Authorization Alignment](https://arxiv.org/abs/2610.27548)**  
   提出 AUTHORIZATION BENCH，评测 Agent 是否越出授权范围 · `Agent 安全` · Zhiping Zhang … Tianshi Li · arXiv 2610.27548 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ir5vlj7aettc0527ng2bz6bxg)
9. **[MAS-Guard: Unified Guardrails from Individual Agents to Multi-Agent LLM Systems](https://arxiv.org/abs/2610.28397)**  
   提出 MAS-Guard，在单智能体与多智能体边界统一拦截不安全动作与对抗操纵 · `Agent 安全` · Mohammad Kachuee … Dan Roth · arXiv 2610.28397 · 2026-10-20 · [解读](https://aisafetyhot.com/items/jmbovkl9cqzg7j0e7gmshtmr2)
10. **[Copyright-Bench: Agentic Evaluation of Copyright Law Compliance](https://openreview.net/forum?id=7y6a5ouziq)**  
   构建评估 LLM 智能体版权法合规性的基准，发现智能体在有公共领域替代品时仍选用侵权内容，开源权重模型在用户偏好和时间压力下违规率上升。 · `Agent 安全` · Zheng Hui … Noam Kolt · ICML 2026 spotlight
11. **[KNOX: Hardware-assisted Regulatory Sandbox for Generative Models](https://arxiv.org/abs/2610.27543)**  
   提出监管沙箱 KNOX，在 TEE 内拦截未授权工具与系统调用 · `Agent 安全` · Vasisht Duddu … Xi He · arXiv 2610.27543 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ktzhekpslnbmrcb295rc74llg)
12. **[Write Once, Check Many: Reusable Ledgers for Post-Hoc Policy Compliance Auditing of Agent Trajectories](https://arxiv.org/abs/2610.24483)**  
   提出策略无关的可复用账本，事后审计 Agent 轨迹是否违规 · `Agent 安全` · Ashwin Nagarajan … Aashiq Muhamed · arXiv 2610.24483 · 2026-10-17 · [解读](https://aisafetyhot.com/items/fjvlb327orrkqb6yw58bgjj2d)
13. **[RATION: Towards Quantitative Risk-Based Access Control for AI Agents](https://arxiv.org/abs/2610.24311)**  
   提出 RATION，用任务级定量风险策略约束智能体工具调用 · `Agent 安全` · Yuntao Du … Ninghui Li · arXiv 2610.24311 · 2026-10-16 · [解读](https://aisafetyhot.com/items/cr3jsr0plahbtitl6tlk16pj0)
14. **[Towards Automating Data Access Permissions in AI Agents](https://sp2026.ieee-security.org/program.html)**  
   实现 AI Agent 数据访问权限的自动化 · `Agent 安全` · Yuhao Wu … Umar Iqbal · IEEE S&P 2026
15. **[From Approval to Abuse: Privilege Escalation Attacks on Harness-Protected Coding Agents](https://arxiv.org/abs/2610.22987)**  
   提出用对抗仓库内容诱导编码 Agent 申请可重用权限并静默越权的攻击 · `Agent 安全` · Xianglin Yang … Jiaheng Zhang · arXiv 2610.22987 · 2026-10-16 · [解读](https://aisafetyhot.com/items/wb676773yg4qnifhc3h2s47ll)
16. **[Learning When to Withdraw: Curriculum Coverage and Rule-Specific Failures in Fine-Tuned Language Agents](https://arxiv.org/abs/2610.21045)**  
   分析课程覆盖不足如何导致微调语言智能体出现规则级撤回失败 · `Agent 安全` · Mohamed Abouzahra · arXiv 2610.21045 · 2026-10-15 · [解读](https://aisafetyhot.com/items/y1qimk3lfaj3hsu9a6i7l8ghi)
17. **[Salesforce 等提出 A2-Failures：跨委托人 Agent 协作的 20 种失效模式，Agent 从不主动核实对方](https://arxiv.org/abs/2610.19342)**  
   提出 A2-Failures 分类法，刻画跨委托人 Agent 协作的失效模式 · `Agent 安全` · Sarath Shekkizhar … Shafiq Joty · arXiv 2610.19342 · 2026-10-14 · [解读](https://aisafetyhot.com/items/o8dsfdudrd4zonj0udj7t11py)
18. **[StepSafe: Learning Timely Intervention with Context-Aware Safety Reasoning](https://arxiv.org/abs/2610.20960)**  
   用 ASPO 训练步级护栏，在智能体动作执行前及时干预 · `Agent 安全` · Siyi Gu … Arman Cohan · arXiv 2610.20960 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dk33qgs4xq8rrphdz7fip26ye)
19. **[Jev-Guard: Fast Routing and Auditing Agent Actions over Editable Policy Trees](https://arxiv.org/abs/2610.18326)**  
   提出 Jev-Guard，沿可编辑策略树路由并审计智能体动作 · `Agent 安全` · Wenbin Hu … Yangqiu Song · arXiv 2610.18326 · 2026-10-13 · [解读](https://aisafetyhot.com/items/mv86fhx0igz7qw9d4166zk90z)
20. **[Caught in the Act: Probes Effectively Detect Sabotage and Catch Unverbalized Deception](https://arxiv.org/abs/2610.12445)**  
   用 FIBS 训练白盒探针，监控智能体破坏行为与未言明欺骗 · `Agent 安全` · Oskar J. Hollinsworth … Chris Cundy · arXiv 2610.12445 · 2026-10-08 · [解读](https://aisafetyhot.com/items/bp1e2e7mg03hqoq6khww30za7)
21. **[VEPA: Verified Evolving Formal Policy for Lifelong LLM Agent Guardrails](https://arxiv.org/abs/2610.12813)**  
   提出 VEPA，以可验证符号规则演化智能体动作护栏 · `Agent 安全` · Duy Nguyen … Long T. Le · arXiv 2610.12813 · 2026-10-08 · [解读](https://aisafetyhot.com/items/kezphhyq30e7ia9jg9j7i0aqi)
22. **[ActBench: Self-Evolving Benchmark of Behavioral Safety in Cowork Agents](https://arxiv.org/abs/2608.09476)**  
   构建自演化基准 ActBench，评测协作智能体的行为安全 · `Agent 安全` · Hongwei Yao … Kui Ren · arXiv 2608.09476 · 2026-08-10 · [解读](https://aisafetyhot.com/items/u7j21k74eb7orhrgfx42y9hpq)
