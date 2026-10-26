# 防御与护栏

每日论文里归到「防御与护栏」的 29 篇，按推送日期从新到旧。

1. **[The Attacker in the Mirror: Breaking Self-Consistency in Safety via Anchored Bipolicy Self-Play](https://neurips.cc/virtual/2026/poster/151513)**  
   指出自博弈红队中攻防共享参数会塌缩为自一致性、丧失对抗压力，提出在冻结基座上训练角色专属 LoRA 的 Anchored Bipolicy Self-Play，安全性提升且参数效率高 100 倍。 · `防御与护栏` · Gabriele La Malfa … Elizabeth Black · NeurIPS 2026 oral
2. **[Cooking Up Risks: Benchmarking and Reducing Food Safety Risks in Large Language Models](https://arxiv.org/abs/2604.01444)**  
   提出 FoodGuardBench 与护栏 FoodGuard-4B，评测并降低食品危害越狱 · `防御与护栏` · Weidi Luo … Muhao Chen · arXiv 2604.01444 · 2026-04-01 · [解读](https://aisafetyhot.com/items/l87krjri3x4aih5he56ob4wnj)
3. **[Surgery: Mitigating Harmful Fine-Tuning for Large Language Models via Attention Sink](https://openreview.net/forum?id=6ojsIliNF0)**  
   发现正 sink divergence 的注意力头数量随有害微调增加，据此提出 Surgery 正则化方法抑制有害模式学习，在 BeaverTails、HarmBench、SorryBench 上分别提升防御 5.90%、11.25%、9.55%。 · `防御与护栏` · Guozhi Liu … Li Shen · ICML 2026 spotlight
4. **[Safety Reconstructed: Generative Modeling via Masked Diffusion Builds Strong Safety Guardrails](https://neurips.cc/virtual/2026/poster/149672)**  
   将护栏训练改为类条件重建目标，微调 LLaDA-8B 的 LLaDA Guard 在七个安全基准上平均排名领先，校准更好（ECE 0.0875 vs 0.1384），并可将不安全提示改写为安全等价（平均 60.7% 转化率）。 · `防御与护栏` · Gert Lek … Lydia Chen · NeurIPS 2026 spotlight
5. **[Spherical Watermark: Encryption-Free, Lossless Watermarking for Diffusion Models](https://openreview.net/forum?id=2eAGrunxVz)**  
   提出免加密无损水印框架，将水印码映射到单位球面恢复高斯噪声，保持视觉保真并提升溯源性与抗攻击鲁棒性。 · `防御与护栏` · Xiaoxiao Hu … Zhenxing Qian · ICLR 2026 Oral
6. **[Concept Removal Guidance: Evidence-Calibrated Negative Guidance for Safe Diffusion Sampling](https://openreview.net/forum?id=BSDvEh7oqy)**  
   提出免训练的 CRG 方法，每步从噪声预测估计违禁概念存在度并自适应校准负引导强度，在红队基准上降低攻击成功率同时保持正常生成质量。 · `防御与护栏` · Yoonseok Choi … Kee-Eung Kim · ICML 2026 spotlight
7. **[Refusing Intent, Not Form: Wrapper-Based Intent-Group Supervision for LLM Safety](https://arxiv.org/abs/2608.13304v1)**  
   提出 WIFA 意图组监督微调，缓解包装式越狱与过度拒答 · `防御与护栏` · Ping Wu … Yi Zeng · arXiv 2608.13304 · 2026-08-13 · [解读](https://aisafetyhot.com/items/sez6mdkitgj2vmmh0afe0z599)
8. **[AdLift: Lifting Adversarial Perturbations to Safeguard 3D Gaussian Splatting Assets Against Instruction-Driven Editing](https://openreview.net/forum?id=RL565ePGHR)**  
   提出 AdLift，将有界 2D 对抗扰动提升为 3D 高斯防护，通过 Lifted PGD 优化，跨任意视角有效且不可感知地防御指令驱动的 2D 与 3DGS 编辑。 · `防御与护栏` · Ziming Hong … Tongliang Liu · ICML 2026 spotlight
9. **[Push-Pull Attentional Anchoring for Diffusion Concept Erasure](https://arxiv.org/abs/2610.27719)**  
   提出 PPAA，在交叉注意力上推拉擦除扩散模型的指定概念 · `防御与护栏` · Nattanat Chatthee … Supasorn Suwajanakorn · arXiv 2610.27719 · 2026-10-20 · [解读](https://aisafetyhot.com/items/lm181gm465y19ab8oin2itauk)
10. **[Safety Mid-Training: Internalizing LLM Safety as a Foundational Capability](https://arxiv.org/abs/2610.26809)**  
   提出 safety mid-training，在预训练与后训练之间内化安全 · `防御与护栏` · Zhengyue Zhao … Chaowei Xiao1 · arXiv 2610.26809 · 2026-10-19 · [解读](https://aisafetyhot.com/items/wfp2wlfdgxteanseiqx23rc24)
11. **[LEMON: Equivariant Learning over Attention Maps for Zero-Shot Misbehavior Monitoring on New LLMs](https://arxiv.org/abs/2610.22723)**  
   提出注意力等变监控器 LEMON，零样本监测幻觉与越狱 · `防御与护栏` · Guy Bar-Shalom … Haggai Maron · arXiv 2610.22723 · 2026-10-15 · [解读](https://aisafetyhot.com/items/ovvtanex4ex50foane563p5zl)
12. **[Concept Removal for Frontier Image Generative Models](https://openreview.net/forum?id=s7NR3XGdwq)**  
   用 transcoder 替换模型内部瓶颈层，使特定概念特征可被关闭；在 SD3.5、Flux、Infinity 上取得领先的概念移除效果，并对对抗提示保持鲁棒。 · `防御与护栏` · Aditya Kumar … Franziska Boenisch · ICML 2026 regular
13. **[Rethinking GRPO for Large Reasoning Model Safety Alignment](https://arxiv.org/abs/2610.23085)**  
   提出 Beacon，用 SSR 与 SUDA 改进推理模型的 GRPO 安全对齐 · `防御与护栏` · Jiawei Chen … Zhaoxia Yin · arXiv 2610.23085 · 2026-10-16 · [解读](https://aisafetyhot.com/items/c00tegsmue8goswm3ywr4vu7s)
14. **[The Tokens Strike Back: Safety-Aware Denoising with Directional Embedding-based Revision](https://arxiv.org/abs/2610.17636)**  
   提出 SADDER，在文本扩散去噪中按嵌入方向门控并修正 token 分布 · `防御与护栏` · Amman Yusuf … Mijung Park · arXiv 2610.17636 · 2026-10-13 · [解读](https://aisafetyhot.com/items/wya4msbotn9zey4mxb0kl8ycc)
15. **[Decoupled Safety Control: A Safety-Control Algorithm for Training-Free Safety Guidance](https://arxiv.org/abs/2610.21569)**  
   提出 DSC，在文生图采样中按当前状态路由免训练安全引导 · `防御与护栏` · Huilin Zhou … Lan Zhang · arXiv 2610.21569 · 2026-10-15 · [解读](https://aisafetyhot.com/items/p7rjwq0nm56rvtb0szt8gsmgd)
16. **[When Reasoning Is Not Enough: Proactive Inquiry for Cross-Modal Safety in Multimodal Large Language Models](https://arxiv.org/abs/2610.22068)**  
   提出 SAFE-PRO，以风险条件不确定性调度跨模态安全的主动澄清与路径优化 · `防御与护栏` · Wei Cai … Xuelong Li · arXiv 2610.22068 · 2026-10-15 · [解读](https://aisafetyhot.com/items/l63s1pb0o8n9x5cc49g697335)
17. **[Counterfactual Neighborhood Risk Fields: Evidence-Grounded Selective Safety for Vision-Language Models](https://arxiv.org/abs/2610.20679)**  
   提出 CNRF，用反事实邻域证据对视觉语言模型做选择性防御 · `防御与护栏` · Tianshi Wang … Lei Zhu · arXiv 2610.20679 · 2026-10-14 · [解读](https://aisafetyhot.com/items/dvuk045xsun0xt6nnbuh5tzpg)
18. **[Resisting Harmful Instructions through Training-Free Weight Editing](https://arxiv.org/abs/2610.21189)**  
   提出免训练权重编辑，降低模型对指定不良指令的遵从 · `防御与护栏` · Ali Ebrahimpour-Boroojeny … ChengXiang Zhai · arXiv 2610.21189 · 2026-10-15 · [解读](https://aisafetyhot.com/items/s8ncf672tvvvi7j4dbeh1nqm0)
19. **[SafeDPO: A Simple Approach to Direct Preference Optimization with Enhanced Safety](https://openreview.net/forum?id=PJdw4VBsXD)**  
   基于安全对齐目标的闭式最优解，提出仅需一个额外超参数的轻量级安全训练方法SafeDPO，无需奖励模型即可在PKU-SafeRLHF基准上显著提升模型安全性。 · `防御与护栏` · Geon-Hyeong Kim … Moontae Lee · ICLR 2026 Oral
20. **[Does a Hybrid Space-Aware Randomized Defense Improve Empirical and Certified Adversarial Robustness?](https://openreview.net/forum?id=Alelgxnwgs)**  
   提出 HySCAN，在权重与特征空间同时注入随机性，认证鲁棒性最多提升约 9.6%，经验鲁棒性提升约 5%，且不降低干净准确率。 · `防御与护栏` · Joy Dhar … Pietro Lio · ICML 2026 regular
21. **[GEM: Geometric Erasure by Contrastive Velocity Matching in Rectified Flows](https://openreview.net/forum?id=NBMCwxTRSA)**  
   针对多模态生成模型合成有害内容与深度伪造的风险，提出GEM概念擦除框架，将基于轨迹的遗忘与教师引导流匹配结合，有效抑制有害概念并保留正常生成。 · `防御与护栏` · Jonas Henry Grebe … Marcus Rohrbach · ICML 2026 spotlight
22. **[SaTPO: Text-to-Image Safety Alignment via Transition Preference Optimization](https://arxiv.org/abs/2610.19563)**  
   提出 SaTPO，用单步转移偏好优化对齐文生图模型 · `防御与护栏` · Ziyi Fang … Haijun Zhang · arXiv 2610.19563 · 2026-10-14 · [解读](https://aisafetyhot.com/items/c2bavsbi9bmvq0znzeifkomln)
23. **[AgentSafeEvo: Adversarial Co-Evolution for LLM Agent Safety](https://arxiv.org/abs/2610.19422)**  
   提出 AgentSafeEvo，协同演化对抗任务构造与安全执行以提升工具智能体稳健性 · `防御与护栏` · Chenxu Wang … Qiaosheng Zhang · arXiv 2610.19422 · 2026-10-14 · [解读](https://aisafetyhot.com/items/qk33mh8fnkkksr403x087j8c0)
24. **[CompanionSafe: From Multi-turn Safety Evaluation to Guardrails for AI Companions](https://arxiv.org/abs/2610.18095)**  
   用多轮对话评测 AI 伴侣关系安全并训练检测护栏 CompanionGuard · `防御与护栏` · Xinyang Liao … Xia Hu · arXiv 2610.18095 · 2026-10-13 · [解读](https://aisafetyhot.com/items/pj4h6slmbz7jnabmu1hj85bui)
25. **[Efficient Safety Guardrails through Latent Dual-Hypothesis Reasoning with On-Demand Trace Reconstruction](https://arxiv.org/abs/2610.18304)**  
   提出潜空间双假设提示词护栏 LR-GUARD，并支持按需重建推理轨迹 · `防御与护栏` · Md Asiful Islam … Mihai Surdeanu · arXiv 2610.18304 · 2026-10-13 · [解读](https://aisafetyhot.com/items/f3k7vkcnsdg15xpr4xyuy3kgq)
26. **[Securing Multimodal AI through Internal Information Decomposition](https://openreview.net/forum?id=GEzZIUmEqE)**  
   提出推理期防御框架FlowGuard，利用部分信息分解监测跨模态内部一致性，仅用良性数据训练单类分类器即可将多模态未知攻击的成功率从90%以上降至15%以下。 · `防御与护栏` · Jehyeok Yeon … Heng Ji · ICML 2026 spotlight
27. **[Modular Pretraining Enables Access Control](https://openreview.net/forum?id=yIubI9l3IT)**  
   提出梯度路由辅助模块预训练方法GRAM，通过推理时消融特定模块移除病毒学与网络安全等高危能力，且比事后遗忘更具抗微调恢复性。 · `防御与护栏` · Ethan Roland … Alex Cloud · ICML 2026 spotlight · [解读](https://aisafetyhot.com/items/vvki9eetl42hlsy0wectawxgn)
28. **[ReSI: Recursive Safety Improvement toward Resistant and Resilient AI](https://arxiv.org/abs/2610.12233)**  
   提出 ReSI，用自动红队与配方搜索递归改进模型安全对齐 · `防御与护栏` · Jingnan Zheng … Xiang Wang · arXiv 2610.12233 · 2026-10-08 · [解读](https://aisafetyhot.com/items/n0pl4tgv52bli3d2e5olutzbp)
29. **[Safety Alignment of LMs via Non-cooperative Games](https://openreview.net/forum?id=Bve790HQrA)**  
   提出将安全对齐建模为攻击者与防御者语言模型间的非零和博弈，通过在线强化学习联合训练，提升了防御模型的安全性与抗对抗攻击能力。 · `防御与护栏` · Anselm Paulus … Arman Zharmagambetov · ICML 2026 spotlight
