# Antimicrobial Peptide Classification Using Machine Learning

A machine learning pipeline to classify antimicrobial peptides (AMPs) from non-AMP protein sequences using sequence-derived features.

## Overview
Antimicrobial peptides are a promising class of molecules against drug-resistant pathogens. This project builds a binary classifier to distinguish AMP from non-AMP sequences using physicochemical and compositional descriptors.

## Methodology
- **Dataset**: Positive (AMP) and negative (non-AMP) FASTA sequences
- **Redundancy removal**: CD-HIT at 99% sequence identity threshold
- **Feature extraction**: Amino Acid Composition (AAC), Dipeptide Composition (DPC), and Physicochemical Properties (PCP) using Pfeature
- **Feature selection**: Variance Threshold to remove low-variance features
- **Model**: Random Forest Classifier (500 estimators)
- **Evaluation**: Accuracy, Precision, Recall, F1-score, Confusion Matrix; additional benchmarking via LazyPredict

## Results
- **Test Accuracy: 71%**

## Tools & Libraries
Python, Scikit-learn, Pfeature, CD-HIT, BioPython, Pandas, NumPy
