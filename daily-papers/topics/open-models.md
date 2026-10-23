# 开源模型与权重安全

每日论文里归到「开源模型与权重安全」的 3 篇，按推送日期从新到旧。

1. **[GoodDiffusion: Proactive Copyright Protection for Diffusion Bridge Models via Learnable Sample-specific Signatures](https://openreview.net/forum?id=wkV9jSqwa9)**  
   借鉴后门机制将授权内化进生成过程，授权签名可正常生成、未授权输入被拒绝，并用可学习签名网络防止替代签名被梯度优化恢复。 · `开源模型与权重安全` · Shixi Qin … Qingming Huang · ICML 2026 spotlight
2. **[LLM Fingerprinting via Semantically Conditioned Watermarks](https://openreview.net/forum?id=t38nZqqi3Z)**  
   提出用语义域触发、弥散于回复中的统计水印替代固定查询-应答式指纹，隐蔽且能抵御微调、量化等常见部署操作，用于验证模型所有权。 · `开源模型与权重安全` · Thibaud Gloaguen … Martin Vechev · ICLR 2026 Oral
3. **[Every Language Model Has a Forgery-Resistant Signature](https://openreview.net/forum?id=vLFqOoMBol)**  
   发现语言模型输出位于高维椭圆面上，构成难以伪造的天然模型签名，可用于识别输出来源并提出类似对称密钥认证的输出验证协议。 · `开源模型与权重安全` · Matthew Finlayson … Swabha Swayamdipta · ICLR 2026 Oral
