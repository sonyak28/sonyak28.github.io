# Sonya Kiskachi

**Statistics · NLP · Geospatial · Machine Learning**

MS Statistics · UC Berkeley · May 2026

[sonyak@berkeley.edu](mailto:sonyak@berkeley.edu) · [LinkedIn](https://www.linkedin.com/in/sonya-kiskachi/) · [GitHub](https://github.com/sonyak28)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=flat&logo=python&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white)

```{image} headshot.jpg
:width: 140px
:align: right
:alt: Sonya Kiskachi
```

I am a statistician and data scientist with experience across industry and
research. I recently completed my MS in Statistics at UC Berkeley, where my
work spanned clinical machine learning, satellite remote sensing, and urban
equity analysis. I am currently a research collaborator at The Nature
Conservancy California, applying deep learning and statistical post-processing
to improve daily streamflow estimates across California's stream network.

Before my master's, I spent two years at Wells Fargo as a Data Scientist and
NLP Engineer, building fraud detection pipelines, topic models for customer
complaint analysis, and company-wide sentiment dashboards. Prior to that I
interned at Apple on software quality and anomaly detection.

I hold a BA in Data Science with a Geospatial Science emphasis from UC Berkeley
(2023), where I also served as Lead Undergraduate Student Instructor for
Foundations of Data Science, the largest course in UC history. I am drawn to
problems where the stakes are real — whether that is understanding how water
moves through a landscape, reducing unnecessary radiation exposure in pediatric
emergency care, or measuring amenity access for transit-dependent communities
in the Bay Area.

---

## Experience

**The Nature Conservancy California** · Data Science Research Collaborator · *Summer 2026*
Applying proportional rescaling to combine an LSTM daily streamflow model with
a trusted monthly hydrological baseline, improving streamflow estimates across
~155,000 California stream segments.
`Python` `PyTorch` `Hydrology` `Time Series` · [Project Dashboard](https://sonyak28.github.io/tnc-streamflow/)

---

**Wells Fargo** · Data Scientist & NLP Engineer · *Jul 2023 – Jul 2025*
Built production NLP pipelines (FLAN-T5, BERT) for customer transcript
classification, automated compliance control reporting, and reduced frontline
QC workload by 70%.
`Python` `BERT` `FLAN-T5` `Snowflake` `SQL`

---

**Apple** · Machine Learning Intern · *Summer 2022*
Applied anomaly detection and k-means clustering to improve internal bug
discovery tooling; built custom KPIs to quantify test coverage across
software quality pipelines.
`Python` `scikit-learn` `Anomaly Detection`

---

## Projects

**[Pediatric TBI Data Analysis](tbi/index.md)**
Cleaned 43,399 clinical records and built classifiers to improve CT scan
decision rules for children with head trauma. Decision tree achieved 97.1%
sensitivity at less than half the scan rate of the clinical standard.
`Python` `scikit-learn` `pandas`

---

**[Arctic Cloud Detection](clouds/index.md)**
Detected clouds in polar satellite imagery where standard methods fail, using
transfer learning from 161 unlabeled images. XGBoost + autoencoder embeddings
reached AUC 0.990 vs. the paper benchmark's 91.8% accuracy.
`Python` `PyTorch` `XGBoost`

---

**[Bay Area Transit Equity Analysis](city/index.md)**
Analyzed amenity access disparities at 79 BART and Caltrain stations,
examining whether peripheral stations underserve transit-dependent communities
using permutation tests, Gini coefficients, and spatial analysis.
`Python` `geopandas` `Census API`