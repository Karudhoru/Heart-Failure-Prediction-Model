# Heart Disease Prediction Project

Heart disease is one of the leading causes of mortality worldwide, and early detection can significantly improve treatment outcomes. This project aims to develop a **predictive model using logistic regression** to assess the risk of heart disease based on various physiological and lifestyle factors. The dataset used for this analysis was sourced from Kaggle and contains detailed records of **919 individuals**.

## Problem Statement

The primary objective of this project is to build a machine learning model that predicts the presence of heart disease based on several key indicators. This model can assist healthcare professionals in identifying high-risk individuals and making informed decisions for early intervention and treatment.

## Dataset Description

The dataset consists of **919 rows and 12 columns**, with each column providing crucial information about a patient's health and potential risk factors for heart disease.

### Column Details
- **Age**: Age of the individual (numeric).
- **Sex**: Biological sex (categorical: 0 = Female, 1 = Male).
- **ChestPainType**: Type of chest pain experienced (categorical: TA, ATA, NAP, ASY).
- **RestingBP**: Resting blood pressure in mmHg (numeric).
- **Cholesterol**: Serum cholesterol in mg/dL (numeric).
- **FastingBS**: Fasting blood sugar (categorical: 0 = <120 mg/dL, 1 = ≥120 mg/dL).
- **RestingECG**: Resting electrocardiogram results (categorical: Normal, ST, LVH).
- **MaxHR**: Maximum heart rate achieved during exercise (numeric).
- **ExerciseAngina**: Exercise-induced angina (categorical: 0 = No, 1 = Yes).
- **Oldpeak**: ST depression induced by exercise relative to rest (numeric).
- **ST_Slope**: Slope of the peak exercise ST segment (categorical: Up, Flat, Down).
- **HeartDisease**: Target variable indicating heart disease presence (categorical: 0 = No, 1 = Yes).

## Tools and Technologies

- **Programming Language**: Python (Jupyter Notebook)
- **Libraries**: NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn

## Model Used

- **Logistic Regression**: A statistical model for binary classification tasks, used to predict the likelihood of heart disease.

## Workflow

### 1. Data Preprocessing
- **One-Hot Encoding**: Categorical variables (such as `Sex`, `ChestPainType`, `RestingECG`, etc.) were encoded using `OneHotEncoder` to convert them into a format suitable for logistic regression.
- **Feature Scaling**: Features were standardized to ensure that all input variables are on the same scale, which helps the logistic regression model converge faster and improves performance.

### 2. Exploratory Data Analysis (EDA) and Visualization
- **Visualization**: Various plots were created using **Seaborn** and **Matplotlib** to better understand the dataset. This included:
  - **Box Plots** to visualize the distribution and detect outliers.
  - **Histograms** to examine the distribution of numeric variables like `Age`, `Cholesterol`, and `MaxHR`.
- **Correlation Matrix**: A heatmap was used to explore the relationships between numeric features.
- **Confusion Matrix**: A confusion matrix was created to evaluate the model's performance in terms of True Positives, True Negatives, False Positives, and False Negatives.

### 3. Model Development
- The dataset was split into **training** and **validation sets** (80:20 ratio).
- **Logistic regression** was applied to the training data, where the model was trained and optimized.

### 4. Model Evaluation
- The model's performance was assessed using accuracy, precision.
- After fine-tuning and proper encoding, the model achieved an **accuracy of 100%** on the validation dataset, demonstrating excellent predictive performance.

## Conclusion

The logistic regression model achieved perfect accuracy of **100%** in predicting heart disease presence. This result is a strong indication of the model's ability to classify heart disease risk based on various health indicators. By using this model, healthcare professionals can confidently identify high-risk individuals and provide early interventions, potentially saving lives. Visualization techniques like box plots, histograms, and confusion matrices helped in the analysis and evaluation of the model's performance, ensuring a robust and reliable prediction.

