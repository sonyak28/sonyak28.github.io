# LLM Based fMRI Brain Encoding

**Course:** Statistics 214, Spring 2026 · UC Berkeley  

A language model pipeline that maps stimulus text to fMRI brain activity,
built to test how well transformer based text embeddings predict neural
response during naturalistic language processing.

## What We Did

- Built a language model pipeline using BERT variants to tokenize and embed
  stimulus text into fixed dimensional representations
- Mapped learned embeddings to fMRI voxel activity to build an encoding
  model of brain response to language
- Fine tuned models with LoRA to adapt embeddings efficiently on the
  Bridges2 HPC cluster
- Evaluated model interpretability using SHAP and LIME, and assessed data
  quality of embeddings and model outputs at each stage of the pipeline

## Tools

Python · PyTorch · BERT · LoRA · SHAP · LIME · Bridges2 HPC

[View Code on GitHub](https://github.com/sonyak28/lab-3-group-14)