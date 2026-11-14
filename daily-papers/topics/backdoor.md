# 后门与投毒

每日论文里归到「后门与投毒」的 15 篇，按推送日期从新到旧。

1. **[Hijacking a Trusted LLM in Real-World Quantized Deployments Only Requires a Disguised Adapter](https://arxiv.org/abs/2611.14978)**  
   提出 QHijack-LoRA 攻击，伪装适配器在全精度审计下正常、底座量化后劫持决策 · `后门与投毒` · Jiayang Li … Wanlei Zhou · arXiv 2611.14978 · 2026-11-11 · [解读](https://aisafetyhot.com/items/vqqorxzt5ywq3xyqjvqa7a6rb)
2. **[Lazare, veni foras: Reprogramming Dormant Neurons to Backdoor AI Agents](https://arxiv.org/abs/2611.15118)**  
   提出 Lazarus 权重编辑攻击，改写少数休眠神经元为 Agent 植入触发式后门 · `后门与投毒` · Yuchen Zeng … Dimitris Papailiopoulos · arXiv 2611.15118 · 2026-11-11 · [解读](https://aisafetyhot.com/items/tq0najoxw4wwosiduzl0kmtcn)
3. **[Poison-then-Hide: Finetuning-Activated Backdoor Attack on Pretrained Vision Encoders](https://arxiv.org/abs/2611.14970)**  
   提出 Poison-then-Hide 攻击，在预训练视觉编码器中植入休眠后门并经干净微调激活 · `后门与投毒` · Qixuan Jin … Marzyeh Ghassemi · arXiv 2611.14970 · 2026-11-11 · [解读](https://aisafetyhot.com/items/hu88vfrnhj363ynahhs6nq701)
4. **[Pick Your Poison: Learning to Select Poison Sets for Stronger LLM Backdoor Attacks](https://arxiv.org/abs/2609.15029v1)**  
   提出 SAILS 投毒集选择方法，用学习的集合打分器在有限预算下选出更强后门投毒集 · `后门与投毒` · Aashiq Muhamed … Matthew Jagielski · arXiv 2609.15029 · 2026-09-14 · [解读](https://aisafetyhot.com/items/tsniwhqqiiz6k3b27d7mlbfxf)
5. **[Homeopathic Learning: Diluting poisoned fine-tuning data can strengthen its effect](https://arxiv.org/abs/2611.10110)**  
   发现投毒数据混入同类干净数据后反而形成后门，提出顺势学习现象 · `后门与投毒` · Matt Clarke … Alex Cloud · arXiv 2611.10110 · 2026-11-06 · [解读](https://aisafetyhot.com/items/hbx2p5yrf6ccnihyzw481u6jt)
6. **[When Experience Becomes a Backdoor: Poisoning Self-Evolving LLM Agents via Failure-Aware Task Optimization](https://arxiv.org/abs/2611.10542)**  
   提出 BadEvolve 任务投毒框架，诱使自演化 Agent 把后门写进技能 · `后门与投毒` · Minhua Lin … Suhang Wang · arXiv 2611.10542 · 2026-11-07 · [解读](https://aisafetyhot.com/items/cy2ew721glyzs94wiolw8bnf5)
7. **[Adversarial Benchmarks and BenchDoor Attacks: Exploiting Benchmark Incentives for Backdoor Attacks](https://arxiv.org/abs/2610.27533)**  
   提出 BenchDoor，用脏标签投毒使被采纳数据既抬高基准分又植入后门 · `后门与投毒` · Yixin Wu … Tadayoshi Kohno · arXiv 2610.27533 · 2026-10-20 · [解读](https://aisafetyhot.com/items/ipnmbz6zrzwn0ytajr7zgxusj)
8. **[You Are the Trigger: Speaker-Activated Backdoors](https://arxiv.org/abs/2610.27210)**  
   用 SAB 将目标说话人的自然语音设为后门触发器 · `后门与投毒` · Nataša Krčo … Yves-Alexandre de Montjoye · arXiv 2610.27210 · 2026-10-19 · [解读](https://aisafetyhot.com/items/wejc7tsr3dljp5gsvrv4lv4ju)
9. **[RAGLeak: Supply-Chain Privacy Backdoors in Retrieval-Augmented Generation](https://arxiv.org/abs/2610.25937)**  
   提出 RAGLeak，用投毒微调植入可逆混淆后门以泄露 RAG 检索文档 · `后门与投毒` · Yuchen Chen … Zhenyu Chen · arXiv 2610.25937 · 2026-10-19 · [解读](https://aisafetyhot.com/items/glsembbaas25wl0zhoni27a5w)
10. **[ShadowFPT: Backdooring Federated Prompt Tuning via Shadow Triggers](https://arxiv.org/abs/2610.22871)**  
   提出 ShadowFPT，用影子触发器在联邦提示微调中植入定向后门 · `后门与投毒` · Kun Zhai … Xingjun Ma · arXiv 2610.22871 · 2026-10-16 · [解读](https://aisafetyhot.com/items/tl0z3j1aupwtk5bf9736kehki)
11. **[Clean Data Can Still Carry Backdoors: Support-Persistent Backdoors for Model Reuse](https://arxiv.org/abs/2610.21208)**  
   提出 DAR 支撑持久后门，使干净蒸馏后的学生仍可被触发 · `后门与投毒` · Junhoo Lee … Nojun Kwak · arXiv 2610.21208 · 2026-10-15 · [解读](https://aisafetyhot.com/items/xj6g2176eqwed1j78j7yy7yjc)
12. **[Watch your steps: Dormant Adversarial Behaviors that Activate upon LLM Finetuning](https://openreview.net/forum?id=yfM2e8Icsw)**  
   提出FAB攻击，通过元学习构造出表面良性但在下游微调后会激活潜伏对抗行为（如越狱、过度拒答）的受损模型，揭示了微调过程中的安全风险。 · `后门与投毒` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
13. **[From Poisoned to Aware: Fostering Backdoor Self-Awareness in LLMs](https://openreview.net/forum?id=lUVEQ1JRIL)**  
   用反演式强化学习让中毒模型自述其植入触发词，并据此提出缓解与检测两种防御，在五种后门攻击上优于六个基线。 · `后门与投毒` · Guangyu Shen … Xiangyu Zhang · ICML 2026 spotlight
14. **[AI Models Can Provably Hide Arbitrary Capabilities](https://arxiv.org/abs/2610.13928)**  
   提出数字锁编译，把可执行网络加密进宿主权重以隐藏任意能力 · `后门与投毒` · Andis Draguns … Christian Schroeder de Witt · arXiv 2610.13928 · 2026-10-09 · [解读](https://aisafetyhot.com/items/ylmaojlfv5xtuhigjqo7pdgtj)
15. **[Rapid Poison: Practical Poisoning Attacks Against the Rapid Response Framework](https://openreview.net/forum?id=hvI3Syn2U7)**  
   揭示利用提示注入向快速响应分类器投毒的方法，通过遗漏攻击植入概念后门或引发误报，仅需1%投毒率即可使针对越狱的防御分类器失效。 · `后门与投毒` · David Huang … Chawin Sitawarin · ICML 2026 spotlight
