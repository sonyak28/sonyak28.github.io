# Pediatric TBI Data Analysis

**Course:** STAT 214, Spring 2026 · UC Berkeley  
**Type:** Individual project

Analysis of the PECARN dataset to evaluate and improve clinical decision
rules for recommending CT scans in children with minor head trauma.
CT scans detect traumatic brain injuries but expose children to radiation —
this project asks when imaging is actually warranted.

## The Problem

Standard cloud detection fails over the Arctic because ice and snow surfaces
are just as bright and cold as clouds — so we need a smarter approach.
For TBI: only 0.9% of the 42,412 children in this dataset had a clinically
important injury, but 35% received CT scans. The goal is to identify who
actually needs one.

## What I Did

- Cleaned 43,399 patient records using 80+ conditional validation rules,
  handling clinical skip logic, special codes, and parent-child dependencies
- Reproduced the exact 42,412-patient cohort from Kuppermann et al. (2009)
  as a reality check on the cleaning pipeline
- Implemented three classifiers: the published PECARN clinical rule,
  logistic regression, and a decision tree

## Key Results

| Model | Sensitivity | CT Scan Rate | Missed Cases |
|---|---|---|---|
| PECARN Rule | 95.5% | 41.6% | 17 |
| Logistic Regression | 95.7% | 44.6% | 16 |
| Decision Tree | 97.1% | 24.9% | 11 |

The decision tree achieved the best balance: highest sensitivity with the
lowest CT recommendation rate — potentially thousands fewer unnecessary
scans while missing fewer serious injuries.

## Tools

Python · pandas · scikit-learn · matplotlib · LaTeX

[View Code and Report on GitHub](https://github.com/sonyak28/Pediatric-TBI-Data-Analysis)