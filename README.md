# Salary Prediction Challenge Kaggle

The challenge objective: tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration. A “story” could be defined any number of ways, and that’s deliberate. The challenge is to deeply explore (through data) the impact, priorities, or concerns of a specific group of data science and machine learning practitioners. 

I decided to bo both the data exploration and build a predictive model using logistic regression to predict the salaries of survey participants.

This project involved:
- Data cleaning, wrangling and manipulation
- Imputation of missing values 
- Statistical Analysis 
- Data exploration
- Visualization
- Hyperparameter Tuning
- Bias-Variance Tradeoff Analyisis

For more details on the challenge itself and the to source the input data please visit: [https://www.kaggle.com/c/kaggle-survey-2019](https://www.kaggle.com/c/kaggle-survey-2019)
  - input data: multiple_choice_responses.csv (20.33 MB)

In terms of the attached notebooks:
- The first notebook **KaggleSalary_DataSet.ipynb** takes the raw survey **multiple_choice_responses.csv** data and does some preliminary data manipulation which involves binning the target variable (Salary) before outputting a file named (Kaggle_Salary.csv)
- The second notebook **Kaggle_Salary_Predictions.ipynb** Is the stand-alone project where data exploration and the multi-class classification models are tested


