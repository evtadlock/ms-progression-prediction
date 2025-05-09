# Predicting Multiple Sclerosis Progression using Clinical and MRI Data

This project applies machine learning techniques to predict the progression of Multiple Sclerosis (MS) from Clinically Isolated Syndrome (CIS) to Clinically Definite MS (CDMS), using clinical and MRI data. The work was completed as a course project in data mining at Texas Woman’s University.

## Project Structure

```
ms-progression-prediction/
├── data/
│   └── ms.csv                     # Cleaned dataset
├── notebooks/
│   └── MS_Project_2_ET.ipynb      # Main analysis notebook
├── report/
│   └── Course_Project_ET.pdf      # Final written report
├── figures/
│   └── (Optional plots: ROC curves, correlation heatmaps, etc.)
├── requirements.txt               # List of Python packages
└── README.md                      # Project overview
```

## Dataset Description

- Source: Kaggle (Conversion Predictors of CIS to MS)
- Size: 273 patients
- Features include:
  - Demographics: Age, Gender, Schooling
  - Clinical variables: Initial_EDSS, Initial_Symptom, Oligoclonal_Bands
  - MRI findings: Spinal_Cord_MRI, Periventricular_MRI, Infratentorial_MRI
  - Evoked potentials: LLSSEP, VEP, BAEP
  - Target variable: group (1 = CDMS, 2 = non-CDMS)

## Methods

- Data preprocessing:
  - Mode imputation for categorical features
  - Median imputation for numerical features
  - Min-Max scaling for model compatibility
- Exploratory data analysis:
  - Correlation heatmaps
  - Pairwise plots and distribution analysis
- Classification models:
  - Support Vector Machine (SVM)
  - k-Nearest Neighbors (k-NN)
- Evaluation metrics:
  - Accuracy
  - F1-score
  - ROC-AUC

## Results Summary

- SVM (C=0.1, gamma=0.1): Accuracy = 82%, ROC-AUC = 0.94
- k-NN (k=5): Accuracy = 98%, ROC-AUC = 0.97

## Running the Notebook

To install dependencies:

```
pip install -r requirements.txt
```

To launch the notebook:

```
jupyter notebook notebooks/MS_Project_2_ET.ipynb
```

## Report

The full project write-up is available at:

`report/Course_Project_ET.pdf`

## Author

Evelyn C. Tadlock  
Texas Woman’s University  
elister@twu.edu
