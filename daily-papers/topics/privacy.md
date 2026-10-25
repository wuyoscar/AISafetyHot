# 隐私与数据泄露

每日论文里归到「隐私与数据泄露」的 10 篇，按推送日期从新到旧。

1. **[CLIOPATRA: Extracting Private Information from LLM Insights](https://neurips.cc/virtual/2026/poster/152543)**  
   作者称首个针对隐私保护型 LLM 洞察系统的攻击，通过注入恶意对话击穿多层防护，在 Anthropic Clio 上以近 100% 精度、最高 65% 的比例提取目标用户医疗聊天内容。 · `隐私与数据泄露` · Meenatchi Sundaram Muthu Selva Annamalai … Peter Kairouz · NeurIPS 2026 oral
2. **[We Should Distinguish Unlearning From Untraining](https://neurips.cc/virtual/2026/poster/140062)**  
   立场论文指出机器遗忘实际包含两种不同问题：撤销特定样本训练影响的Untraining与移除整个子分布概念的Unlearning，混淆二者会导致指标误用。 · `隐私与数据泄露` · Eleni Triantafillou … Georgios Kaissis · NeurIPS 2026 oral
3. **[Unlearning That Lasts: Utility-Preserving, Robust, and Almost Irreversible Forgetting in LLMs](https://neurips.cc/virtual/2026/poster/149440)**  
   提出以JS散度为目标的JensUn遗忘方法和新数据集LPF，改进评估显示许多现有遗忘方法实际效果不如此前认为的那样好。 · `隐私与数据泄露` · Naman Deep Singh … Matthias Hein · NeurIPS 2026 spotlight
4. **[Asymptotic Optimality of the High-Dimensional Gaussian Mechanism and Improved Low-Dimensional Mechanisms for Differential Privacy](https://openreview.net/forum?id=82Wosp2Iu1)**  
   证明高维极限下无加噪机制能渐近优于高斯机制的隐私-效用权衡，并提出球面广义Gamma机制族，其中部分成员在低维设定下优于高斯和ℓ2机制。 · `隐私与数据泄露` · Yu Wei … Antigoni Polychroniadou · ICML 2026 spotlight
5. **[Exact Unlearning in Reinforcement Learning](https://openreview.net/forum?id=oLmwqIhzqj)**  
   形式化强化学习中的精确遗忘问题，提出TV稳定的RL算法，使删除用户数据后的输出与从未交互不可区分，计算成本仅为重训的一小部分，并证明其接近极小极大最优。 · `隐私与数据泄露` · Thanh Nguyen-Tang, Raman Arora · ICML 2026 spotlight
6. **[Leave My Images Alone: Preventing Multi-Modal Large Language Models from Analyzing Images via Visual Prompt Injection](https://aclanthology.org/2026.acl-long.72/)**  
   提出 ImageProtector,在图像中嵌入近乎不可见的扰动使 MLLM 拒答,在六个模型和四个数据集上有效,对部分对策仍具抵抗力。 · `隐私与数据泄露` · Zedian Shao … Neil Zhenqiang Gong · ACL 2026 long
7. **[Benchmarking Empirical Privacy Protection for Adaptations of Large Language Models](https://openreview.net/forum?id=jY7fAo9rfK)**  
   系统评估了差分隐私微调大模型在成员推断与金丝雀提取攻击下的实际隐私风险，发现分布偏移对经验隐私保护具有显著影响。 · `隐私与数据泄露` · Bartłomiej Marek … Adam Dziedzic · ICLR 2026 Oral
8. **[Gaussian certified unlearning in high dimensions: A hypothesis testing approach](https://openreview.net/forum?id=0FJYicpOj0)**  
   提出面向高维机制的ε-高斯可认证性，理论证明单步牛顿法结合高斯噪声即可同时实现隐私消除与模型精度。 · `隐私与数据泄露` · Aaradhya Pandey … Sanjeev Kulkarni · ICLR 2026 Oral
9. **[How much can language models memorize?](https://openreview.net/forum?id=bA6BgSbaUi)**  
   提出区分非预期记忆与泛化的新方法，测定GPT模型容量约为每参数3.6比特，并建立了模型容量、数据规模与成员推断之间的标度律。 · `隐私与数据泄露` · John Xavier Morris … Saeed Mahloujifar · ICML 2026 spotlight
10. **[Hubble: a Model Suite to Advance the Study of LLM Memorization](https://openreview.net/forum?id=ZfdnZhOP0k)**  
   发布开源模型套件Hubble，通过可控插入文本模拟记忆风险，揭示敏感数据频率和训练阶段对记忆的影响，为成员推断与机器遗忘提供基准。 · `隐私与数据泄露` · Johnny Wei … Robin Jia · ICLR 2026 Oral
