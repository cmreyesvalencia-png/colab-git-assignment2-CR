# **Assignment 12: Neural Network and Deep Learning Basics**
- **Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 13

# CIFAR-10 Neural Network & Deep Learning Project

## Project Description
This comprehensive deep learning project implements and compares neural network architectures for image classification using the CIFAR-10 dataset. The analysis includes traditional feedforward neural networks versus convolutional neural networks (CNNs), with detailed performance benchmarking and architectural insights.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to https://colab.research.google.com/
2. Sign in with your Google account

### Step 2: Upload and Open Notebook
1. Download `Assignment_12_Neural_Networks.ipynb` to your computer
2. In Colab, click **File → Upload notebook**
3. Select the downloaded `.ipynb` file
4. Click **Open**

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Load CIFAR-10 dataset automatically via TensorFlow/Keras
   - Perform image preprocessing and normalization
   - Train Neural Network and CNN models
   - Generate performance comparisons and visualizations
   - Produce comprehensive evaluation reports

## Dataset Source
- **Dataset**: CIFAR-10
- **Automatically loaded** via TensorFlow: `tf.keras.datasets.cifar10`
- **Size**: 60,000 32x32 color images
- **Classes**: 10 categories (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)

## No Installation Required
Google Colab provides all required libraries:
- tensorflow, keras
- matplotlib, seaborn, numpy
- scikit-learn

## Results Preview
- **Best Model**: Convolutional Neural Network (75.17% accuracy)
- **Comparative Model**: Neural Network (39.22% accuracy)
- **Performance Gap**: +35.95% improvement with CNN
- **Key Features**: Training history plots, confusion matrices, architectural analysis

## Model Performance Summary
| Model | Accuracy | Parameters | Training Status |
|-------|----------|------------|-----------------|
| Convolutional Neural Network | 75.17% | 500K | ✅ Excellent |
| Neural Network | 39.22% | 1.6M | ❌ Underfitting |

## Technical Highlights
- **Advanced Preprocessing**: Image normalization and data augmentation
- **Architecture Comparison**: Feedforward NN vs CNN performance analysis
- **Visualization**: Training history, confusion matrices, prediction samples
- **Model Interpretation**: Comprehensive architectural insights and recommendations

## Troubleshooting
- If any cell fails: Click the play button to re-run it
- Ensure you're signed into Google Colab
- Internet connection required for dataset download
- First run may take 10-15 minutes for model training
- Restart runtime if packages fail to load: **Runtime → Restart runtime**
- For memory issues: **Runtime → Restart and run all**