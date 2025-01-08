# St Stephens Heart Disease EDA and ML Prediction

![causes-heart-disease-diagram-100747333](https://github.com/user-attachments/assets/213f64fc-521a-4787-adad-b672febb50bd)

## Project Description:
St Stephen’s Hospital and Maternity is a private owned hospital located in Lagos, Nigeria. It was founded in 1972 by an astute medical professional. The hospital provides a wide range of medical services, including but not limited to general medicine, surgery, pediatrics, obstetrics and gynecology. The Hospital is known for its state-of-the-art facilities, modern equipment, and highly skilled medical professionals. 
It was then observed that an increasing number of patients presented themselves with complains including chest pains, blood pressure related issues, cholesterol level declines and stroke in some cases,  hence an inquiry into the possibility of patients being at risk of a heart disease. 

This project focuses on exploring and analyzing a heart disease dataset, using exploratory data analysis (EDA) and machine learning techniques to predict the likelihood of heart disease in individuals. 
The primary goal is to uncover key patterns and relationships within the data that can assist in identifying at-risk patients. Through Exploratory Data Analysis, I gained insights into factors such as age, cholesterol levels, blood pressure, and other clinical attributes. I then applied machine learning algorithms, to predict the probability of a patient having a heart disease, aiming to improve early detection and inform better clinical decision-making.

## Dataset Description
Source: Collected data from approximately 5500 medical patients evaluated for heart disease.

Target Variable: Binary outcome indicating heart disease presence (1) or absence (0).

Independent Variables: information believed to have an influence on the outcome to predict. Eg Age, Cholesterol level, Blood Pressure etc

This Heart Disease Dataset contains information about 5500 medical patients evaluated for the presence of heart disease. Each record provides details on different patient characteristics that may influence the likelihood of a heart disease diagnosis. The dataset includes the following attributes:

## Feature Description
Age - in years.

Sex - (M=male, F= female).

ChestPainType - (TA:typical angina. ATA: atypical angina, NAP:non-angina, ASY: asymptomatic).

RestingBP- Resting Blood Pressure.

Cholesterol- Serum Cholesterol in mg/dl.

FastingBS - (Fasting Blood Sugar > 120mg/dl)(1 =true, 0= false)

RestingECG- Resting Electrocardiographic Results

MaxHR - Maximum Heart Rate Achieved

ExerciseAngina - Exercise Induced Angina (Y = yes, N= no).

Oldpeak - ST depression induced by exercise relative to rest

ST_Slope- the slope of the peak exercise ST segment

HeartDisease - Have disease or not (1=yes, 0 = no) 

## Data Preparation (EDA)
*   Loading the Data
*   Data Cleaning
*   Handling Missing Data
*   Model Building and Predictions
*   Summarizing and Visualization


## Model Evaluation Summary
Based on the displayed results, here’s an evaluation of the model’s performance:
1. Accuracy: The logistic regression model gave an 86% accuracy and a precision of 85% which does not appear as best as both false positives and false negatives can have serious implications. A further review with random forest did better with a 100% accuracy and precision.
2. Confusion Matrix: The Logistic Regression Model gave True Negatives (TN): 407 (correctly predicted as "No heart disease"). False Positives (FP): 91 (incorrectly predicted as "Heart disease" when they don’t have it). True Positives (TP): 549 (correctly predicted as "Heart disease"). False Negatives (FN): 55 (incorrectly predicted as "No heart disease" when they actually have it). However, the Random Forest Classifier gave an accurate prediction required considering the nature of project involved.

## Analysis Summary
In this analysis, I aimed to build a machine learning model that can predict the
Likelihood of a person having a heart disease based on the given features. My workflow included data preparation, model selection/building, and model evaluation using logistic regression and other Machine Learning Algorithms to determine the most suitable model to use.  
Below is a summary of each step:

1. Data Cleaning and Transformation
I checked for missing values and data inconsistencies in the dataset, standardizing data to maintain model integrity. Some outliers were noted and converted to their positive counterparts as they were suspected to be entry errors. This ensured logical consistency across the dataset.

2. Model Building
The data was split into training and testing sets, with 80% of the data used for training the model and 20% for testing. This provided an unbiased evaluation of the model’s performance. I reviewed logistic regression and further examined 7 other machine algorithms to determine the model with optimal effectiveness in other to reduce issues arising from false predictions as human lives are involved and the project essence is to achieve early detection and avoid needless deaths.

3. Model Evaluation
The logistic regression is 86% accurate and a precision of 85% which doesnt appear as best, a further review of other models is shown below with random forest doing better with a 100% accuracy and precision.

## Conclusion
This analysis provided a comprehensive workflow for building a heart disease classification model using various machine learning algorithms to determine the most effective classifier based on four key metrics: Accuracy, Precision, Recall, and ROC Score. The results provide clear insights into the performance of each model. The XGBoost Classifier, Random Forest, and Decision Tree consistently outperformed other models across all metrics, achieving perfect scores (100%) in Accuracy, Precision, Recall, and ROC Score. These models demonstrated accurate predictions, correctly identifying true positives, and distinguished between classes with high reliability.
