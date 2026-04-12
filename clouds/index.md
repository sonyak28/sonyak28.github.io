# Arctic Cloud Detection

**Course:** STAT 214, Spring 2026 · UC Berkeley  
**Type:** Group project

Detection of clouds in polar satellite imagery using NASA's Multi-angle
Imaging SpectroRadiometer (MISR). Standard cloud detection fails over the
Arctic because ice and snow are just as bright and cold as the clouds above
them — this project uses multi-angle radiance patterns and transfer learning
to tell them apart.

## The Problem

With only 3 expert-labeled images out of 164 total, supervised learning
alone is not enough. We pre-trained an autoencoder on the 161 unlabeled
images to learn what Arctic pixels look like, then used those learned
representations as features for classification.

## What We Did

- EDA across 18.9 million pixels spanning 164 satellite images
- Engineered local 3×3 patch features (mean SD, std AN, mean NDAI)
  to capture spatial texture beyond pointwise measurements
- Pre-trained a patch autoencoder on 18.6M unlabeled patches, then
  fine-tuned on the 3 labeled images without using labels
- Trained five classifiers: logistic regression, LDA, QDA (replicating
  Shi et al. 2008), random forest, and XGBoost

## Key Results

| Model | Validation AUC | Cloud Recall |
|---|---|---|
| XGBoost | 0.990 | 0.99 |
| Random Forest | 0.986 | 0.96 |
| QDA (replicates paper) | 0.981 | 0.98 |

XGBoost achieved a final test AUC of 0.984. Our QDA — which mirrors the
method from Shi et al. — reached 94.6% validation accuracy vs. the paper's
91.8%, using the same approach but with richer autoencoder features.
Transfer learning was the main driver: embeddings pushed leave-one-image-out
AUC from 0.832 to 0.974.

## Tools

Python · PyTorch · XGBoost · scikit-learn · matplotlib

[View Code and Report on GitHub](https://github.com/sonyak28/arctic-cloud-detection)