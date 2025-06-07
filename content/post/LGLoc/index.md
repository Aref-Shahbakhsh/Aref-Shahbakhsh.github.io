---
title: ✅ LGLoc Paper has been Published!
summary: LGLoc as a new language model-driven graph neural network for mRNA localization!
date: 2025-05-28
authors:
  - admin
image:
  caption: 'LGLoc model overview'
---
Im happy to share that our new paper (LGLoc as a new language model-driven graph neural network for mRNA localization!)
## Abstract
The localization of mRNA is crucial for the synthesis of functional proteins and plays a significant role in cellular processes. Understanding mRNA localization can enhance applications in disease diagnosis (e.g., cancer, Alzheimer’s) and drug development. While numerous methods have been developed for this purpose, existing approaches face challenges: experimental methods are often costly and time-consuming, while computational methods may lack accuracy and efficiency. To address these limitations, we propose LGLoc, a machine learning-based approach designed to improve the accuracy of mRNA localization predictions with low computational overhead. LGLoc employs a Graph Neural Network encoder that utilizes the RNA’s secondary structure, complemented by a BERT encoder focused on the primary RNA sequence. Additionally, it integrates k-mer and nucleotide frequency-based encoders to capture essential sequence characteristics. Feature selection is conducted using an analysis of variance, and classification is performed through a one-vs-rest Naïve Bayes classifier tailored for mRNA classification. Our results indicate that LGLoc significantly outperforms existing methods, such as mRNALoc and MSLP, across key performance metrics including Accuracy, Sensitivity, Specificity, F1-score, AUC, and MCC. Notably, LGLoc achieves over 49% improvement in average F1-score and 26% in average MCC compared to mRNALoc, demonstrating its reliability and effectiveness in mRNA subcellular localization.