# IITG.ai Recruitment Submission - Beyond The Box

This repository contains my submission for the **IITG.ai Freshers Recruitment (Beyond The Box)** challenge. It consists of two main parts: Exploratory Data Analysis (EDA) and a Machine Learning Hackathon task.

## Repository Contents

* **`Task1.ipynb`**: My solution for the EDA task.
* **`Task2.ipynb`**: My solution for the Hackathon prediction task.

## Task 1: Exploratory Data Analysis (EDA)

In the `Task1.ipynb` notebook, I analyzed the **Atlantis Citizens** dataset to understand the data's story before building any models.

**What I did:**

* Loaded and cleaned the dataset (`atlantis_citizens_final.csv`).
* Checked for missing values and analyzed columns like `Wealth_Index` and `Bio_Hash`.
* *Observation:* I found that `Bio_Hash` was unique for every citizen and wouldn't be useful for patterns, so I dropped it.
* *Observation:* I verified that missing wealth data was distributed evenly across different occupations.


* Created visualizations (like correlation heatmaps) to see how features like `House_Size`, `Life_Expectancy`, and `Occupation` relate to each other.

## Task 2: Hackathon (Modeling)

In `Task2.ipynb`, I built a machine learning model to solve the prediction problem for the hackathon.

**My Approach:**

* I used **Scikit-Learn** pipelines to handle data preprocessing cleanly.
* **Preprocessing:** Used a custom imputer strategy of grouping the data and then filling with the corresponding group median for missing values, `StandardScaler` for numerical features, and `Label Encoding` for categorical features.
* **Model:** I implemented a **Logistic Regression** model to train on the data and predict the outcomes for the hidden test set (`test_atlantis_hidden.csv`).


