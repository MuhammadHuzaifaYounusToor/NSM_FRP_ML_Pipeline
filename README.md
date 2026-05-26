# A-Data-Driven-Framework-for-Predicting-Bond-Strength-and-Failure-Modes-in-NSM-CFRP-Strips
This repository presents a machine learning–based framework for predicting the bond strength and failure modes of Near-Surface Mounted (NSM) CFRP strip systems in concrete structures using ensemble learning and explainable artificial intelligence (XAI).
---

## Overview

Near-Surface Mounted (NSM) CFRP strengthening systems are widely used for retrofitting reinforced concrete structures. However, predicting bond behavior and governing failure mechanisms remains challenging because of the complex interaction between CFRP strips, adhesive layers, and surrounding concrete.

This repository provides a complete machine learning pipeline for:

* Predicting ultimate bond strength
* Classifying governing failure modes
* Comparing multiple machine learning models
* Developing ensemble learning strategies
* Performing cross-validation and performance evaluation
* Applying SHAP-based explainability analysis

---

## Machine Learning Models

The notebook includes implementation and comparison of:

* Extra Trees
* Random Forest
* Gradient Boosting
* XGBoost
* LightGBM

The best-performing models are combined into an ensemble framework to improve prediction robustness and generalization.

---

## Explainable AI (XAI)

SHAP (SHapley Additive exPlanations) is used to:

* Evaluate feature importance
* Interpret model decisions
* Identify dominant parameters influencing bond behavior
* Improve transparency of the machine learning framework

---

## Dataset

The database consists of experimental and literature-based NSM CFRP strip specimens.

The dataset includes parameters such as:

* Bonded length
* CFRP width
* CFRP thickness
* Aspect ratio
* Bonded area
* Concrete strength
* Epoxy properties
* CFRP material properties

The framework predicts:

1. Ultimate bond strength
2. Governing failure mode

---

## Workflow

The notebook follows the workflow below:

1. Data loading and preprocessing
2. Feature preparation
3. Train-test split
4. Hyperparameter optimization
5. Model training
6. Cross-validation
7. Ensemble model development
8. Regression and classification evaluation
9. SHAP explainability analysis
10. Visualization of results

---

## Repository Structure

```text
├── NSM_FRP_ML_Pipeline.ipynb
├── NSM_FRP_Strength_Failure_Dataset.xlsx
├── README.md
