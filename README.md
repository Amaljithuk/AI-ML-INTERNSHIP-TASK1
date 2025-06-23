# AI-ML-INTERNSHIP-TASK1

Task Overview

This repository contains the solution for Task 1 of the Elevate AI & ML Internship. The objective is to clean and preprocess the Titanic dataset to prepare it for machine learning, using Python in a Jupyter Notebook with libraries like Pandas, NumPy, Matplotlib, Seaborn, and scikit-learn.

Steps Performed





Data Exploration: Imported the Titanic dataset and analyzed its structure, data types, and missing values using df.info() and df.isnull().sum().



Handling Missing Values:





Filled missing Age values with the median.



Filled missing Embarked values with the mode.



Dropped the Cabin column due to excessive missing data.



Encoding Categorical Features:





Applied label encoding to Sex (male: 0, female: 1).



Applied one-hot encoding to Embarked, creating dummy variables (Embarked_C, Embarked_Q, Embarked_S).



Feature Scaling: Standardized numerical features (Age, Fare, SibSp, Parch) using StandardScaler to ensure zero mean and unit variance.



Outlier Detection and Removal:





Visualized outliers using boxplots for numerical features.



Removed outliers using the Interquartile Range (IQR) method.



Generated before-and-after boxplots to show the effect of outlier removal.



Output: Saved the cleaned dataset as Titanic-Cleaned-Dataset.csv.

Files





titanic_data_cleaning.ipynb: Jupyter Notebook implementing the data cleaning and preprocessing steps.



Titanic-Dataset.csv: Original Titanic dataset.



Titanic-Cleaned-Dataset.csv: Preprocessed dataset after cleaning.



boxplots_before_outlier_removal.png: Boxplots showing numerical features before outlier removal.



boxplots_after_outlier_removal.png: Boxplots showing numerical features after outlier removal.



README.md: This documentation file.

Tools Used





Python 3



Jupyter Notebook



Pandas



NumPy



Matplotlib



Seaborn



scikit-learn

How to Run





Clone this repository:

git clone https://github.com/Amaljithuk/AI-ML-INTERNSHIP-TASK1.git



Install required dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn jupyter



Launch Jupyter Notebook:

jupyter notebook



Open titanic_data_cleaning.ipynb in the Jupyter interface.



Run all cells in the notebook to:





Generate the cleaned dataset (Titanic-Cleaned-Dataset.csv).



Save boxplot visualizations (boxplots_before_outlier_removal.png, boxplots_after_outlier_removal.png).



Display dataset information and the first few rows of the cleaned data.

Notes





The notebook addresses Pandas FutureWarning for inplace=True in fillna by using explicit assignments (e.g., df['Age'] = df['Age'].fillna(df['Age'].median())).



The cleaned dataset is ready for machine learning tasks, with numerical features standardized and categorical features encoded.



Visualizations help assess the impact of outlier removal on the data distribution.



Ensure the Titanic-Dataset.csv file is in the same directory as the notebook before running.

Submission

This repository is submitted for Task 1 of the Elevate AI & ML Internship, completed on June 23, 2025, within the 10:00 AM to 10:00 PM submission window.
