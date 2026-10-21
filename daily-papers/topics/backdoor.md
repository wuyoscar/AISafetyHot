# 后门与投毒

每日论文里归到「后门与投毒」的 9 篇，按推送日期从新到旧。

1. **[Adversarial Benchmarks and BenchDoor Attacks: Exploiting Benchmark Incentives for Backdoor Attacks](https://arxiv.org/abs/2610.27533)**  
   提出 BenchDoor，用脏标签投毒使被采纳数据既抬高基准分又植入后门 · `后门与投毒` · Yixin Wu … Tadayoshi Kohno · arXiv 2610.27533 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ipnmbz6zrzwn0ytajr7zgxusj)
2. **[You Are the Trigger: Speaker-Activated Backdoors](https://arxiv.org/abs/2610.27210)**  
   用 SAB 将目标说话人的自然语音设为后门触发器 · `后门与投毒` · Nataša Krčo … Yves-Alexandre de Montjoye · arXiv 2610.27210 · 2026-10-19 · [解读](https://aisafetyhot.com/items/wejc7tsr3dljp5gsvrv4lv4ju)
3. **[RAGLeak: Supply-Chain Privacy Backdoors in Retrieval-Augmented Generation](https://arxiv.org/abs/2610.25937)**  
   提出 RAGLeak，用投毒微调植入可逆混淆后门以泄露 RAG 检索文档 · `后门与投毒` · Yuchen Chen … Zhenyu Chen · arXiv 2610.25937 · 2026-10-19 · [解读](https://aisafetyhot.com/items/glsembbaas25wl0zhoni27a5w)
4. **[ShadowFPT: Backdooring Federated Prompt Tuning via Shadow Triggers](https://arxiv.org/abs/2610.22871)**  
   提出 ShadowFPT，用影子触发器在联邦提示微调中植入定向后门 · `后门与投毒` · Kun Zhai … Xingjun Ma · arXiv 2610.22871 · 2026-10-16 · [解读](https://aisafetyhot.com/items/tl0z3j1aupwtk5bf9736kehki)
5. **[Clean Data Can Still Carry Backdoors: Support-Persistent Backdoors for Model Reuse](https://arxiv.org/abs/2610.21208)**  
   提出 DAR 支撑持久后门，使干净蒸馏后的学生仍可被触发 · `后门与投毒` · Junhoo Lee … Nojun Kwak · arXiv 2610.21208 · 2026-10-15 · [解读](https://aisafetyhot.com/items/xj6g2176eqwed1j78j7yy7yjc)
6. **[Watch your steps: Dormant Adversarial Behaviors that Activate upon LLM Finetuning](https://openreview.net/forum?id=yfM2e8Icsw)**  
   提出FAB攻击，通过元学习构造出表面良性但在下游微调后会激活潜伏对抗行为（如越狱、过度拒答）的受损模型，揭示了微调过程中的安全风险。 · `后门与投毒` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
7. **[From Poisoned to Aware: Fostering Backdoor Self-Awareness in LLMs](https://openreview.net/forum?id=lUVEQ1JRIL)**  
   用反演式强化学习让中毒模型自述其植入触发词，并据此提出缓解与检测两种防御，在五种后门攻击上优于六个基线。 · `后门与投毒` · Guangyu Shen … Xiangyu Zhang · ICML 2026 spotlight
8. **[AI Models Can Provably Hide Arbitrary Capabilities](https://arxiv.org/abs/2610.13928)**  
   提出数字锁编译，把可执行网络加密进宿主权重以隐藏任意能力 · `后门与投毒` · Andis Draguns … Christian Schroeder de Witt · arXiv 2610.13928 · 2026-10-09 · [解读](https://aisafetyhot.com/items/ylmaojlfv5xtuhigjqo7pdgtj)
9. **[Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework](https://openreview.net/forum?id=hvI3Syn2U7)**  
   揭示利用提示注入向快速响应分类器投毒的方法，通过遗漏攻击植入概念后门或引发误报，仅需1%投毒率即可使针对越狱的防御分类器失效。 · `后门与投毒` · David Huang … Chawin Sitawarin · ICML 2026 spotlight
