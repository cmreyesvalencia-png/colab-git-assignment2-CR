# **Assignment 13: Generative AI Essentials**
**Course:** Data Analytics and Business Intelligence Analyst
- **Institution:** Willis College
- **Student Name:** Carlos Reyes
- **Instructor:** Ratinder Rajpal
- **Date:** 2025 Nov, 14


# GPT-2 Text Generation & Fine-tuning Project

## Project Description
This project implements and demonstrates text generation capabilities using OpenAI's GPT-2 model fine-tuned on literary texts from Project Gutenberg. The implementation includes model training, parameter tuning, and practical content creation applications with comprehensive generation controls.

## Quick Setup & Run (Google Colab)

### Step 1: Open Google Colab
1. Go to https://colab.research.google.com/
2. Sign in with your Google account

### Step 2: Create New Notebook
1. Click **File → New notebook**
2. Copy and paste the provided code into cells
3. Or upload the existing `.ipynb` file if available

### Step 3: Run the Analysis
1. Click **Runtime → Run all** (or press `Ctrl+F9`)
2. Wait for all cells to execute automatically
3. The notebook will:
   - Install required transformers and datasets libraries
   - Load pre-trained GPT-2 model and tokenizer
   - Download and preprocess Project Gutenberg dataset
   - Fine-tune GPT-2 on literary texts
   - Generate text samples with various parameters
   - Demonstrate content creation applications

## Dataset Source
- **Primary Dataset**: Project Gutenberg (via Hugging Face `gutenberg`)
- **Alternative**: `sedthh/gutenberg_english` 
- **Fallback**: Curated literary excerpts from classic literature
- **Content**: Public domain literary works including novels, poetry, and classic texts

## Required Libraries
Google Colab provides most libraries, but additional installations needed:
```python
!pip install transformers torch datasets