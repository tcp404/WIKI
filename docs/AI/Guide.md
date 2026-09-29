https://chatgpt.com/share/6ab92c00-c994-83e8-8348-8f07c9948ec6

不要把 Transformer 想成“一个会聊天的东西”。

把它想成一个非常巨大的：

$$ f_\theta(x) $$

输入 token sequence，经过几十/上百层矩阵运算，输出一个概率分布：

$$ P(x_{next}|x_{1:n}) $$

然后整个大模型产业，其实就是围绕这个函数做了很多事情：

```
怎么让 f 更强？ -> Transformer / Scaling

怎么让 f 更便宜？ -> MoE / Quantization / KV Cache

怎么让 f 更听话？ -> SFT(Supervised Fine-Tuning) / RLHF(Reinforcement Learning from Human Feedback)

怎么让 f 更会解决复杂问题？ -> Reasoning / Test-time Compute

怎么让 f 能看图、听声音？ -> Multimodal

怎么让 f 能访问外部世界？ -> Tool Use / Agent / RAG
```

