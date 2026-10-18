# 防御与护栏

每日论文里归到「防御与护栏」的 16 篇，按推送日期从新到旧。

1. **[The Tokens Strike Back: Safety-Aware Denoising with Directional Embedding-based Revision](https://arxiv.org/abs/2610.17636)**  
   提出 SADDER，在文本扩散去噪中按嵌入方向门控并修正 token 分布 · `防御与护栏` · Amman Yusuf … Mijung Park · arXiv 2610.17636 · 2026-10-13 · [解读](https://aisafetyhot.com/items/wya4msbotn9zey4mxb0kl8ycc)
2. **[Decoupled Safety Control: A Safety-Control Algorithm for Training-Free Safety Guidance](https://arxiv.org/abs/2610.21569)**  
   提出 DSC，在文生图采样中按当前状态路由免训练安全引导 · `防御与护栏` · Huilin Zhou … Lan Zhang · arXiv 2610.21569 · 2026-10-15 · [解读](https://aisafetyhot.com/items/p7rjwq0nm56rvtb0szt8gsmgd)
3. **[When Reasoning Is Not Enough: Proactive Inquiry for Cross-Modal Safety in Multimodal Large Language Models](https://arxiv.org/abs/2610.22068)**  
   提出 SAFE-PRO，以风险条件不确定性调度跨模态安全的主动澄清与路径优化 · `防御与护栏` · Wei Cai … Xuelong Li · arXiv 2610.22068 · 2026-10-15 · [解读](https://aisafetyhot.com/items/l63s1pb0o8n9x5cc49g697335)
4. **[Counterfactual Neighborhood Risk Fields: Evidence-Grounded Selective Safety for Vision-Language Models](https://arxiv.org/abs/2610.20679)**  
   提出 CNRF，用反事实邻域证据对视觉语言模型做选择性防御 · `防御与护栏` · Tianshi Wang … Lei Zhu · arXiv 2610.20679 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dvuk045xsun0xt6nnbuh5tzpg)
5. **[Resisting Harmful Instructions through Training-Free Weight Editing](https://arxiv.org/abs/2610.21189)**  
   提出免训练权重编辑，降低模型对指定不良指令的遵从 · `防御与护栏` · Ali Ebrahimpour-Boroojeny … ChengXiang Zhai · arXiv 2610.21189 · 2026-10-15 · [解读](https://aisafetyhot.com/items/s8ncf672tvvvi7j4dbeh1nqm0)
6. **[SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety](https://openreview.net/forum?id=PJdw4VBsXD)**  
   基于安全对齐目标的闭式最优解，提出仅需一个额外超参数的轻量级安全训练方法SafeDPO，无需奖励模型即可在PKU-SafeRLHF基准上显著提升模型安全性。 · `防御与护栏` · Geon-Hyeong Kim … Moontae Lee · ICLR 2026 Oral
7. **[Does a Hybrid Space-Aware Randomized Defense Improve Empirical and Certified Adversarial Robustness?](https://openreview.net/forum?id=Alelgxnwgs)**  
   提出 HySCAN，在权重与特征空间同时注入随机性，认证鲁棒性最多提升约 9.6%，经验鲁棒性提升约 5%，且不降低干净准确率。 · `防御与护栏` · Joy Dhar … Pietro Lio · ICML 2026 regular
8. **[GEM: Geometric Erasure by Contrastive Velocity Matching in Rectified Flows](https://openreview.net/forum?id=NBMCwxTRSA)**  
   针对多模态生成模型合成有害内容与深度伪造的风险，提出GEM概念擦除框架，将基于轨迹的遗忘与教师引导流匹配结合，有效抑制有害概念并保留正常生成。 · `防御与护栏` · Jonas Henry Grebe … Marcus Rohrbach · ICML 2026 spotlight
9. **[SaTPO: Text-to-Image Safety Alignment via Transition Preference Optimization](https://arxiv.org/abs/2610.19563)**  
   提出 SaTPO，用单步转移偏好优化对齐文生图模型 · `防御与护栏` · Ziyi Fang … Haijun Zhang · arXiv 2610.19563 · 2026-10-14 · [解读](https://aisafetyhot.com/items/c2bavsbi9bmvq0znzeifkomln)
10. **[AgentSafeEvo: Adversarial Co-Evolution for LLM Agent Safety](https://arxiv.org/abs/2610.19422)**  
   提出 AgentSafeEvo，协同演化对抗任务构造与安全执行以提升工具智能体稳健性 · `防御与护栏` · Chenxu Wang … Qiaosheng Zhang · arXiv 2610.19422 · 2026-10-14 · [解读](https://aisafetyhot.com/items/qk33mh8fnkkksr403x087j8c0)
11. **[CompanionSafe: From Multi-turn Safety Evaluation to Guardrails for AI Companions](https://arxiv.org/abs/2610.18095)**  
   用多轮对话评测 AI 伴侣关系安全并训练检测护栏 CompanionGuard · `防御与护栏` · Xinyang Liao … Xia Hu · arXiv 2610.18095 · 2026-10-13 · [解读](https://aisafetyhot.com/items/pj4h6slmbz7jnabmu1hj85bui)
12. **[Efficient Safety Guardrails through Latent Dual-Hypothesis Reasoning with On-Demand Trace Reconstruction](https://arxiv.org/abs/2610.18304)**  
   提出潜空间双假设提示词护栏 LR-GUARD，并支持按需重建推理轨迹 · `防御与护栏` · Md Asiful Islam … Mihai Surdeanu · arXiv 2610.18304 · 2026-10-13 · [解读](https://aisafetyhot.com/items/f3k7vkcnsdg15xpr4xyuy3kgq)
13. **[Securing Multimodal AI through Internal Information Decomposition](https://openreview.net/forum?id=GEzZIUmEqE)**  
   提出推理期防御框架FlowGuard，利用部分信息分解监测跨模态内部一致性，仅用良性数据训练单类分类器即可将多模态未知攻击的成功率从90%以上降至15%以下。 · `防御与护栏` · Jehyeok Yeon … Heng Ji · ICML 2026 spotlight
14. **[Modular Pretraining Enables Access Control](https://openreview.net/forum?id=yIubI9l3IT)**  
   提出梯度路由辅助模块预训练方法GRAM，通过推理时消融特定模块移除病毒学与网络安全等高危能力，且比事后遗忘更具抗微调恢复性。 · `防御与护栏` · Ethan Roland … Alex Cloud · ICML 2026 spotlight · [解读](https://aisafetyhot.com/items/vvki9eetl42hlsy0wectawxgn)
15. **[ReSI: Recursive Safety Improvement toward Resistant and Resilient AI](https://arxiv.org/abs/2610.12233)**  
   提出 ReSI，用自动红队与配方搜索递归改进模型安全对齐 · `防御与护栏` · Jingnan Zheng … Xiang Wang · arXiv 2610.12233 · 2026-10-08 · [解读](https://aisafetyhot.com/items/n0pl4tgv52bli3d2e5olutzbp)
16. **[Safety Alignment of LMs via Non-cooperative Games](https://openreview.net/forum?id=Bve790HQrA)**  
   提出将安全对齐建模为攻击者与防御者语言模型间的非零和博弈，通过在线强化学习联合训练，提升了防御模型的安全性与抗对抗攻击能力。 · `防御与护栏` · Anselm Paulus … Arman Zharmagambetov · ICML 2026 spotlight
