# **Assignment 10: Advanced Sentiment Analysis with Traditional ML and Transformers**
- **Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 21

# Twitter Airline Sentiment Analysis

## Project Description
This advanced NLP project analyzes customer sentiment from US airline tweets using both traditional machine learning and transformer models. The analysis compares Logistic Regression, SVM, Random Forest, and BERT models, with **BERT achieving 90% accuracy**. The project includes comprehensive EDA, multi-model comparison, and production-ready deployment strategies.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to [Google Colab](https://colab.research.google.com/)
2. Sign in with your Google account

### Step 2: Upload and Open Notebook
1. Download `Lesson_10_assignment.ipynb` to your computer
2. In Colab, click **File → Upload notebook**
3. Select the downloaded `.ipynb` file
4. Click **Open**

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Load Twitter airline dataset from GitHub
   - Perform text preprocessing and cleaning
   - Train multiple ML models (Logistic Regression, SVM, Random Forest)
   - Fine-tune BERT transformer model
   - Generate performance comparisons and visualizations
   - Create sentiment prediction examples

## Dataset Source
- **Location**: GitHub repository
- **Automatically loaded** from: 
  `https://raw.githubusercontent.com/cmreyesvalencia-png/colab-git-assignment2-CR/main/Tweets.csv`
- **Size**: 14,640 tweets from US airlines
- **Sentiment Distribution**: Negative (62.7%), Neutral (21.2%), Positive (16.1%)

## No Installation Required
Google Colab provides all required libraries pre-installed:
- pandas, numpy, matplotlib, seaborn
- scikit-learn, nltk, wordcloud
- transformers, torch (for BERT model)

## Results Preview
- **Best Model**: BERT Transformer (90% accuracy)
- **Traditional ML**: Logistic Regression (78.6% accuracy)
- **Key Features**: Word clouds, t-SNE visualization, feature importance
- **Multi-Model Pipeline**: Production-ready sentiment analysis system

## Model Performance Summary
| Model | Accuracy | Best Use Case |
|-------|----------|---------------|
| BERT | 90% | High-accuracy customer service |
| Logistic Regression | 78.6% | Real-time processing |
| SVM | 78.2% | Balanced performance |
| Random Forest | 63.7% | Feature analysis |

## Troubleshooting
- If any cell fails: Click the play button ▶️ to re-run it
- Ensure you're signed into Google Colab
- Internet connection required for dataset download and BERT model loading
- First run may take longer due to BERT model download (~5-10 minutes)
- For BERT errors: Restart runtime and run again