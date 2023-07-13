# Comparing Supervised Learning Performance: Project Overview
- The project aims to identify the most effective model for predicting the desired outcome. The insights gained from this analysis can guide decision-making and provide valuable recommendations for future applications in similar domains.
- To ensure robust and reliable evaluations, cross-validation techniques are employed, dividing the data into multiple folds and performing model training and testing across different subsets.
- Involves a comprehensive analysis of multiple supervised learning models, including Logistic Regression, Decision Tree Classifier, and Random Forest.
- The project also considers data preprocessing steps, such as handling class imbalance and feature selection, to optimize the models' predictive capabilities.

## Code and Resources Used
Python Version: 3.9<br>
Packages: pandas, numpy, sklearn, matplotlib, seaborn, imblearn<br>
Dataset: [Kaggle](https://www.kaggle.com/datasets/mnassrib/telecom-churn-datasets)

## Data Preprocessing
After loading the dataset, the data needed to be cleaned and preprocessed so that it was usable for our model. The following data preprocessing steps were performed:
- Handling Duplicate and Missing Values
- Feature Selection
- Encoding Categorical Variables
- Handling Class Imbalance

## EDA
After examining the data distributions and analyzing the value counts of the categorical variables, several notable observations were derived from the pivot tables. Here are a few key highlights.<br>
![Churn Distribution](image_url)<br>
![Confusion Matrix](https://github.com/farhanulf/Project_1/blob/main/Confusion%20Matrix.png)

## Training & Evaluating Models
To start, I divided the dataset into training and testing sets, using a test size of 20%. The evaluation of the models is based on several metrics, including accuracy, precision, recall, and ROC AUC. To ensure robust and reliable evaluations, I employed cross-validation techniques.

I tried three different models:
- LogisticRegression - widely used for classification tasks
- Decision Tree - splits the data based on the selected attributes
- Random Forest - combines multiple decision trees and aggregates their predictions to improve accuracy and mitigate overfitting

## Model Performance
After training and testing the models, here's the performance report of each models.<br>
![Comparison Performance Report](image_url)<br>

## Conclusion
Based on the performance report, it is evident that using the Random Forest model is the most effective approach to achieve a satisfactory score in predicting customer churn. Our treatment and model provide a high level of confidence, with a 93% accuracy in predicting customer churn correctly. Additionally, out of all the customers predicted to churn, 94% of them are indeed churned (True Positive), while the remaining 6% are not actually churned (False Positive).
