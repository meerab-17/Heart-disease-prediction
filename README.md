# Heart-disease-prediction
A model to predict whether a person is at risk of heart disease based on their health data.


 Problem Statement

Heart disease is a leading cause of mortality worldwide. Early prediction of heart disease can greatly improve the chances of timely treatment and preventive care. In this task, we aim to use machine learning techniques to build a predictive model that classifies whether an individual is likely to have heart disease based on clinical attributes such as age, cholesterol levels, chest pain type, maximum heart rate, and more.

This project applies logistic regression and decision tree models to the problem and evaluates their performance using appropriate metrics such as accuracy, confusion matrix, and ROC-AUC.


 Dataset:

- Source: [Kaggle – Heart Disease UCI Dataset]
  
- File used: `heart.csv'
  
- Features: 13 medical attributes + target variable

Features:

| age in years |
| sex |
|Chest pain type (0–3) |
| trestbps: Resting blood pressure |
|Serum cholesterol (mg/dl) |
| fbs: Fasting blood sugar > 120 mg/dl |
| restecg: Resting ECG results (0–2) |
| thalach: Maximum heart rate achieved |
| exang: Exercise induced angina (1 = yes) |
| oldpeak: ST depression induced by exercise |
| slope: Slope of peak exercise ST segment |
| ca: Number of major vessels (0–3) colored by fluoroscopy |
| thal: 0 = normal, 1 = fixed defect, 2 = reversible defect |
| target:  1 = heart disease, 0 = no heart disease |


Tools & Libraries

Python

Pandas : Data loading and manipulation 

Seaborn & Matplotlib : Data visualization 

scikit-learn : ML models, preprocessing, evaluation 

Google Colab : Execution environment 


- Data Inspection:
  
- Checked for null values
  
- Reviewed column names and summary statistics
  

 Data Visualization:
 
- Count plot of heart disease presence
  
- Correlation heatmap to identify feature relationships
  

 Preprocessing:
 
- Feature-target split (`X` and `y`)
  
- Train-test split (80% training, 20% testing)
  
- Standardized the input features using `StandardScaler`
  

 Model Training:
 
- Logistic Regression: A baseline classification model
  
- Decision Tree Classifier: For interpretable rule-based decisions
  

 Evaluation:
 
- Accuracy score
  
- Confusion matrix
  
- ROC Curve and AUC for Logistic Regression
  



 Results:

 Logistic Regression:
 
- Performs well on scaled input
  
- AUC score showed strong separation between classes
  
- Works best for linear relationships
  

 Decision Tree:
 
- More interpretable
  
- Slightly lower accuracy but useful for explaining decisions
  

---

- Count plot of the target variable
  
- Correlation heatmap of features
  
- Confusion matrices for both models
  
- ROC curve for Logistic Regression
  

---

Conlusion:

- Logistic Regression was effective in identifying heart disease based on the given attributes.
  
- Decision Trees help in interpretability and rule generation, especially for healthcare professionals.
  
- Features like **chest pain type (cp)**, **max heart rate (thalach)**, and **oldpeak** showed strong correlation with heart disease.
  



