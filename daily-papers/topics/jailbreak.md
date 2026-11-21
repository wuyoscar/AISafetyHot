# 越狱与攻击

每日论文里归到「越狱与攻击」的 20 篇，按推送日期从新到旧。

1. **[Question, Then Affirm: Restoring Commitment Does Not Restore Refusal](https://arxiv.org/abs/2611.25929)**  
   研究者在多个商用图像生成器上发现，把被拦截的有害陈述改写成问句、再附加对勾等肯定元素，系统会生成支持原主张的图像，作者称之为延迟语义承诺（DSC）。 · `越狱与攻击` · arXiv 2611.25929 · 2026-11-19 · [解读](https://aisafetyhot.com/items/aui59p72k3q9xp592j1ff2moa)
2. **[Creating Steering Vectors via Input Optimisation](https://arxiv.org/abs/2611.17481)**  
   提出 ActGCG，用 GCG 搜索输入后缀复现 steering vector 的激活与行为 · `越狱与攻击` · Batuhan Akar · arXiv 2611.17481 · 2026-11-12 · [解读](https://aisafetyhot.com/items/fxafmziktxxltvw1owro217yf)
3. **[AUTEUR: Acoustic Plan Learning for Red-Teaming Text-to-Audio Models](https://arxiv.org/abs/2611.09351)**  
   提出 AUTEUR 声学计划学习框架，自动化红队测试文生音频模型并绕过文本护栏 · `越狱与攻击` · Jiashu Zhang … Yi Yu · arXiv 2611.09351 · 2026-11-06 · [解读](https://aisafetyhot.com/items/wlnq098g3pyjp61oup27bqr5x)
4. **[Babel: Jailbreaking Safety Attention via Obfuscation Distribution Optimized Sampling](https://arxiv.org/abs/2605.17971)**  
   提出 Babel 混淆分布采样，黑盒越狱闭源 LLM 安全注意力 · `越狱与攻击` · Ziwei Wang … Yang Liu · arXiv 2605.17971 · 2026-05-18 · [解读](https://aisafetyhot.com/items/u0y6zdur82m66vnxykutn757h)
5. **[Divide, Consult, Conquer: Capability Laundering Through Aligned LLMs](https://arxiv.org/abs/2609.15383v1)**  
   提出能力洗钱攻击，拆分任务向对齐模型套取能力 · `越狱与攻击` · Mark Russinovich … Ahmed Salem · arXiv 2609.15383 · 2026-09-14 · [解读](https://aisafetyhot.com/items/ap5tbrnbbw61z3duinryi8wbi)
6. **[Automatic Red Teaming for Implicit Vulnerabilities of Text-to-Image Models](https://arxiv.org/abs/2609.06094v1)**  
   提出 AdvPIE，在黑盒下搜索表面无害却生成有害图像的提示 · `越狱与攻击` · Chang Ma … Jindong Gu · arXiv 2609.06094 · 2026-09-05 · [解读](https://aisafetyhot.com/items/vzefxwismqfzc9di4ag1uh894)
7. **[Trust Me, I'm Your Developer: Self-Issued Authentication in Large Language Models](https://arxiv.org/abs/2609.03247v1)**  
   提出 MIPC 与 CFA，观察模型自拟测验后接受开发者身份 · `越狱与攻击` · Syed Ghazanfar Abbas, Dongyan Xu · arXiv 2609.03247 · 2026-09-03 · [解读](https://aisafetyhot.com/items/cmzpnw9jprvm4att0hc0grygf)
8. **[Misrouter: Exploiting Routing Mechanisms for Input-Only Attacks on Mixture-of-Experts LLMs](https://arxiv.org/abs/2605.04446)**  
   提出 Misrouter，借 MoE 路由优化仅输入前缀并迁移攻击 · `越狱与攻击` · Zekun Fei … XiaoFeng Wang · arXiv 2605.04446 · 2026-05-06 · [解读](https://aisafetyhot.com/items/rv5gb9txiy76ogozfbtzg8t4f)
9. **[Stable-GFlowNet: Toward Diverse and Robust LLM Red-Teaming via Contrastive Trajectory Balance](https://arxiv.org/abs/2605.00553)**  
   提出 Stable-GFlowNet，用对比轨迹平衡训练红队策略生成多样高毒性攻击 · `越狱与攻击` · Minchan Kwon … Junmo Kim · arXiv 2605.00553 · 2026-05-01 · [解读](https://aisafetyhot.com/items/te4gw6bpri9wzqp71y1hicy6l)
10. **[Jailbreak Foundry: From Papers to Runnable Attacks for Reproducible Benchmarking](https://openreview.net/forum?id=BSi2mfMDsx)**  
   提出多智能体系统 JBF，将越狱论文自动翻译为可执行模块并统一评测，复现 30 种攻击的 ASR 平均偏差仅 +0.26 个百分点，实现跨 10 个模型的标准化基准。 · `越狱与攻击` · Zhicheng Fang … Wei Xu · ICML 2026 spotlight
11. **[Jailbreaking Frontier Foundation Models Through Intention Deception](https://arxiv.org/abs/2604.24082)**  
   提出多轮意图欺骗越狱 iDecep，用良性意图伪装引出有害内容 · `越狱与攻击` · Xinhe Wang … Yaqi Xie · arXiv 2604.24082 · 2026-04-27 · [解读](https://aisafetyhot.com/items/lii77tpeqz6p7eqxxca99l334)
12. **[Adaptive Prompt Embedding Optimization for LLM Jailbreaking](https://arxiv.org/abs/2604.24983)**  
   提出 PEO，直接优化原提示词嵌入实现白盒越狱 · `越狱与攻击` · Miles Q. Li … Ebrahim Bagheri · arXiv 2604.24983 · 2026-04-27 · [解读](https://aisafetyhot.com/items/fd8rnnvqd3q5kg2ti6fs63hml)
13. **[Jailbreaking the Matrix: Nullspace Steering for Controlled Model Subversion](https://arxiv.org/abs/2604.10326)**  
   提出 HMNS，通过注意力头掩码与零空间注入实现机制级越狱 · `越狱与攻击` · Vishal Pramanik … Sumit Kumar Jha · arXiv 2604.10326 · 2026-04-11 · [解读](https://aisafetyhot.com/items/f089wbhtzg8w53dtu6vrainbc)
14. **[Polarity Blindness in LLM Safety: A Systematic Study of Negation, Antonym Substitution, and Adversarial Framing](https://arxiv.org/abs/2610.27908)**  
   提出极性盲视探针，用否定与反义词替换绕过聊天模型安全护栏 · `越狱与攻击` · Diego Miguel Lozano … Nuria Oliver · arXiv 2610.27908 · 2026-10-20 · [解读](https://aisafetyhot.com/items/xoch8z7lovrsw6znh1bjv6ko7)
15. **[Training a General Purpose Automated Red Teaming Model](https://arxiv.org/abs/2604.23067)**  
   提出强化学习流程，训练能按任意对抗目标生成攻击的红队模型 · `越狱与攻击` · Aishwarya Padmakumar … Christopher Parisien · arXiv 2604.23067 · 2026-04-24 · [解读](https://aisafetyhot.com/items/xv2fxmfpsehzuvne1wjk8gnco)
16. **[On the Existence of Consistent Adversarial Attacks in High-Dimensional Linear Classification](https://openreview.net/forum?id=PUIivg3GrO)**  
   提出区分对抗攻击与表达能力不足所致误分类的新误差度量，给出高维二分类的精确渐近刻画，发现模型越过参数化，对保持标签的扰动越脆弱。 · `越狱与攻击` · Matteo Vilucchio … Bruno Loureiro · ICML 2026 spotlight
17. **[Multiple Turns, Short Horizons: Measuring Effective-Horizon Compression in Jailbreaks](https://arxiv.org/abs/2610.22928)**  
   测量多轮越狱的有效视界压缩，并用短查询后缀重放续攻 · `越狱与攻击` · Zhipeng Wei … N. Benjamin Erichson · arXiv 2610.22928 · 2026-10-16 · [解读](https://aisafetyhot.com/items/xkmz0kgr6d8yttxlsa8zs4he6)
18. **[RedDarwin: Evolving Jailbreak Skills against Frontier LLMs](https://arxiv.org/abs/2610.23726)**  
   提出 REDDARWIN，将越狱方法演化为可执行技能以攻击前沿 LLM · `越狱与攻击` · Zhouyuan Ma … Xingjun Ma · arXiv 2610.23726 · 2026-10-14 · [解读](https://aisafetyhot.com/items/wd5x5gztipurgec9y4eaq1ksu)
19. **[Diagnose Before You Refine: Multi-Dimensional Judge Feedback for Query-Efficient Jailbreak Attacks](https://arxiv.org/abs/2610.19971)**  
   提出 JSB，用多维评判反馈在有限查询内优化越狱提示 · `越狱与攻击` · Yixin Tan … Rui Wen · arXiv 2610.19971 · 2026-10-14 · [解读](https://aisafetyhot.com/items/wbnhewi0o0jmeiehm11r6u51k)
20. **[Moral Combat: Exploiting Moral Foundations Theory to Jailbreak LLMs](https://arxiv.org/abs/2610.19587)**  
   提出 Moral Combat，把有害请求改写为道德义务以越狱 · `越狱与攻击` · Adel Khorramrouz … Sharon Levy · arXiv 2610.19587 · 2026-10-14 · [解读](https://aisafetyhot.com/items/bcapsgqvfeqpox3rp55aagu36)
