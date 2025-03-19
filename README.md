# Predicting-Diabetics-Readmission-using-Machine-learning-Algorithms

## Student Information
**Student Name:** Charitha Sri Iddum  

## Deliverables
Jupyter Notebooks:
- **Data Preprocessing**
- **Model Evaluation**

Blog Post:

Executive Summary
### Introduction
we have chosen a binary classification project on predicting 30-day Readmission Risk of patients with Diabetes.

### Objectives
Hospital readmissions are associated with unfavorable patient outcomes and high financial costs.

- The Medicare Payment Advisory Commission (MedPAC) reported that in 2005, 17.6% of hospital admissions resulted in readmissions within 30 days of discharge, 11.3% within 15 days, and 6.2% within 7 days. National Conference of State Legislatures

- Diabetes is one of the most frequently treated condition in US Hospitals with 20.3% readmission rate. Agency for Healthcare Research and Quality

- Healthcare Regulatory Agencies are focused on 30-day readmission rates as a way to improve quality. The Centers for Medicare and Medicaid Services (CMS) have labeled 30-day readmission rates as a measure of healthcare quality and emphasize its reduction as a strategy to reduce healthcare costs while also maintaining quality. Some of these mandatory and/or voluntary programs are as follows:
  - Hospital Readmissions Reduction Program (HRRP) is a Medicare value-based purchasing program that reduces payments to hospitals with excess readmissions. The Affordable Care Act established the Hospital Readmissions Reduction Program to improve the quality of care while reducing costs. The program incentivizes hospitals to improve communication and care coordination efforts, and to better engage patients and caregivers, with respect to post-discharge planning.
- Bundled Payments for Care Improvement Advanced (BPCIA). An alternative payment model to incentivize financial accountability, care redesign, data analysis and feedback, provider engagement, and patient engagement with bundled payments, care redesign activities, and accountability for performance on quality measures. This program links reimbursement or payment to the quality of care provided during a specific episode period.
- Comprehensive Care for Joint Replacement (CJR) model is an episode payment model that uses bundled payments for clinical episodes focused on lower extremity joint replacements
- Medicare Shared Savings Program (MSSP) is a voluntary program that encourages groups of doctors, hospitals, and other health care providers to come together as an Accountable Care Organization (ACO) to give coordinated, high quality care to their Medicare patients. This program showed greater reductions in readmission rates.
- Delivery System Reform Incentive Payment (DSRIP) Program is the main mechanism by which New York State will implement the Medicaid Redesign Team (MRT) Waiver Amendment. DSRIP´s purpose is to restructure the health care delivery system by reinvesting in the Medicaid program, with the primary goal of reducing avoidable hospital use by 25% over 5 years. Up to $6.42 billion dollars are allocated to this program with payouts based upon achieving predefined results in system transformation, clinical management and population health.

### Project Goals
A successful predictive model will help the Healthcare Organization:
- Identify high-risk patients to reduce preventable readmissions.
- Improve resource utilization and operational efficiency.
- Improve hospital rating and patient satisfaction.
- Reduce financial penalties associated with high readmission rates.

---

## Data Science Workflow
Using the **OSEMN Framework**:
1. **Obtain the data** - Understanding the problem and gathering requirements.
2. **Scrubbing** - Pre-processing (handling nulls, outliers, normalization, feature selection).
3. **Explore** - Understanding cohort characteristics and impactful predictors.
4. **Modeling** - Building and tuning the model.
5. **iNterpret** - Communicating results to stakeholders.

---

## Project Breakdown
### Part I:
- Introduction
- Data Loading
- Data Preprocessing

### Part II:
- Model Development
- Hyperparameter Tuning
- Model Evaluation
- Performance Metrics
- Final Model Selection & Saving

### Research Questions:
1. Who among hospitalized diabetic patients are at risk for 30-day readmission?
2. How can we risk stratify and rank patients based on readmission probability?
3. Which features are the most important predictors?
4. Are HbA1c results, treatment changes, and glycemic factors significant contributors?

---

## Dataset Information
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)    
**Hospitals:** 130 US hospitals  
**Number of Instances:** 101,766  
**Number of Variables:** 50  

### Target Variable:
- **Readmitted:** '<30' (readmitted within 30 days), '>30', 'No' (not readmitted)

### Predictors:
- **Demographics:** Race, Gender, Age, Weight
- **Hospitalization Details:** Admission Type, Discharge Disposition, Time in Hospital
- **Medical History:** Number of Lab Procedures, Medications, Diagnoses
- **Diabetes Specific Variables:** HbA1c test result, Change of Medications, Diabetes Medications
- **Other:** Number of inpatient/outpatient visits, emergency visits

### Missing Data:
- **Race:** 2,273 missing
- **Weight:** 98,569 missing
- **Payer Code:** 40,256 missing
- **Medical Specialty:** 49,949 missing
- **Diagnosis 1-3:** Some missing values

---

## Prerequisites
Before running the project, install the necessary dependencies:
```sh
# Install Anaconda
https://docs.anaconda.com/anaconda/install/

# Install Scikit-learn
conda install -c anaconda scikit-learn

# Install Imbalanced-Learn
conda install -c conda-forge imbalanced-learn

# Install XGBoost
conda install -c conda-forge xgboost
```

---

## Acknowledgments
- **Dataset:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **Research Paper:** [Impact of HbA1c Measurement on Readmission Rates](https://www.hindawi.com/journals/bmri/2014/781670/)
- **Class Imbalance Techniques:** [Machine Learning Mastery](https://machinelearningmastery.com/what-is-imbalanced-classification/)
- **Precision-Recall Curves:** [Machine Learning Mastery](https://machinelearningmastery.com/roc-curves-and-precision-recall-curves-for-classification-in-python/)

---
