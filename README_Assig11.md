# **Assignment 11: Image Classification Using Random Forest**
- **Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 12

# CIFAR-10 Image Classification Project

## Project Description
This advanced computer vision project implements and compares multiple machine learning approaches for image classification using the CIFAR-10 dataset. The analysis includes traditional ML models (Random Forest, SVM) with comprehensive feature engineering, along with performance benchmarking and deployment strategies.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to https://colab.research.google.com/
2. Sign in with your Google account

### Step 2: Upload and Open Notebook
1. Download `Lesson_11_assignment.ipynb` to your computer
2. In Colab, click **File → Upload notebook**
3. Select the downloaded `.ipynb` file
4. Click **Open**

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Load CIFAR-10 dataset automatically via TensorFlow/Keras
   - Perform image preprocessing and normalization
   - Train multiple ML models (Random Forest, SVM)
   - Generate performance comparisons and visualizations

## Dataset Source
- **Dataset**: CIFAR-10
- **Automatically loaded** via TensorFlow: `tf.keras.datasets.cifar10`
- **Size**: 60,000 32x32 color images
- **Classes**: 10 categories (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)

## No Installation Required
Google Colab provides all required libraries:
- pandas, numpy, matplotlib, seaborn
- scikit-learn, scikit-image
- tensorflow

## Results Preview
- **Best Model**: Random Forest (40.8% accuracy)
- **Comparative Model**: SVM (29.6% accuracy)
- **Key Features**: Confusion matrices, feature importance visualization

## Model Performance Summary
| Model | Accuracy | Best Use Case |
|-------|----------|---------------|
| Random Forest | 40.8% | Best traditional ML performance |
| SVM | 29.6% | Linear classification tasks |

## Technical Highlights
- **Advanced Preprocessing**: Image normalization and flattening
- **Hyperparameter Tuning**: GridSearchCV for optimal model configuration
- **Feature Analysis**: Top-30 feature importance visualization
- **Model Interpretation**: Comprehensive confusion matrix analysis

## Troubleshooting
- If any cell fails: Click the play button to re-run it
- Ensure you're signed into Google Colab
- Internet connection required for dataset download
- First run may take 5-10 minutes for model training
- Restart runtime if packages fail to load: **Runtime → Restart runtime**