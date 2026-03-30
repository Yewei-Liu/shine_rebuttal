We visualize the relationship between text quality, text length and answer F1-Score. Here we measure text quality by calculating its ppl on Qwen3-8B-Base, a pretrain version of Qwen3-8B

---

Text quality vs. F1-Score

![](ppl_analysis/2wikimultihopqa/2wikimultihopqa_ppl_f1_scatter.png)
![](ppl_analysis/hotpotqa/hotpotqa_ppl_f1_scatter.png)
![](ppl_analysis/msmarco_v1/msmarco_v1_ppl_f1_scatter.png)
![](ppl_analysis/msmarco_v2/msmarco_v2_ppl_f1_scatter.png)
![](ppl_analysis/musique/musique_ppl_f1_scatter.png)
![](ppl_analysis/squad/squad_ppl_f1_scatter.png)

The higher text quality is, the better it can be converted into LoRA.

---

Text length vs. F1-Score

![](ctx_len_analysis/2wikimultihopqa/2wikimultihopqa_ctxlen_f1_scatter.png)
![](ctx_len_analysis/hotpotqa/hotpotqa_ctxlen_f1_scatter.png)
![](ctx_len_analysis/msmarco_v1/msmarco_v1_ctxlen_f1_scatter.png)
![](ctx_len_analysis/msmarco_v2/msmarco_v2_ctxlen_f1_scatter.png)
![](ctx_len_analysis/musique/musique_ctxlen_f1_scatter.png)
![](ctx_len_analysis/squad/squad_ctxlen_f1_scatter.png)

The shorter the text is, the better it can be converted into LoRA.