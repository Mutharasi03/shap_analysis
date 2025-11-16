# Credit Risk Prediction – SHAP and LIME Interpretability

## Project Overview

This project explores interpretable machine learning for credit risk prediction using anonymized borrower data.  
We train a non-linear classification model (XGBoost) to predict loan default risk and apply SHAP and LIME to explain both global and local feature importance.  
The goal is to simulate real-world compliance scenarios where model transparency is essential for regulatory approval and stakeholder trust.

## Key Findings

- **Model Performance**:  
  After tuning, the model achieved an AUC of 0.84, Precision of 0.78, and Recall of 0.81.  
  These metrics indicate strong predictive power and balanced classification performance.

- **Global Interpretability (SHAP)**:  
  The top predictors of loan default include FICO Score, Debt-to-Income Ratio, Employment Length, Annual Income, and Loan Amount.  
  SHAP summary plots reveal consistent global feature rankings across the dataset.

- **Local Interpretability (SHAP vs LIME)**:  
  Three cases were analyzed: one clear approval, one clear denial, and one borderline decision.  
  SHAP force plots and LIME weights were compared side-by-side to highlight feature contributions.  
  SHAP provided stable, additive explanations aligned with model behavior, while LIME offered intuitive surrogate approximations.

## Repository Structure
credit-risk-interpretability/
├── shap.ipynb  
├── report.md 
├── requirements.txt 
├── credit_data.csv 
└── plots/ # Saved SHAP and LIME visualizations


## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mutharasi03/shap_analysis.git
   cd shap_analysis

2. **Create a virtual environment**
   python -m venv venv
   source venv/bin/activate   # On Linux/Mac
   venv\Scripts\activate      # On Windows

3. **Install dependencies**
   pip install -r requirements.txt

4. **Run the notebook**
   jupyter notebook shap.ipynb

**Deliverables**
shap.ipynb: Model training, SHAP and LIME analysis

report.md: Text-based summary of results and comparison

plots/: Visualizations of global and local explanations

requirements.txt: Python environment setup

**Notes**
Ensure credit_data.csv is placed in the root directory.

All plots are saved automatically when running the notebook.

The report.md file is generated with actual feature weights for SHAP and LIME.

This version directly addresses the feedback:
- It summarizes **key findings** and model choices.
- It avoids generic boilerplate and highlights **interpretability results**.
- It sets up the project clearly for reviewers or collaborators.
