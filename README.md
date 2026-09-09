# AI4D Tanzania Tourism Classification

### 2nd Place, AI4D Africa's Anglophone Research Lab Tanzania Tourism Classification Challenge

A machine learning solution for classifying the expenditure range of tourists visiting Tanzania from survey and demographic data.

The solution was developed by **AI SQUAD** and finished **2nd place** in the Zindi competition.

**Challenge:** https://zindi.africa/competitions/ai4d-lab-tanzania-tourism-classification-challenge

---

## Problem

Tourism is an important part of Tanzania's economy, but trip costs vary significantly across visitors. The challenge was to build a multiclass classification model that predicts the expenditure category of a tourist using available survey information.

A useful solution has to work with mixed data types, categorical information, demographic variables, and interactions between visitor characteristics and travel behaviour.

---

## Solution Approach

The notebook follows a competition-style machine learning workflow:

```text
Raw Survey Data
      ↓
EDA & Data Cleaning
      ↓
Feature Engineering
      ↓
Categorical Encoding / Transformation
      ↓
Cross-Validation
      ↓
CatBoost + LightGBM Experiments
      ↓
Model Selection / Tuning
      ↓
Final Predictions
```

The solution uses tree-based boosting methods that are well suited to structured tabular data.

### Models used

- **CatBoostClassifier**
- **LightGBM / LGBMClassifier**

The notebook also includes model-selection and tuning experiments using tools such as **Optuna**.

### Validation

The workflow includes **StratifiedKFold**-based validation to preserve target-distribution structure across folds and provide a more reliable estimate of generalisation performance.

---

## Repository Structure

```text
.
├── README.md
├── 2nd_placesolution_AISQUAD.ipynb   # Main 2nd-place solution notebook
└── AI4D_/                            # Competition data files
```

---

## Why This Project Matters

This project is a good example of applied tabular machine learning where model performance depends on more than simply choosing an algorithm.

The work required:

- understanding the target and class structure
- exploring mixed survey variables
- engineering useful features
- choosing validation that reflects the classification problem
- comparing strong boosting models
- iterating quickly under competition constraints

---

## Run the Notebook

The original solution was developed in Google Colab.

To reproduce it:

1. Clone the repository

```bash
git clone https://github.com/emmanuel-123tech/AI4D-Africa-s-Anglophone-Research-Lab-Tanzania-Tourism-Classification-Challenge.git
cd AI4D-Africa-s-Anglophone-Research-Lab-Tanzania-Tourism-Classification-Challenge
```

2. Open `2nd_placesolution_AISQUAD.ipynb` in Jupyter or Google Colab.

3. Install the notebook dependencies when prompted and run the cells sequentially.

---

## Result

**2nd Place** in the **AI4D Africa's Anglophone Research Lab Tanzania Tourism Classification Challenge** on Zindi.

---

## Team: AI SQUAD

- **Emmanuel Ebiendele — Team Leader**
- Adetoro Michael Oluwaferanmi
- D-PROF

---

## Author

**Emmanuel Ebiendele**  
AI/ML Engineer & AI Product Builder

- GitHub: https://github.com/emmanuel-123tech
- LinkedIn: https://www.linkedin.com/in/emmanuel-ebiendele-063ba0255/
- Zindi: https://zindi.africa/users/Ebiendele
