# Salary Exploration & Prediction Challenge Kaggle

## The challenge objective: tell a data story about a subset of the data science community represented in this survey, through a combination of both narrative text and data exploration. A “story” could be defined any number of ways, and that’s deliberate. The challenge is to deeply explore (through data) the impact, priorities, or concerns of a specific group of data science and machine learning practitioners. 

I decided to bo both the data exploration and build a predictive model using logistic regression to predict the salaries of survey participants.

This project involved:
- Data cleaning, wrangling and manipulation
  - Ordinal & Coordinal encoding 
- Imputation of missing values 
- Statistical Analysis 
- Data exploration
- Visualization
- Feature Reduction 
  - Tree Based Feature Importance 
  - Lasso for feature selection
- Hyperparameter Tuning
- Bias-Variance Tradeoff Analyisis

For more details on the challenge itself and the to source the input data please visit: [https://www.kaggle.com/c/kaggle-survey-2019](https://www.kaggle.com/c/kaggle-survey-2019)
  - input data: multiple_choice_responses.csv (20.33 MB)

In terms of the attached notebooks:
- The first notebook **KaggleSalary_DataSet.ipynb** takes the raw survey **multiple_choice_responses.csv** data and does some preliminary data manipulation which involves binning the target variable (Salary) before outputting a file named (Kaggle_Salary.csv)
- The second notebook **Kaggle_Salary_Predictions.ipynb** Is the stand-alone project where data exploration and the multi-class classification models are tested

## Key Findings & Results

<img src="https://github.com/kamalmukhalalaty/Kaggle-Salary-Predictions/blob/main/Overall%20Distribution%20of%20Salaries.png" width="500" height="300">

The distribution of salaries is very skewed with a very high number of data points for the lowest salary bracket as well as a "bump" in observations at the 100-125k salary bracket. This is due to a high number of respondents from various developping countries with a lower average/median salary (eg. India, which has a large number of survey participants as well while the bump at the 100-125k salary bracket can be seen as a somehwat normal distribution of salaries for the North America/USA alone.

To investgiate this further I have created the following plots:
<img src="https://github.com/kamalmukhalalaty/Kaggle-Salary-Predictions/blob/main/US%20vs%20India%20Salary%20Distributions.png" width="1500" height="300">
<img src="https://github.com/kamalmukhalalaty/Kaggle-Salary-Predictions/blob/main/US%20vs%20India%20Salaries%20W:R:T%20Education.png" width="1500" height="300">

Looking at this we can validate that there is somewhat normal distribution of salaries around 125-150k for the US alone with what could be some outliers in the 0-9,999 salrary bracket; and a skewed distrubtion at 0-10000 for indian respondants alone with some outliers at the >250,000$ salary bracket.

Geography has a large impact on salary, but due to the high variability in number of samples from each geographic region, this impact will be difficult for our models to learn and explain. 
