# Wine Quality Prediction using Logistic Regression

## Project Overview
This project predicts wine quality based on physicochemical properties using **logistic regression**.  
Wine quality is a multi-class target variable. The project demonstrates an end-to-end workflow including:

- Data preprocessing  
- Feature scaling  
- Model training  
- Model evaluation  
- Feature importance analysis  

---

## Step-by-Step Workflow

### Step 1: Load and Inspect Dataset
- The dataset contains features: `acidity`, `sugar`, `pH`, `alcohol`, `density`  
- Target: `quality` (wine quality rating)  
- **Observations:**
  - No missing values  
  - Numerical features are continuous  

**Sample Data:**
| acidity | sugar | pH    | alcohol | density | quality |
|---------|-------|-------|---------|---------|---------|
| 5.822   | 7.531 | 2.840 | 8.178   | 0.9979  | 6       |
| 3.959   | 1.871 | 3.236 | 12.053  | 0.9822  | 3       |
| 4.059   | 5.781 | 3.679 | 8.269   | 1.048   | 8       |

---

### Step 2: Data Preprocessing
- Features (`X`) and target (`y`) separated  
- Dataset split into **training set (80%)** and **test set (20%)**

**Training samples:** 80% of total  
**Test samples:** 20% of total  

---

### Step 3: Feature Scaling
- Standardization applied to all features to bring them to the same scale  
- Mean = 0, Standard deviation = 1  

---

### Step 4: Train Logistic Regression Model
- Logistic Regression used for **multi-class classification**  
- `max_iter` increased to ensure convergence  

---

### Step 5: Model Predictions
- Predictions made on the test set  

---

### Step 6: Model Evaluation
**Metrics Used:**
- **Accuracy:** Overall proportion of correct predictions  
- **Macro-F1:** Average F1 score treating all classes equally  
- **Weighted-F1:** Average F1 score weighted by class frequency

## Conclusion
- Logistic Regression provides a **baseline model** for predicting wine quality.  
- The model shows **low accuracy**, highlighting the need for more complex models for multi-class classification.  
- **Acidity, sugar, and pH** are the most influential features.  
- Using advanced algorithms, feature engineering, and proper handling of class imbalance can significantly improve prediction performance.  
- This project demonstrates the importance of **data preprocessing, feature scaling, evaluation metrics, and feature analysis** in a machine learning workflow.

---
