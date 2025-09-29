# Heart_Disease_Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/Pandas-1.5-brightgreen) 
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-purple)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-1.2-orange)  

This repository contains a Python implementation of **Exploratory Data Analysis (EDA)**, preprocessing, and machine learning classification using **Decision Trees** and **Random Forests** on the Heart Disease dataset. The project explores model performance, overfitting control, feature importance, and cross-validation to ensure robust evaluation.

## 📑 Table of Contents
- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Exploratory Data Analysis](#exploratory-data-analysis)  
- [Modeling](#modeling)  
- [Tools & Libraries](#tools--libraries)  
- [How to Run](#how-to-run)  
- [Conclusion](#conclusion)  
- [Author](#author)  

## 📌 Project Overview
The goal of this project is to predict whether a patient is likely to have **heart disease** based on clinical and demographic features.  

- **Decision Tree Classifier**: Provides an interpretable model but can overfit if depth is not controlled.  
- **Random Forest Classifier**: An ensemble of decision trees that improves accuracy and generalization.  

By combining EDA, model training, and evaluation, this project helps identify **important risk factors** and **predictive features** for heart disease.

## 📊 Dataset

**Source:** [Heart Disease UCI Dataset](https://www.kaggle.com/datasets/ronitf/heart-disease-uci)  

The dataset contains **303 patient records** with **14 attributes** used to predict the presence (`1`) or absence (`0`) of heart disease.  

### 🔹 Features Overview

- **Target Variable**  
  - `target`: Presence of heart disease (`1` = Disease, `0` = No Disease).  

- **Patient Demographics**  
  - `age`: Age of the patient (in years).  
  - `sex`: Gender (1 = Male, 0 = Female).  

- **Chest Pain & Symptoms**  
  - `cp`: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic).  

- **Blood Pressure & Cholesterol**  
  - `trestbps`: Resting blood pressure (in mm Hg).  
  - `chol`: Serum cholesterol level (mg/dl).  
  - `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).  

- **Electrocardiographic & Exercise Data**  
  - `restecg`: Resting electrocardiographic results (0, 1, 2).  
  - `thalach`: Maximum heart rate achieved.  
  - `exang`: Exercise-induced angina (1 = yes, 0 = no).  
  - `oldpeak`: ST depression induced by exercise relative to rest.  
  - `slope`: Slope of the peak exercise ST segment (0, 1, 2).  

- **Other Clinical Features**  
  - `ca`: Number of major vessels colored by fluoroscopy (0–3).  
  - `thal`: Thalassemia test result (0 = normal, 1 = fixed defect, 2 = reversible defect).  

### 📈 Dataset Characteristics
- **Number of Instances**: 303  
- **Number of Features**: 13 predictors + 1 target variable  
- **Classes**: Heart Disease (1 = 165 cases), No Disease (0 = 138 cases)  
- **Imbalance**: Slightly skewed but balanced enough for binary classification tasks  


## 🔍 Exploratory Data Analysis
1. **Data Overview** – Summary statistics, missing values check.  
2. **Target Distribution** – Class balance between patients with and without heart disease.  
3. **Correlation Heatmap** – Showed relationships between clinical measurements.  
4. **Boxplots & Violin Plots** – Compared cholesterol, blood pressure, and age across target groups.  
5. **Countplots for Categorical Features** – Visualized distributions of chest pain type, gender, thalassemia, etc.  


## 🤖 Modeling
1. **Decision Tree Classifier**  
   - Controlled tree depth to reduce overfitting.  
   - Visualized the decision tree for interpretability.  

2. **Random Forest Classifier**  
   - Improved accuracy using an ensemble of decision trees.  
   - Feature importance ranking identified most predictive factors.  

3. **Evaluation Metrics**  
   - Accuracy, precision, recall, and F1-score.  
   - Confusion matrix for error analysis.  
   - ROC curve comparison between Decision Tree and Random Forest.  
   - Cross-validation for robust performance check.  
   - Learning curves to evaluate bias vs variance.  


##  Tools & Libraries
- **Python**  
- **Pandas & NumPy** – data handling  
- **Matplotlib & Seaborn** – visualization  
- **Scikit-learn** – preprocessing, modeling, evaluation  
- **Jupyter Notebook** – interactive exploration  


##  How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Shrilaxmi-16/Heart_Disease_Analysis.git
   cd Heart_Disease_Analysis

## ✅ Conclusion
This project demonstrated how **machine learning models** can be applied to predict heart disease using clinical and demographic features.  

- **Exploratory Data Analysis (EDA)** revealed important insights such as higher cholesterol, ST depression (`oldpeak`), and chest pain type (`cp`) being strongly associated with heart disease.  
- A **Decision Tree Classifier** provided interpretability but showed signs of **overfitting** when depth was not restricted.  
- The **Random Forest Classifier** outperformed the single decision tree, achieving **higher accuracy and better generalization** by leveraging ensemble learning.  
- **Feature importance analysis** highlighted `cp`, `thalach`, `oldpeak`, and `ca` as key predictive factors for heart disease.  
- **ROC curves and cross-validation** confirmed that the Random Forest was more robust and reliable compared to the Decision Tree.  
- **Learning curves** showed that Random Forest mitigates variance issues and benefits from more training data, while Decision Trees saturate quickly.  

## Author
Shrilaxmi Gidd

Email: shrilaxmigidd16@gmail.com

Date: 29-09-2025

