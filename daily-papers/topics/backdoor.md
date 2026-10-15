# 后门与投毒

每日论文里归到「后门与投毒」的 4 篇，按推送日期从新到旧。

1. **[Watch your steps: Dormant Adversarial Behaviors that Activate upon LLM Finetuning](https://openreview.net/forum?id=yfM2e8Icsw)**  
   提出FAB攻击，通过元学习构造出表面良性但在下游微调后会激活潜伏对抗行为（如越狱、过度拒答）的受损模型，揭示了微调过程中的安全风险。 · `后门与投毒` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
2. **[From Poisoned to Aware: Fostering Backdoor Self-Awareness in LLMs](https://openreview.net/forum?id=lUVEQ1JRIL)**  
   用反演式强化学习让中毒模型自述其植入触发词，并据此提出缓解与检测两种防御，在五种后门攻击上优于六个基线。 · `后门与投毒` · Guangyu Shen … Xiangyu Zhang · ICML 2026 spotlight
3. **[AI Models Can Provably Hide Arbitrary Capabilities](https://arxiv.org/abs/2610.13928)**  
   提出数字锁编译，把可执行网络加密进宿主权重以隐藏任意能力 · `后门与投毒` · Andis Draguns … Christian Schroeder de Witt · arXiv 2610.13928 · 2026-10-09 · [解读](https://aisafetyhot.com/items/ylmaojlfv5xtuhigjqo7pdgtj)
4. **[Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework](https://openreview.net/forum?id=hvI3Syn2U7)**  
   揭示利用提示注入向快速响应分类器投毒的方法，通过遗漏攻击植入概念后门或引发误报，仅需1%投毒率即可使针对越狱的防御分类器失效。 · `后门与投毒` · David Huang … Chawin Sitawarin · ICML 2026 spotlight
