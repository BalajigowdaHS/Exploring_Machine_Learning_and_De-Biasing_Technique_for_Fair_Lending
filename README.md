# Machine Learning for Fair Lending 

## Overview 

The project aimed to investigate potential fair lending violations in both the Home Mortgage Disclosure Act (HMDA) dataset and high-priced loans dataset. The focus was on building machine learning models to predict lending outcomes while identifying and mitigating algorithmic biases to ensure fairness across different demographic groups.

## Key Steps and Methodologies

### 1. Data Analysis for Fair Lending Violations:

**Exploratory Data Analysis (EDA):** Comprehensive EDA was performed on both the HMDA dataset and high-priced loans dataset. This included analyzing applicant demographics, loan characteristics, and outcomes to identify patterns and disparities.

**Comparative Analysis:** We compared lending outcomes and rates between standard loans and high-priced loans to detect any significant disparities that could indicate biased lending practices.

**Fair Lending Metrics:** Key metrics such as denial rates, approval rates, loan pricing, and disparate impact ratios were calculated to assess potential biases in the decision-making process for both datasets.

### 2. Building Predictive Models:

**Model Selection:** We developed several machine learning models including Logistic Regression, Decision Trees, Random Forests, and Gradient Boosting Machines. These models were selected for their capacity to handle complex relationships in the data and for their varying levels of interpretability.

**Feature Engineering:** Important features were selected and engineered to optimize model performance. This involved handling missing data, encoding categorical variables, normalizing numerical features, and creating new features based on domain knowledge.

**Model Training and Evaluation:** Models were trained on historical lending data and evaluated using performance metrics such as accuracy, precision, recall, and AUC-ROC. Separate evaluations were conducted for standard and high-priced loans to ensure robust performance across different types of lending.

### 3. Bias Mitigation Techniques:

**Pre-processing Techniques:** We applied techniques such as re-sampling to balance the representation of different demographic groups and re-weighting to adjust the influence of underrepresented groups before training the models.

**In-processing Techniques:** Algorithms like adversarial debiasing and constraint-based methods were implemented to promote fairness during the model training process by directly modifying the learning algorithm.

**Post-processing Techniques:** Techniques such as equalized odds post-processing were used to adjust model outputs to reduce bias after initial training, ensuring fairness in the final predictions.

### 4. Evaluation of De-biasing Effects:

**Fairness Metrics:** We measured the impact of de-biasing techniques using fairness metrics like demographic parity, equalized odds, and disparate impact ratios. These metrics were crucial in evaluating the reduction of bias in both standard and high-priced loan predictions.

**Trade-off Analysis:** We analyzed the trade-offs between fairness and model performance by comparing the accuracy, precision, recall, and other metrics of the original and debiased models. This helped in understanding the impact of de-biasing on model efficacy.

### 5. Above Files and Description

**HMDA 2022 Schema**: This document contains various sheets explaining the content of
variables and observations in the HMDA 2022 dataset.

**Approved & Denied Model (Data Cleaning and Model Selection):** Python code for data
cleaning, various model training, and model selection based on multiple performance metrics.

**Approved & Denied Model (Bias Removal on XGB Model):** The Python code for bias
removal on the best-performing model.

**High-Priced Model (Data Cleaning and Model Selection):** The Python code for data cleaning,
various model training, and model selection based on multiple performance metrics.

**High-Priced Model (Bias Removal on XGB Model):** The Python code for bias removal on the
best-performing model.

**Pre_Approval_Denial_Debias:** The clean dataset used to perform all the de-biasing techniques
in the Approval and Denial model.

**Pre_High_Priced_Debias:** The clean dataset used to perform all the de-biasing techniques in the
High-Priced model.

**Approved & Denied De-Biasing Techniques:** The Python code for running all the de-biasing
techniques on the Approved & Denied Model.

**High-Priced De-Biasing Techniques:** The Python code for running all the de-biasing techniques
on the High Priced Model.

**HMDA Dashboard:** PowerBI dashboard for the 2022 HMDA dataset. Requires PowerBI to
open.
