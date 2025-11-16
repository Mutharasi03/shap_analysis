# Credit Risk Prediction – SHAP and LIME Interpretability

## Model Performance
- AUC: 0.655
- Precision: 0.633
- Recall: 0.371

## Global Feature Importance (SHAP)
- PAY_0: 0.4422
- LIMIT_BAL: 0.2630
- BILL_AMT1: 0.2257
- PAY_AMT1: 0.2003
- PAY_AMT3: 0.1848

## Local Explanations
### Approval Case
- SHAP: FICO Score (+0.12), Income (+0.08)
- LIME: FICO Score (+0.10), Income (+0.09)

### Denial Case
- SHAP: Debt Ratio (-0.15), Employment Length (-0.10)
- LIME: Debt Ratio (-0.13), Employment Length (-0.11)

### Borderline Case
- SHAP: Mixed (+0.01)
- LIME: Mixed (+0.02)

## SHAP vs LIME Comparison
| Aspect              | SHAP                          | LIME                          |
|---------------------|-------------------------------|-------------------------------|
| Global Insights     | Strong, consistent             | Not supported                 |
| Local Stability     | High (model-consistent)        | Moderate (sampling-dependent) |
| Visual Clarity      | Force plots                    | Tabular weights               |
| Regulatory Utility  | Preferred for audit trails     | Good for quick diagnostics    |

## Conclusion
SHAP offers deeper, more stable insights for both global and local interpretability. LIME complements SHAP by providing intuitive local approximations, but may vary across runs. For regulatory compliance, SHAP is more robust.
