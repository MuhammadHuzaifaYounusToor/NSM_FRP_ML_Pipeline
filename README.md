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
NSM_FRP_ML_Pipeline/
│
├── NSM_FRP_ML_Pipeline.ipynb
├── NSM_FRP_ML_Pipeline.py
├── NSM_FRP_Strength_Failure_Dataset.xlsx
├── README.md

---

## Installation

Clone the repository:

```bash
git clone https://github.com/MuhammadHuzaifaYounusToor/NSM_FRP_ML_Pipeline.git
cd NSM_FRP_ML_Pipeline


Install required packages:
pip install pandas numpy scikit-learn xgboost lightgbm shap matplotlib openpyxl


Usage

Open the notebook:
jupyter notebook NSM_FRP_ML_Pipeline.ipynb

Run the notebook sequentially to:

Train machine learning models
Generate ensemble predictions
Evaluate performance
Visualize results
Perform SHAP-based interpretation


Output Visualizations

The framework generates:

Actual vs Predicted plots
Confusion matrices
Cross-validation comparison plots
Feature importance plots
SHAP summary plots
Ensemble model comparison figures

Research Contribution

This framework addresses limitations of traditional empirical bond strength equations by integrating machine learning and explainable AI techniques.

The proposed framework:

Improves prediction accuracy
Handles nonlinear relationships
Simultaneously predicts strength and failure mode
Provides interpretable predictions using SHAP
Offers a flexible framework for future NSM CFRP studies

Applications

Potential applications include:

Structural retrofitting assessment
FRP bond behavior prediction
Structural health monitoring research
Data-driven structural engineering studies
Explainable AI in civil engineering


Author

Muhammad Huzaifa Younus Toor
M.S. Structural Engineering
Korea National University of Transportation (KNUT)

Research Interests:

Structural Health Monitoring (SHM)
Acoustic Emission (AE)
FRP Strengthening Systems
Machine Learning in Structural Engineering
Digital Twin Frameworks
Explainable Artificial Intelligence (XAI)

GitHub: https://github.com/MuhammadHuzaifaYounusToor


License
This project is intended for academic and research purposes.

Acknowledgment
This research was supported by the National Research Foundation of Korea (NRF) under a Grant funded by the Korea government (MSIT) (No. RS-2022-NR070123).
