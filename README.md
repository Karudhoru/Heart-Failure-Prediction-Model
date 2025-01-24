# **Project Overview**

Heart disease is a leading cause of mortality worldwide, and early detection can significantly improve treatment outcomes. This project aims to develop a predictive model using **logistic regression** to assess the risk of heart disease based on various physiological and lifestyle factors. The dataset for this analysis was sourced from Kaggle and contains detailed records of **919 individuals**.

## **Problem Statement**

The primary goal of this project is to build a machine learning model that predicts the presence of heart disease based on several key indicators. This model can assist healthcare professionals in identifying high-risk individuals and making informed decisions for early intervention.

## **Dataset Description**

The dataset consists of **919 rows and 12 columns**, which include both features and the target variable. Each column provides critical information about a patient's health and potential risk factors for heart disease.

### **Column Details**
1. **Age**: Age of the individual (numeric).  
2. **Sex**: Biological sex (categorical: 0 = Female, 1 = Male).  
3. **ChestPainType**: Type of chest pain experienced (categorical: TA, ATA, NAP, ASY).  
4. **RestingBP**: Resting blood pressure in mmHg (numeric).  
5. **Cholesterol**: Serum cholesterol in mg/dL (numeric).  
6. **FastingBS**: Fasting blood sugar (categorical: 0 = <120 mg/dL, 1 = ≥120 mg/dL).  
7. **RestingECG**: Resting electrocardiogram results (categorical: Normal, ST, LVH).  
8. **MaxHR**: Maximum heart rate achieved during exercise (numeric).  
9. **ExerciseAngina**: Exercise-induced angina (categorical: 0 = No, 1 = Yes).  
10. **Oldpeak**: ST depression induced by exercise relative to rest (numeric).  
11. **ST_Slope**: Slope of the peak exercise ST segment (categorical: Up, Flat, Down).  
12. **HeartDisease**: Target variable indicating heart disease presence (categorical: 0 = No, 1 = Yes).  

## **Tools and Technologies**

- **Programming Language**: Python (Jupyter Notebook)  
- **Libraries**: NumPy, Pandas, Scikit-learn, Matplotlib 

## **Model Used**

- **Logistic Regression**: A statistical model used for binary classification tasks.

## **Workflow**

### 1. **Data Preprocessing**
   - Categorical variables were encoded using one-hot encoding.
   - Features were scaled to standardize the input values for the logistic regression model.

### 2. **Model Development**
   - The dataset was split into training and validation sets (80:20 ratio).
   - Logistic regression was applied to the training data to build the model.

### 3. **Model Evaluation**
   - Accuracy was measured on both training and validation datasets to ensure the model's reliability.
   - The model achieved an accuracy of **86%** on the validation dataset.

## **Conclusion**

The logistic regression model demonstrated strong predictive performance, achieving an accuracy of **86%**. By leveraging this model, healthcare professionals can better identify individuals at risk for heart disease and facilitate timely interventions.
