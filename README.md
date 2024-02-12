# Health Data Analysis

This project analyzes health data to predict the likelihood of developing cardiovascular disease (CVD) using machine learning models.

## Overview

Cardiovascular disease (CVD) is a leading cause of mortality worldwide, and early detection of risk factors can help in prevention and management. This project utilizes the Framingham Heart Study dataset to develop predictive models for assessing the risk of CVD based on various health indicators.

## Features

- Data loading and preprocessing: The dataset is loaded and preprocessed to handle missing values and encode categorical variables.
- Model training: Machine learning models, such as Random Forest, are trained on the preprocessed data to predict the likelihood of developing CVD.
- Model evaluation: The performance of the trained models is evaluated using accuracy and other relevant metrics.
- Visualization: The project includes visualizations to showcase interesting trends and insights in the health data.

## Installation

1. Clone the repository:
git clone https://github.com/dcoolvip/health-analysis.git


2. Install dependencies:
pip install -r requirements.txt


## Usage

1. Run the main script to analyze the health data and train machine learning models:
python main.py

## Dataset

The Framingham Heart Study dataset is used for this analysis. It contains various health indicators and demographic information collected from participants in the Framingham Heart Study, a long-term cardiovascular study conducted in Framingham, Massachusetts. Refer: https://www.kaggle.com/datasets/aasheesh200/framingham-heart-study-dataset/data 

## Dependencies

- pandas
- scikit-learn
- matplotlib
- seaborn

## Analysis Findings

Refer notebook_output.pdf file for results with the visualizations

**1. Distribution of TenYearCHD (Coronary Heart Disease):**

  The count plot shows the distribution of the target variable TenYearCHD, which represents the presence or absence of coronary heart disease (CHD) within ten years.
  
  **Insights:**
  
    - We can observe the imbalance in the distribution of the target variable, with a larger proportion of 
    individuals labeled as not having CHD (TenYearCHD = 0) compared to those labeled as having CHD (TenYearCHD = 1).
    
    - This class imbalance may need to be addressed when training machine learning models to predict CHD risk.
    
**2. Correlation Heatmap:**

  The heatmap visualizes the correlation matrix between different features in the dataset.

  **Insights:**
  
    - Certain features show a moderate to strong positive correlation with each other, indicating a relationship 
    between them. For example, age and systolic blood pressure (sysBP) exhibit a positive correlation, which is 
    expected in a cardiovascular risk assessment.
    
    - Features with higher correlations with the target variable (TenYearCHD) are potential predictors 
    of CHD risk. For example, age, systolic blood pressure, and total cholesterol (totChol) show moderate
    positive correlations with CHD risk, while HDL cholesterol (totChol) exhibits a moderate negative 
    correlation, which is in line with medical knowledge.
    
These insights provide valuable information for understanding the dataset and identifying potential predictors of coronary heart disease risk. They can guide further analysis and model development to create effective risk prediction models and inform preventive measures to reduce the incidence of CHD.
