# **Assignment 14: Ethical AI Analysis and Explainability**
**Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 16

## Project Description
This comprehensive ethical AI project implements a complete fairness assessment pipeline for machine learning models predicting income levels. The analysis includes bias detection using Fairlearn, model explainability with SHAP and LIME, and detailed fairness metrics evaluation across demographic groups. The project demonstrates practical techniques for identifying and mitigating algorithmic bias in real-world scenarios.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to https://colab.research.google.com/
2. Sign in with your Google account

### Step 2: Upload and Open Notebook
1. Download the project notebook to your computer
2. In Colab, click **File → Upload notebook**
3. Select the downloaded `.ipynb` file
4. Click **Open**

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Load Adult Income dataset automatically from UCI Repository
   - Perform data preprocessing and feature engineering
   - Train logistic regression model for income prediction
   - Conduct comprehensive fairness analysis using Fairlearn
   - Generate SHAP and LIME explainability visualizations
   - Produce bias detection reports and ethical recommendations

## Dataset Source
- **Dataset**: UCI Adult Income Dataset
- **Automatically loaded** from UCI Repository
- **Size**: 32,561 instances with 15 demographic features
- **Target**: Binary income classification (>50K or <=50K)
- **Sensitive Attributes**: Gender, race for fairness analysis

## No Installation Required
Google Colab provides all required libraries:
- fairlearn, shap, lime
- scikit-learn, pandas, numpy
- matplotlib, seaborn

## Results Preview
- **Overall Accuracy**: 80.3% on test set
- **Critical Finding**: 18.3% selection rate disparity between genders
- **Bias Detection**: Significant gender-based discrimination identified
- **Key Insights**: Model actively uses gender for predictions (SHAP analysis)

## Model Fairness Summary
| Metric | Female | Male | Disparity | Status |
|--------|--------|------|-----------|---------|
| **Selection Rate** | 1.5% | 19.8% | 18.3% | ❌ High Bias |
| **Accuracy** | 88.3% | 76.3% | 12.0% | ⚠️ Unbalanced |
| **True Positive Rate** | 5.3% | 43.7% | 38.4% | ❌ Severe Bias |

## Technical Highlights
- **Fairness Assessment**: Comprehensive metrics using Fairlearn framework
- **Global Explainability**: SHAP summary plots for model-level bias detection
- **Local Explainability**: LIME for individual prediction interpretations
- **Bias Visualization**: Comparative bar plots across demographic groups
- **Ethical Recommendations**: Actionable mitigation strategies

## Analysis Pipeline
- **Data Preprocessing**: Handling missing values, categorical encoding
- **Model Training**: Logistic regression with stratified sampling
- **Fairness Metrics**: Selection rate, false positive rate, true positive rate
- **Explainability**: Feature importance analysis and prediction explanations

## Ethical Impact
- **Risk Level**: High - Model would institutionalize gender discrimination
- **Deployment Readiness**: Not recommended without bias mitigation
- **Critical Issue**: Explicit use of protected attributes in predictions

## Troubleshooting
- If any cell fails: Click the play button to re-run it
- Ensure you're signed into Google Colab
- Internet connection required for dataset download
- First run may take 5-8 minutes for complete analysis
- Restart runtime if packages fail to load: **Runtime → Restart runtime**
- For memory issues: **Runtime → Restart and run all**
- If SHAP/LIME visualization fails: Re-run individual explainability cells

## Key Recommendations
1. Remove sensitive attributes from training data
2. Implement fairness-aware algorithms
3. Conduct proxy variable analysis
4. Establish continuous fairness monitoring
5. Apply demographic parity constraints

## Learning Outcomes
- Practical experience with AI fairness assessment
- Hands-on bias detection and mitigation techniques
- Explainable AI implementation for model transparency
- Ethical considerations in machine learning deployment
