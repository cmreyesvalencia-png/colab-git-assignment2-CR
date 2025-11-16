# **Assignment 15: Loan Default Prediction**
**Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 16

## Project Description
<!-- This project implements a complete machine learning pipeline for predicting loan defaults, with a strong emphasis on model explainability and fairness. The analysis includes comprehensive data cleaning, feature engineering, model training with a Random Forest classifier, and a deep-dive fairness assessment using age as a sensitive attribute. The project demonstrates practical techniques for building a transparent and ethically-aware predictive model in a financial context. -->

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
<!-- 1. Go to https://colab.research.google.com/
2. Sign in with your Google account -->

### Step 2: Create a New Notebook
<!-- 1. In Colab, click **File → New notebook**
2. Copy and paste the entire provided Python code into the first cell
3. Alternatively, create multiple cells by splitting the code at the `"""` comment blocks -->

### Step 3: Run the Analysis
<!-- 1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Automatically install required packages (`lime`, `shap`)
   - Load the Bank Loan dataset directly from GitHub
   - Perform exploratory data analysis (EDA) with visualizations
   - Clean the data and handle missing values
   - Create new engineered features
   - Train and evaluate a Random Forest model
   - Generate SHAP explainability plots
   - Conduct a comprehensive fairness analysis across age groups
   - Produce bias detection reports and ethical recommendations -->

## Dataset Source
<!-- - **Dataset:** Publicly Available Bank Loan Dataset
- **Source:** Loaded automatically from a GitHub repository URL
- **Initial Size:** 850 entries, 9 features
- **Final Cleaned Size:** 700 entries (after removing missing targets)
- **Target:** Binary default classification (1=Default, 0=No Default)
- **Key Features:** `age`, `ed` (education), `employ` (employment years), `income`, `debtinc` (debt-to-income ratio), `creddebt`, `othdebt`
- **Sensitive Attribute:** Age (used for fairness analysis) -->

## No Installation Required
<!-- Google Colab provides all required libraries:
- `scikit-learn`, `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `shap`, `lime` (installed automatically in the notebook) -->

## Results Preview
<!-- - **Overall Accuracy:** 80.7% on test set
- **Class Performance:** Stronger prediction for non-defaulters (F1: 87%) vs. defaulters (F1: 61%)
- **Critical Fairness Finding:** 38.7% accuracy disparity between age groups
- **Key Insights:** Debt-to-income ratio and employment stability are top predictors of default -->

## Model Performance Summary
<!-- | Metric | Class 0 (Non-Default) | Class 1 (Default) | Overall |
|--------|---------------------|-----------------|---------|
| **Precision** | 85% | 66% | - |
| **Recall** | 89% | 57% | - |
| **F1-Score** | 87% | 61% | - |
| **Accuracy** | - | - | 80.7% | -->

## Fairness Analysis by Age Group
<!-- | Age Group | Sample Size | Actual Default Rate | Predicted Default Rate | Accuracy |
|-----------|-------------|-------------------|----------------------|----------|
| **Young (20-35)** | 81 | 30.9% | 25.9% | 88.7% |
| **Middle-aged (36-50)** | 53 | 17.0% | 17.0% | 77.8% |
| **Senior (51-65)** | 6 | 50.0% | 33.3% | 50.0% | -->

## Technical Highlights
<!-- - **Feature Engineering:** Created 3 new predictive features (`total_debt`, `employment_stability`, `creddebt_ratio`)
- **Model Explainability:** SHAP summary plots for global feature importance
- **Fairness Assessment:** Comprehensive metrics across demographic groups
- **Statistical Testing:** Chi-square test for bias detection
- **Visual Analytics:** Multiple comparative plots for model performance and fairness -->

## Analysis Pipeline
<!-- - **Data Cleaning:** Handling missing target values, feature normalization
- **Exploratory Data Analysis:** Distribution analysis, correlation heatmaps, target variable analysis
- **Feature Engineering:** Creating domain-informed features to enhance predictive power
- **Model Training:** Random Forest classifier with stratified train-test split
- **Model Evaluation:** Accuracy, confusion matrix, classification report
- **Explainability:** SHAP analysis for model interpretation
- **Fairness Analysis:** Performance and prediction disparities across age groups -->

## Ethical Impact
<!-- - **Risk Level:** Medium-High - Significant performance disparity for senior applicants
- **Deployment Readiness:** Requires bias mitigation before production use
- **Critical Issue:** Model accuracy drops to 50% for the senior age group, potentially leading to unfair loan decisions for qualified older applicants -->

## Troubleshooting
<!-- - If `shap` or `lime` installation fails: Re-run the first pip install cell separately
- Ensure you're signed into Google Colab for full functionality
- Internet connection required for dataset download from GitHub
- First run may take 3-5 minutes for complete analysis
- If visualization fails: Re-run individual plotting cells
- For memory issues: **Runtime → Restart and run all**
- If SHAP plots don't display: Ensure `shap.initjs()` is executed -->

## Key Recommendations
<!-- 1. **Address Class Imbalance:** Implement techniques like SMOTE to improve default prediction sensitivity
2. **Mitigate Age Bias:** Apply fairness-aware algorithms or remove age-related proxy variables
3. **Human Oversight:** Implement manual review for applicants in the senior age group
4. **Feature Review:** Assess if `employment_stability` unfairly disadvantages younger applicants
5. **Continuous Monitoring:** Establish ongoing fairness audits in production deployment -->

## Learning Outcomes
<!-- - End-to-end implementation of a machine learning pipeline for financial risk prediction
- Practical experience with feature engineering and domain-informed feature creation
- Hands-on model explainability using SHAP values
- Comprehensive fairness assessment across sensitive demographic attributes
- Ethical considerations in financial machine learning applications
- Techniques for identifying and addressing algorithmic bias in real-world scenarios -->