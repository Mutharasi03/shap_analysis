# Credit Risk Prediction – SHAP and LIME Analysis

## Project Overview
This project applies interpretable machine learning techniques to credit risk prediction.  
We train a classification model (XGBoost) on anonymized borrower data and use SHAP and LIME to explain both global and local feature importance.  
The focus is on model transparency and compliance, simulating real-world requirements where explainability is essential for regulatory approval and stakeholder trust.

## Repository Structure
credit-risk-interpretability/ 
├── shap.ipynb # Main notebook with model training and interpretability analysis
├── report.md # Markdown report with results and comparison
└── plots/ # Saved SHAP and LIME visualizations


## Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mutharasi03/shap_analysis.git
   cd shap_analysis
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

2.Generate results

Train the model and evaluate metrics (AUC, Precision, Recall).

Produce SHAP summary plots for global feature importance.

Generate SHAP force plots and LIME explanations for selected cases.

A report.md file will be created automatically with results.

3. Deliverables
Model performance metrics (AUC, Precision, Recall).

Global SHAP feature importance (top 5 predictors).

Local explanations for approval, denial, and borderline cases.

Comparative analysis of SHAP vs LIME.
