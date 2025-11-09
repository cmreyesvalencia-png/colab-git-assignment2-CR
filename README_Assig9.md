# **Assignment 9: Unsupervised Learning - Customer Segmentation**
- **Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 08

# Mall Customer Segmentation

## Project Description
This unsupervised learning project segments mall customers into distinct groups based on their demographics and spending behavior. The analysis compares K-Means vs Hierarchical Clustering models, identifying **3 optimal customer segments**. The project includes comprehensive EDA, clustering optimization, and customer profiling.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to [Google Colab](https://colab.research.google.com/)
2. Sign in with your Google account

### Step 2: Upload and Open Notebook
1. Download `Lesson_9_assignment.ipynb` to your computer
2. In Colab, click **File → Upload notebook**
3. Select the downloaded `.ipynb` file
4. Click **Open**

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Load Mall Customers dataset from GitHub
   - Perform data preprocessing and scaling
   - Apply K-Means and Hierarchical Clustering
   - Determine optimal clusters using Elbow Method
   - Generate customer segmentation visualizations
   - Create PCA plots for dimensionality reduction

## Dataset Source
- **Location**: GitHub repository
- **Automatically loaded** from: 
  `https://raw.githubusercontent.com/cmreyesvalencia-png/colab-git-assignment2-CR/main/Mall_Customers.csv`
- **Size**: 200 customer records
- **Features**: Age, Annual Income, Spending Score, Gender

## No Installation Required
Google Colab provides all required libraries pre-installed:
- pandas, numpy, matplotlib, seaborn
- scikit-learn for clustering algorithms
- StandardScaler for feature normalization

## Results Preview
- **Optimal Clusters**: 3 distinct customer segments
- **Best Model**: K-Means (Silhouette Score: 0.368)
- **Key Insights**: Clear customer groups based on income and spending patterns
- **Visualizations**: Elbow curve, PCA plots, cluster distributions

## Model Performance Summary
| Model | Clusters | Silhouette Score | Best Use Case |
|-------|----------|------------------|---------------|
| K-Means | 3 | 0.368 | Customer segmentation |
| Hierarchical | 3 | 0.363 | Cluster hierarchy visualization |

## Business Applications
- **Targeted Marketing**: Customized campaigns for each customer segment
- **Product Placement**: Optimize store layout based on customer profiles
- **Customer Retention**: Develop loyalty programs for high-value segments
- **Inventory Management**: Stock products matching segment preferences

## Troubleshooting
- If any cell fails: Click the play button ▶️ to re-run it
- Ensure you're signed into Google Colab
- Internet connection required for dataset download
- Check that all libraries load properly in first cell
- For visualization issues: Restart runtime and run again