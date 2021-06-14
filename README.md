# geo-bert

This work will is associated with the paper "On Geodesic Distances and Contextual Embedding Compression for Text Classification".
To be presented at TextGraphs-15 at NAACL on June 11th.

## How to use: 

Either download the ipynb and run locally or run in Google Colab. The data arguments (`data_args.task_name`) can be modified to run on different datasets and there are several flags to save/load precomputed embeddings and BERT (`load_embeddings`, `load_bert`). Additionally, there are arguments to change the compressed embedding dimensions (`l_pca_dim`, `iso_dim`, ...).

## Link to paper: 

**ACL:** https://www.aclweb.org/anthology/2021.textgraphs-1.15/

**ArXiv:** https://arxiv.org/abs/2104.11295

## Bibtex:

**ACL:** 
```
@inproceedings{jha-mihata-2021-geodesic,
    title = "On Geodesic Distances and Contextual Embedding Compression for Text Classification",
    author = "Jha, Rishi  and
      Mihata, Kai",
    booktitle = "Proceedings of the Fifteenth Workshop on Graph-Based Methods for Natural Language Processing (TextGraphs-15)",
    month = jun,
    year = "2021",
    address = "Mexico City, Mexico",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2021.textgraphs-1.15",
    pages = "144--149",
    abstract = "In some memory-constrained settings like IoT devices and over-the-network data pipelines, it can be advantageous to have smaller contextual embeddings. We investigate the efficacy of projecting contextual embedding data (BERT) onto a manifold, and using nonlinear dimensionality reduction techniques to compress these embeddings. In particular, we propose a novel post-processing approach, applying a combination of Isomap and PCA. We find that the geodesic distance estimations, estimates of the shortest path on a Riemannian manifold, from Isomap{'}s k-Nearest Neighbors graph bolstered the performance of the compressed embeddings to be comparable to the original BERT embeddings. On one dataset, we find that despite a 12-fold dimensionality reduction, the compressed embeddings performed within 0.1{\%} of the original BERT embeddings on a downstream classification task. In addition, we find that this approach works particularly well on tasks reliant on syntactic data, when compared with linear dimensionality reduction. These results show promise for a novel geometric approach to achieve lower dimensional text embeddings from existing transformers and pave the way for data-specific and application-specific embedding compressions.",
}
```
