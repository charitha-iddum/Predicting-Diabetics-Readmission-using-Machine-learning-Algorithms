# Predicting-Diabetics-Readmission-using-Machine-learning-Algorithms

## Student Information
**Student Name:** Charitha Sri Iddum  

## Deliverables
### Jupyter Notebooks:
- **Data Preprocessing**
- **Model Evaluation**

### Blog Post:

## Executive Summary
### Introduction
For the final project for Module 5, we have chosen a binary classification project on predicting 30-day Readmission Risk of patients with Diabetes.

### Objectives
Hospital readmissions are associated with unfavorable patient outcomes and high financial costs.

- **Medicare Payment Advisory Commission (MedPAC)** :
  - 17.6% of hospital admissions resulted in readmissions within 30 days.
  - 11.3% within 15 days.
  - 6.2% within 7 days.  

- **Diabetes Readmission Rate:** 20.3% (Agency for Healthcare Research and Quality)

- **Healthcare Regulatory Agencies Focus on 30-day Readmission Rates:**
  - Hospital Readmissions Reduction Program (HRRP)
  - Bundled Payments for Care Improvement Advanced (BPCIA)
  - Comprehensive Care for Joint Replacement (CJR) Model
  - Medicare Shared Savings Program (MSSP)
  - Delivery System Reform Incentive Payment (DSRIP) Program

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
