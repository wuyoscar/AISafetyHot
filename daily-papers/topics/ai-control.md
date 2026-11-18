# 监控与 AI 控制

每日论文里归到「监控与 AI 控制」的 5 篇，按推送日期从新到旧。

1. **[Are LLM Safety Judges Policy-Invariant? A Three-Principle Stress-Test](https://neurips.cc/virtual/2026/poster/139215)**  
   提出策略不变性三原则并压力测试四个智能体类安全评审，发现内容等价的策略改写可翻转最高 9.1% 的判定，18–43% 的翻转发生在无歧义案例上，并给出 Policy Invariance Score 与 Judge Card 报告协议。 · `监控与 AI 控制` · Shihao Weng … Xiaofei Xie · NeurIPS 2026 spotlight
2. **[Trusting What You Cannot See: Auditable Fine-Tuning and Inference for Proprietary AI](https://www.usenix.org/conference/usenixsecurity26/presentation/jin)**  
   提出 AFTUNE 框架，通过轻量执行记录与在 TEE 中抽样验证执行块，使客户能以适度开销审计云端大模型微调与推理是否按约定配置执行。 · `监控与 AI 控制` · Heng Jin … Wenjing Lou · USENIX Security 2026
3. **[Monitoring Monitorability](https://openreview.net/forum?id=b82fgbMVpz)**  
   提出三类评估原型与可监控性指标，发现CoT监控优于仅动作监控，更长思维链通常更可监控，追问并共享思维链可提升可监控性。 · `监控与 AI 控制` · Melody Y. Guan … Bowen Baker · ICML 2026 spotlight
4. **[Removing Sandbagging in LLMs by Training with Weak Supervision](https://openreview.net/forum?id=J4DiM8EiMJ)**  
   SFT 与 RL 结合可在弱监督下引出 sandbagging 模型的真实能力,单独使用均不可靠;但若模型能区分训练与部署,仍会继续藏拙。 · `监控与 AI 控制` · Emil Ryd … Vivek Hebbar · ICML 2026 regular
5. **[Reliable Weak-to-Strong Monitoring of LLM Agents](https://openreview.net/forum?id=WV7xIboTDK)**  
   提出 monitor red teaming 流程，在 SHADE-Arena 上压测隐蔽不良行为监控；发现 agent 知晓被监控会显著削弱检测，混合式监控设计让弱监控者能监督强 agent。 · `监控与 AI 控制` · Neil Kale … Zifan Wang · ICLR 2026 Oral
