# System Thread Forecaster

**System Thread Forecaster** is a machine learning project developed as part of a Kaggle competition. The objective was to develop a predictive model capable of identifying potential security threats in computer systems based on system configuration and usage data. This enables early warnings before a system becomes compromised by malware or other attacks.

##  Project Objective

To forecast whether a system is at risk of being infected by a specific malware family using its static properties and behavior logs. The aim was to enhance proactive security measures through intelligent threat prediction.

##  Tools & Technologies

**Python** (Pandas, NumPy, Scikit-learn)
**Matplotlib** and **Seaborn** for exploratory data analysis (EDA)
**Scikit-learn** models:
  `RandomForestClassifier` (best performer: ~96% accuracy)
  `RidgeClassifier` (moderate: ~60% accuracy)
  `LogisticRegression` and `SGDClassifier` (lower performance)
Feature encoding and scaling
Model evaluation using accuracy, confusion matrix, and cross-validation

##  Dataset Overview

Shape: 100,000 rows × 78 features
Mixed data types: numerical and categorical
Balanced target classes (50:50 infected vs. clean)
Preprocessing included:
  - Handling missing values
  - Label encoding of categorical variables
  - Feature selection for high-variance and correlation

##  Model Performance

 Model               -   Accuracy 

Random Forest        - 96%      
Ridge Classifier     - 60%      
Logistic Regression  - ~50%     
SGD Classifier       - ~50%     

Random Forest significantly outperformed other models, indicating strong nonlinear patterns in the data and high relevance of categorical feature interactions.
