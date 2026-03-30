# Ablation Study on M2PTransformer Architecture Design

![m2ptransformer](pretrain_ppl_m2ptransformer.png)

We perform ablation studies comparing our M2P Transformer against alternative architecture designs to demonstrate the effectiveness of our design.

- Linear small: 2 layer linear layer with hidden size 8192
- Linear: 8 layer linear layer with hidden size 8192, nearly same number of parameters as M2P Transformer
- Linear Residual: Linear with residual connection.
- Only Horizontal: M2P Transformer but with 4 token transformer.
- Origin: Origin M2P Transformer with 2 token transformer and 2 layer transformer.

The results shows Transformer architectures generally performance much better than linear(projection) architectures. Origin and Only Horizontal performance similarly in the end, but Origin converges faster in early stage.
