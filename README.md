# Task-5-EDA
 Project Overview
Objective:
Perform an Exploratory Data Analysis (EDA) on the Titanic dataset to extract insights using statistical summaries and visual exploration.

Tools Used:

Python (Pandas, Seaborn, Matplotlib)

Dataset: train.csv from Titanic competition

Files Provided
train.csv: Main dataset used for analysis

test.csv: Held out for future use (not used in this EDA)

gender_submission.csv: Also for future modeling (not relevant in EDA)

Steps Performed
1. Loaded the Dataset
Used pandas to load and inspect the Titanic training dataset.

2. Initial Data Checks
.info(), .describe(), .isnull().sum() to explore:

Total entries

Data types

Missing values

Basic statistics

3. Target Variable: Survival Distribution
Bar plot of Survived column using sns.countplot

Observation: Majority did not survive

4. Categorical Analysis
Sex vs Survived (countplot):

Females had a significantly higher survival rate.

Pclass vs Survived (countplot):

1st class passengers were most likely to survive.

5. Numerical Features Analysis
Age Distribution:

Histogram revealed most passengers were young adults.

Boxplot of Age by Class:

Younger passengers were more common in 3rd class.

6. Missing Values Visualization
Used sns.heatmap() to show missing data:

Cabin had the most missing values.

Age had several missing entries.

7. Pairplot of Key Features
Pairplot of Survived, Pclass, Age, and Fare

Helped visualize clusters and separability

8. Correlation Matrix
Heatmap of correlations between numerical features

Key correlations with Survived:

Sex (strongest)

Pclass

Fare


Summarizes observations and insights from each step

Provides a conclusion and next-step suggestions

Summary of Insights
Sex and Pclass are key predictors of survival.

Fare and Age have weaker correlations.

Cabin is missing too much data for analysis.

Further steps include:

Handling missing values

Feature engineering (e.g., family size)

Preparing for modeling and predictions
