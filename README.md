# Covid-Analysis
This project is part of my data science portfolio and was created to showcase some of the skills I have learned since I started my journey into programming and data science!

### Introduction

The purpose of this project is to create a logistic regression classifier using Covid data. Patient characteristics, such as if they have pneumonia, diabetes, and their age, will be used to predict whether they will die from Covid. This type of prediction algorithm would be useful for a healthcare company, hospital, or even a Primary Care Physician for determining whether patients are more at risk for dying from Covid. This would allow them to potentially tailor their treatment based on their pre-existing conditions or characteristics.

### Methods Used
* Data Visualization
* EDA (Exploratory Data Analysis)
* Data Cleaning
* Logisitc Regression
* Feature Selection through Sequential Feature Selection
* Metrics (Accuracy, Precision, Recall, f1, confusion matrix)
* Regularization

### Technologies
* Pandas
* Python
* Matplotlib
* Jupyter Notebook
* SkLearn
* Seaborn
* mlxtend
* Chi2contingency

### Project Description
There is one file used in this project, which is a .csv file obtained from kaggle: `https://www.kaggle.com/datasets/meirnizri/covid19-dataset`. The initial file contains 21 columns including sex of the patient, age, pre-existing conditions such as diabetes, asthma, and tobacco use. The variable that will be predicted is whether the patient died, which is determined by a column that lists the date of death. 

Analysis was performed on how each pre-existing condition affects the mortality rate for patients with and without each condition. In addition, the number of pre-existing conditions for each patient was calculated and compared to the mortality rate. These simple calculations provided some insight into how the characteristics can influence whether a patient is at risk of dying from Covid.

After data cleaning and preparing the dataframe for analysis, the logistic regression will be fit and used to predict whether each patient died from Covid. Metrics used to determine how the classifier fits to the data include the accuracy, precision, and recall. In this case, recall is the most important because of the healthcare application of the data. Recall takes into account how many of the positives (patients that died) were predicted to be true, which means what percentage of the patients that died from Covid were predicted correctly. Accuracy is an important metric as well, but predicting whether or not a person that is not at risk is a lower priority.

### Conclusion

The analysis yielded favorable results, where almost 90% of people that died were able to be predicted.
It was shown that a higher number of pre-existing conditions can greatly increase your chances of dying from Covid and that each pre-existing conditions increases the mortality rate.

Potential areas where the logistic regression and general analysis could be improved include:

- Creating a model that predicts whether a patient is at high risk for hospitalization, or the ICU rather than death
- Adding additional variables could help with prediction (there was a variable for whether a patient tested positive, but the values were hard to decipher clearly: a simple yes or no for whether the patient tested positive would be best)
- Using a different classification algorithm, such as Decision Tree, KNN, K-Means, or Random Forest

