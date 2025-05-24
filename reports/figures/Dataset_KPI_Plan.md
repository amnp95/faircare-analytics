# Dataset & KPI Plan

## Problem Statement

Hospital readmissions within 30 days of discharge are both costly and preventable. We aim to develop a machine learning model that predicts which patients are at highest risk of being readmitted within 30 days, based on their electronic health records (EHR). In addition to predictive performance, the project integrates fairness analysis to ensure equitable treatment across demographics such as race, gender, and insurance status.


## Dataset Selected: MIMIC-IV (Medical Information Mart for Intensive Care)

**Source**: MIT & Beth Israel Deaconess Medical Center  
**Access**: Public, via PhysioNet with data use agreement  
**Coverage**: 2008–2019, over 70,000 ICU and hospital admissions  
**Features**: Age, gender, race, diagnoses (ICD codes), vital signs, lab results, medications, procedures, discharge disposition, and readmission history

**Website**: [https://physionet.org/content/mimiciv/3.1/](https://physionet.org/content/mimiciv/3.1/)


## Stakeholders

- **Clinicians**: Use model outputs to identify high-risk patients before discharge.
- **Hospital Administrators**: Reduce readmission penalties and optimize post-discharge care.
- **Case Managers and Care Coordinators**: Prioritize follow-up for high-risk patients.
- **Health Equity Advocates**: Ensure fairness in predictive models.
- **Patients**: Benefit from timely interventions and improved outcomes.
- **Data Science Team**: Build, evaluate, and maintain the predictive model.

## Key Performance Indicators (KPIs)

### 📌 Core KPIs (During Development)

🔸 AUC-ROC and F1-score  
  → Measures the model's ability to correctly predict and balance actual readmissions vs false alarms.

🔸 True positive rate across demographic groups  
  → Ensures the model performs fairly for all populations (e.g., race, gender, insurance).

🔸 SHAP-based explainability  
  → Provides transparency by explaining which features influenced each prediction.

🔸 Disparate impact ratio between subgroups  
  → Checks for bias by comparing prediction rates between different demographic groups.

### 🔮 Future KPIs (Post-Deployment Evaluation)

🔸 Reduction in predicted readmission rate for top-risk decile  
  → Evaluates the model’s impact by checking if it correctly identifies patients most at risk.

🔸 Stakeholder satisfaction/feedback during prototype demo  
  → Gauges real-world acceptance and usability of the model among clinicians and staff.

