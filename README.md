# Breast Cancer Classification using Decision Trees

## Overview

This project explores the use of machine learning models to classify breast cancer tumors as **malignant** or **benign** based on diagnostic features extracted from medical data.

The study focuses on the use of **decision tree algorithms** and compares their performance with other classification models such as **random forest** and **logistic regression**.

The goal of the project is to evaluate how interpretable machine learning models can support medical decision-making and improve diagnostic classification.

The full paper is available in this repository.

---

## Problem

Breast cancer diagnosis requires distinguishing between **malignant** and **benign** tumors.  
Machine learning models can assist in this task by identifying patterns in cell features obtained from diagnostic tests.

This project investigates how effectively **decision tree models** can classify breast cancer cells and compares their performance with other machine learning approaches. :contentReference[oaicite:0]{index=0}

---

## Dataset

The analysis uses the **Breast Cancer Wisconsin dataset**, an open-source dataset containing diagnostic measurements of breast mass samples.

The dataset includes **32 attributes**, describing characteristics of cell nuclei extracted from medical imaging data. :contentReference[oaicite:1]{index=1}

Examples of features include:

- radius_mean
- texture_mean
- perimeter_mean
- area_mean
- concavity_mean
- symmetry_mean
- fractal_dimension_mean

These variables describe physical characteristics of the tumor that help determine whether it is malignant or benign.

---

## Methods

Models were implemented using **WEKA** and evaluated using **10-fold cross-validation**.

The following models were compared:

### Decision Tree Algorithms
- REPTree
- J48
- J48 with pruning

### Other Classification Models
- Random Forest
- Logistic Regression

Confusion matrices and ROC curves were used to evaluate and compare model performance. :contentReference[oaicite:2]{index=2}

---

## Results

Among the decision tree models:

- **J48** achieved higher accuracy than **REPTree**
- **Pruning** simplified the J48 model while maintaining similar accuracy

However, ensemble and statistical models achieved higher performance overall.

Model accuracy comparison:

| Model | Accuracy |
|------|------|
| REPTree | 92.44% |
| J48 | 93.15% |
| J48 (Pruned) | 93.67% |
| Random Forest | 95.96% |
| Logistic Regression | 94.20% |

Random forest achieved the highest classification accuracy, while decision trees provided more interpretable models. :contentReference[oaicite:3]{index=3}

---

## Key Insight

Although decision trees are slightly less accurate than ensemble models, they offer strong **interpretability**, which can be valuable in clinical decision support systems.

A pruned J48 model was able to reduce model complexity while maintaining similar predictive performance.

---

## Repository Structure
```text
breast-cancer-classification/
├── README.md
└── Decision Tree Paper - Yeju Seol.pdf
```

---

## Tools

WEKA  
Decision Trees (REPTree, J48)  
Random Forest  
Logistic Regression  
