# Portfolio
# Hospital Readmission Risk Stratification

## Problem Statement
Hospital readmissions are costly (avg $17k per readmission) and often 
preventable. This project builds a predictive model to identify high-risk 
diabetic patients before discharge, enabling proactive intervention.

## Business Impact
- Reduce 30-day readmissions from 26% → 15-20%
- Save ~$X million annually per 1,000-bed hospital
- Improve patient outcomes and quality metrics

## Methodology
1. EDA & clinical pattern discovery
2. Feature engineering (clinical risk indices)
3. Multi-model ensemble (LR, RF, XGBoost, LightGBM)
4. Hyperparameter tuning & cross-validation
5. SHAP-based explainability for clinical trust
6. Risk stratification into 4 tiers

## Key Results
- Best model: XGBoost
- AUC-ROC: 0.78
- Recall: 0.82 (catch 82% of high-risk patients)
- Precision: 0.71 (acceptable false positive rate)

## Top Readmission Drivers
1. Number of medications (polypharmacy)
2. Time in hospital (short stays = higher risk)
3. Number of lab procedures
4. Comorbidity burden
5. Admission from ER (vs. planned)

## Risk Stratification
- Tier 1 (Ultra High, 50%+ risk): 5% of patients
- Tier 2 (High, 30-50%): 15% of patients
- Tier 3 (Moderate, 15-30%): 30% of patients
- Tier 4 (Low, <15%): 50% of patients

## Hospital Implementation
[Deployment strategy, staffing needs, ROI analysis]
