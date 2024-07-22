# Heart_Disease_Predictive_Model

## Project Overview
A supervised machine learning project for predicting heart disease. In this project, five optimized models were trained and tested both with and without PCA, alongside the development of an ensemble model.

## Objective
The objective of the model is to accurately predict the presence of heart disease in patients based on various medical and demographic features.

## Dataset
The dataset used in this project is the Cleveland Heart Disease dataset available on Kaggle. It contains 303 patient records with 14 attributes that provide valuable information about each patient. The dataset is considered reliable and has been extensively used in academic research for developing machine learning models for heart disease prediction.

## Features
- **Age**: The age of the patient.
- **Sex**: The sex of the patient (1 = male; 0 = female).
- **CP (Chest Pain Type)**: The type of chest pain experienced by the patient.
  - 0: Typical angina
  - 1: Atypical angina
  - 2: Non-anginal pain
  - 3: Asymptomatic
- **Trestbps (Resting Blood Pressure)**: The blood pressure of the patient while at rest (measured in mm Hg).
- **Chol (Serum Cholesterol)**: The cholesterol level in the patient's blood (measured in mg/dl).
- **FBS (Fasting Blood Sugar > 120 mg/dl)**: Whether the patient’s blood sugar level is greater than 120 mg/dl after fasting (1 = yes; 0 = no).
- **Restecg (Resting Electrocardiographic Results)**: Results from an ECG test performed while the patient is at rest.
  - 0: Normal results
  - 1: Abnormal results
  - 2: Probable or definite left ventricular hypertrophy
- **Thalach (Maximum Heart Rate Achieved)**: The highest heart rate achieved by the patient during physical activity.
- **Exang (Exercise Induced Angina)**: Whether the patient experienced angina during exercise (1 = yes; 0 = no).
- **Oldpeak (ST Depression Induced by Exercise Relative to Rest)**: A measure of abnormal heart activity during exercise compared to rest.
- **Slope (Slope of the Peak Exercise ST Segment)**: The slope of the peak exercise ST segment.
  - 0: Upsloping
  - 1: Flat
  - 2: Downsloping
- **Ca (Number of Major Vessels Colored by Fluoroscopy)**: The number of major blood vessels visible in a fluoroscopy image (0-3).
- **Thal (Thalassemia)**: A blood disorder status determined by a blood test.
  - 1: Normal blood flow
  - 2: Fixed defect
  - 3: Reversible defect
- **Target**: The diagnosis of heart disease (0 = absence; 1 = presence).

## Methodology
### Data Preprocessing
The dataset underwent several preprocessing steps to prepare it for analysis and modeling:
- Handling missing values using median imputation.
- Removing duplicates.
- Encoding categorical variables using one-hot encoding.
- Feature scaling using `StandardScaler`.
- Exploratory Data Analysis (EDA) to understand the distribution and relationships between features.
- Addressing class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

### Model Training and Evaluation
Several machine learning models were trained and evaluated, including:
- RandomForestClassifier
- XGBClassifier
- LGBMClassifier
- SVC (Support Vector Classifier)
- LogisticRegression

### Parameter Tuning and Optimization
GridSearchCV and RandomizedSearchCV were used for hyperparameter tuning. Principal Component Analysis (PCA) was applied to compare model accuracies.

### Ensemble Model
An ensemble model using VotingClassifier was created to combine the strengths of individual models for superior performance.

## Results
The model with the highest accuracy was the optimized SVC with PCA, achieving an accuracy of 0.935. The ensemble model also demonstrated improved accuracy in predicting heart disease.

## Conclusion
This project demonstrates a comprehensive approach to building a predictive model for heart disease diagnosis using machine learning techniques. The optimized SVC with PCA was the best-performing model, achieving an accuracy of 0.935.

## Acknowledgements
We extend our heartfelt gratitude to Dr. Abbass Rammal for his invaluable guidance and support throughout this course. Additionally, we thank the Lebanese American University (LAU) for providing the resources and environment conducive to academic and research excellence.

## Author
Abdul Rahman Al Zaatari

