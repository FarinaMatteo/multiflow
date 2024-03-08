# Description
Official implementation of the paper "MULTIFLOW: Shifting Towards Task-Agnostic Vision-Language Pruning", accepted at CVPR 2024.  
Authors: [Matteo Farina](https://scholar.google.com/citations?user=SxQwDD8AAAAJ&hl=it&oi=ao), [Massimiliano Mancini](https://scholar.google.com/citations?hl=it&user=bqTPA8kAAAAJ), [Elia Cunegatti](https://scholar.google.com/citations?hl=it&user=a2JJRjMAAAAJ), [Gaowen Liu](https://scholar.google.com/citations?hl=it&user=NIv_aeQAAAAJ), [Giovanni Iacca](https://scholar.google.com/citations?hl=it&user=qSw6YfcAAAAJ), [Elisa Ricci](https://scholar.google.com/citations?hl=it&user=xf1T870AAAAJ).

# Updates 🗞️
[March 8th, 2024] - Public Repo online, the code will be out very soon!  


# Features Preview 🧞‍♀️
In addition to the implementation of `MULTIFLOW`, we will release various pruners with a shared access interface. Model dependency will be abstracted, such that instances of `torch.nn.Module` can be pruned by implementing minor user-defined modular functions (*e.g.*, how to forward a batch of data with the model you want to prune). The list of pruners includes:  
1. `SNIP`, from [Lee *et al.*](https://arxiv.org/abs/1810.02340);
2. `IterSNIP`, from [De Jorge *et al.*](https://arxiv.org/abs/2006.09081);
3. `OMP` and `LocalMP`: One-shot and Layer-wise Magnitude Pruning;
4. `LAMP`: Layer-Adaptive Sparsity for Magnitude Pruning, from [Lee *et al.*](https://arxiv.org/abs/2010.07611);
5. `CHITA`: Combinatorial Hessian-free Iterative Thresholding Algorithm, from [Benbaki *et al.*](https://arxiv.org/pdf/2302.14623.pdf);
6. `CHITA++`, *i.e.*, the iterative version of (5), also from [Benbaki *et al.*](https://arxiv.org/pdf/2302.14623.pdf);


The code for dense or sparse model finetuning for **Image-Text Retrieval**, **Image Captioning**, and **Visual Question Answering** will also be released. 
