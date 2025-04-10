---
title: ✅ ParaAntiProt Paper has been Published!
summary: Paratope prediction using language models!
date: 2024-11-22
authors:
  - admin
image:
  caption: 'ParaAntiProt model overview'
---
Im happy to share that our new paper (ParaAntiProt Provides Paratope Prediction Using Antibody and Protein Language Models) has been Published!
## Abstract
Efficiently predicting the paratope holds immense potential for enhancing antibody design, treating cancers and other serious diseases, and advancing personalized medicine. Although traditional methods are highly accurate, they are often time-consuming, labor-intensive, and reliant on 3D structures, restricting their broader use. On the other hand, machine learning-based methods, besides relying on structural data, entail descriptor computation, consideration of diverse physicochemical properties, and feature engineering. Here, we develop a deep learning-assisted prediction method for paratope identification, relying solely on amino acid sequences and being antigen-agnostic. Built on the ProtTrans architecture, and utilizing pre- trained protein and antibody language models, we extract efficient embeddings for predicting paratope. By incorporating positional encoding for Complementarity Determining Regions, our model gains a deeper structural understanding, achieving remarkable performance with a 0.904 ROC AUC, 0.701 F1-score, and 0.585 MCC on benchmark datasets. In addition to yielding accurate antibody paratope predictions, our method exhibits strong performance in predicting nanobody paratope, achieving a ROC AUC of 0.912 and a PR AUC of 0.665 on the nanobody dataset. Notably, our approach outperforms structure-based prediction methods, boasting a PR AUC of 0.731. Various conducted ablation studies, which elaborate on the impact of each part of the model on the prediction task, show that the improvement in prediction performance by applying CDR positional encoding together with CNNs depends on the specific protein and antibody language models used. These results highlight the potential of our method to advance disease understanding and aid in the discovery of new diagnostics and antibody therapies.

Keywords: Paratope Prediction; Antibody Language Models; Protein Language Models; Complementarity Determining Regions; Deep Learning