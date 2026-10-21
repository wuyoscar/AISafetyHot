# 隐私与数据泄露

每日论文里归到「隐私与数据泄露」的 6 篇，按推送日期从新到旧。

1. **[Exact Unlearning in Reinforcement Learning](https://openreview.net/forum?id=oLmwqIhzqj)**  
   形式化强化学习中的精确遗忘问题，提出TV稳定的RL算法，使删除用户数据后的输出与从未交互不可区分，计算成本仅为重训的一小部分，并证明其接近极小极大最优。 · `隐私与数据泄露` · Thanh Nguyen-Tang, Raman Arora · ICML 2026 spotlight
2. **[Leave My Images Alone: Preventing Multi-Modal Large Language Models from Analyzing Images via Visual Prompt Injection](https://aclanthology.org/2026.acl-long.72/)**  
   提出 ImageProtector,在图像中嵌入近乎不可见的扰动使 MLLM 拒答,在六个模型和四个数据集上有效,对部分对策仍具抵抗力。 · `隐私与数据泄露` · Zedian Shao … Neil Zhenqiang Gong · ACL 2026 long
3. **[Benchmarking Empirical Privacy Protection for Adaptations of Large Language Models](https://openreview.net/forum?id=jY7fAo9rfK)**  
   系统评估了差分隐私微调大模型在成员推断与金丝雀提取攻击下的实际隐私风险，发现分布偏移对经验隐私保护具有显著影响。 · `隐私与数据泄露` · Bartłomiej Marek … Adam Dziedzic · ICLR 2026 Oral
4. **[Gaussian certified unlearning in high dimensions: A hypothesis testing approach](https://openreview.net/forum?id=0FJYicpOj0)**  
   提出面向高维机制的ε-高斯可认证性，理论证明单步牛顿法结合高斯噪声即可同时实现隐私消除与模型精度。 · `隐私与数据泄露` · Aaradhya Pandey … Sanjeev Kulkarni · ICLR 2026 Oral
5. **[How much can language models memorize?](https://openreview.net/forum?id=bA6BgSbaUi)**  
   提出区分非预期记忆与泛化的新方法，测定GPT模型容量约为每参数3.6比特，并建立了模型容量、数据规模与成员推断之间的标度律。 · `隐私与数据泄露` · John Xavier Morris … Saeed Mahloujifar · ICML 2026 spotlight
6. **[Hubble: a Model Suite to Advance the Study of LLM Memorization](https://openreview.net/forum?id=ZfdnZhOP0k)**  
   发布开源模型套件Hubble，通过可控插入文本模拟记忆风险，揭示敏感数据频率和训练阶段对记忆的影响，为成员推断与机器遗忘提供基准。 · `隐私与数据泄露` · Johnny Wei … Robin Jia · ICLR 2026 Oral
