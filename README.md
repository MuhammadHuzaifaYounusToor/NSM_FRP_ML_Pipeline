# A Data-Driven Framework for Predicting Bond Strength and Failure Modes in NSM CFRP Strips

## 📄 Associated Journal Article

This repository accompanies the following peer-reviewed journal publication:

**Toor, M. H. Y., Seo, S.-Y., & Tran, H. V.**

*A Data-Driven Framework for Predicting Bond Strength and Failure Modes in NSM CFRP Strips Using Ensemble Learning and Explainable Artificial Intelligence.*

**Construction and Building Materials (2026)**

DOI:
https://doi.org/10.1016/j.conbuildmat.2026.147334
---

## Overview

Near-surface mounted (NSM) carbon fiber-reinforced polymer (CFRP) strips are widely used for strengthening reinforced concrete structures due to their superior bond performance and durability; however, accurate prediction of bond strength remains challenging because multiple failure mechanisms govern their behavior. This study investigates the bond performance of 130 NSM CFRP specimens, including 9 specimens tested experimentally and 121 collected from the literature. The experimental program consisted of pull-out tests designed to promote interface-controlled failure, where all tested specimens exhibited debonding between the CFRP and adhesive (DFA) without concrete damage. The results showed that CFRP cross-sectional dimensions, bonded area, and aspect ratio (β) significantly influence bond strength and failure behavior. A comparative evaluation of five widely used bond strength models revealed considerable prediction errors due to their inability to distinguish between different failure modes and incorporate key governing parameters. To address these limitations, a data-driven modeling framework based on an ensemble of tree-based machine learning models was developed to simultaneously predict bond strength and failure mode. The proposed model achieved an accuracy of 84.62%, along with an average experimental-to-predicted ratio of 0.995, a standard deviation of 0.079, a coefficient of variation of 0.079, and a coefficient of determination (R²) of 0.967. The results demonstrate that the proposed framework provides more accurate and consistent predictions of bond behavior than existing models, while also reliably identifying governing failure mechanisms, making it a practical tool for the analysis and design of NSM CFRP-strengthened systems.

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

- Concrete Compressive Strength
- Epoxy Shear Strength
- FRP Tensile Strength
- FRP Thickness
- FRP Width
- Groove Thickness
- Groove Width
- FRP Perimeter of the Failure Plane
- Perimeter Length of Groove
- Aspect Ratio of FRP Cross-Section
- FRP Cross-Sectional Area
- Bonded Area of FRP Strip
- Bonded Area of the Groove
- Bonded Length
- Edge Distance

The framework predicts:

1. Bond strength
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
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/MuhammadHuzaifaYounusToor/NSM_FRP_ML_Pipeline.git
cd NSM_FRP_ML_Pipeline
```

Install required packages:

```bash
pip install pandas numpy scikit-learn xgboost lightgbm shap matplotlib openpyxl
```

---

## Usage

Open the notebook:

```bash
jupyter notebook NSM_FRP_ML_Pipeline.ipynb
```

Run the notebook sequentially to:

- Train machine learning models
- Generate ensemble predictions
- Evaluate performance
- Visualize results
- Perform SHAP-based interpretation

---

## Output Visualizations

The framework generates:

- Actual vs Predicted plots
- Confusion matrices
- Cross-validation comparison plots
- Feature importance plots
- SHAP summary plots
- Ensemble model comparison figures

---

## Research Contribution

This framework addresses limitations of traditional empirical bond strength equations by integrating machine learning and SHAP-based interpretability techniques.

The proposed framework:

- Improves prediction accuracy
- Handles nonlinear relationships
- Simultaneously predicts strength and failure mode
- Provides interpretable predictions using SHAP
- Offers a flexible framework for future NSM CFRP studies

---

## Applications

Potential applications include:

- Structural retrofitting assessment
- FRP bond behavior prediction
- Structural health monitoring research
- Data-driven structural engineering studies
- Machine learning applications in civil engineering

---

## Authors

Muhammad Huzaifa Younus Toor, Soo-Yeon Seo, and Hai Van Tran

### Repository Maintainer

Muhammad Huzaifa Younus Toor  
M.S. Structural Engineering  
Korea National University of Transportation (KNUT)

### Research Interests

- Structural Health Monitoring (SHM)
- Structural Dynamics
- Acoustic Emission (AE)
- Machine Learning in Structural Engineering
- Digital Twin Frameworks
- Internet of Things (IoT)
- Non Destructive Testing
- Fiber-Reinforced Polymer (FRP) retrofitting technology

GitHub:  
https://github.com/MuhammadHuzaifaYounusToor

---

## License

This project is intended for academic and research purposes.

---

## Acknowledgment

This research was supported by the National Research Foundation of Korea (NRF) under a grant funded by the Korea government (MSIT) (No. RS-2022-NR070123).

# Citation

If you use this repository, dataset, code, or any part of this work in your research, please cite the associated journal article.

### APA

Toor, M. H. Y., Seo, S.-Y., & Tran, H. V. (2026).
*A Data-Driven Framework for Predicting Bond Strength and Failure Modes in NSM CFRP Strips Using Ensemble Learning and Explainable Artificial Intelligence.*
Construction and Building Materials.
https://doi.org/10.1016/j.conbuildmat.2026.147334

### BibTeX

@article{Toor2026,
  author = {Muhammad Huzaifa Younus Toor and Soo-Yeon Seo and Hai Van Tran},
  title = {A Data-Driven Framework for Predicting Bond Strength and Failure Modes in NSM CFRP Strips Using Ensemble Learning and Explainable Artificial Intelligence},
  journal = {Construction and Building Materials},
  year = {2026},
  doi = {10.1016/j.conbuildmat.2026.147334}
}
