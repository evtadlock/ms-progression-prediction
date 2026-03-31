# MS Progression Prediction

## Overview

This project investigates the prediction of disease progression in Multiple Sclerosis (MS) patients using clinical and MRI-derived features. The objective is to evaluate how well machine learning models can identify patients at higher risk of progression and to understand which features contribute most to these predictions.

The analysis is based on patient-level clinical data and focuses on classification rather than time-to-event modeling.

---

## Research Objective

To predict the likelihood of disease progression in MS patients using structured clinical and imaging variables, and to evaluate the performance of supervised learning models in a clinical context.

---

## Data Description

The dataset contains patient-level clinical and diagnostic variables commonly used in MS research.

Features include:

- Age
- Gender
- MRI findings:
  - Periventricular lesions
  - Cortical lesions
  - Infratentorial lesions
  - Spinal cord involvement
- Oligoclonal Bands (OCB)
- Visual Evoked Potentials (VEP)
- Sensory and motor symptoms
- Initial disability score (EDSS)

Target variable:

- Disease progression status (CDMS vs Non-CDMS)

---

## Methodology

### Data Preprocessing

- Missing values were handled using appropriate imputation strategies
- Categorical variables were encoded into numeric form
- Feature selection was applied to reduce dimensionality and improve model performance

### Models Implemented

The following supervised learning models were evaluated:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

### Evaluation Metrics

Model performance was assessed using:

- Accuracy
- ROC-AUC
- F1-score

---

## Results

The Random Forest model demonstrated the strongest performance among the evaluated models, indicating that nonlinear relationships between clinical variables contribute to predicting MS progression.

Key contributing features included:

- MRI-based findings
- Age
- Immunological markers such as Oligoclonal Bands

---

## Clinical Interpretation

The results suggest that structural MRI findings and clinical indicators are important predictors of disease progression in MS.

These findings align with clinical understanding of MS, where lesion location and early neurological indicators are associated with disease trajectory.

Predictive modeling in this context may support earlier identification of high-risk patients and inform treatment decisions.

---

## Key Takeaways

- Machine learning models can effectively classify MS progression using clinical data
- MRI-derived features play a significant role in predictive performance
- Model interpretability is essential for clinical relevance

---

## Repository Structure

``` id="yyxfy2"
.
├── data/
├── notebooks/
├── results/
├── README.md
