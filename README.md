# Impact of Lifestyle Factors on College GPA

A statistical analysis project examining how everyday lifestyle habits, such as study time, sleep, exercise, and attendance, relate to academic performance.

## Overview

This project investigates how lifestyle factors affect college students' GPA, using a synthetic dataset of 200 students designed through stratified sampling (by gender and major) to simulate a realistic undergraduate population. The goal was to identify which habits actually move the needle on academic performance, and which are more likely just noise.

**Note:** the dataset is synthetic, not collected from real students. It was generated to simulate plausible relationships between lifestyle habits and GPA, which made it possible to apply and validate statistical methods (hypothesis testing, correlation, regression, confidence intervals) in a controlled setting, without the noise or bias of a real-world sample.

## Key Findings

- **Study hours and attendance** were both significantly correlated with GPA (p < 0.0001 for each), while **sleep** (p = 0.58) and **exercise** (p = 0.88) showed no meaningful relationship.
- A linear regression model using study hours and attendance explained **35% of the variance in GPA (R² = 0.35)**, with study hours as the strongest individual predictor.
- The sample's average GPA was **3.05 (SD = 0.41)**, with a 95% confidence interval of **(2.99, 3.11)** for the true population mean.
- A two-sample hypothesis test found **no significant GPA difference between genders** (p = 0.37).

## Approach

- Generated a synthetic dataset of 200 students using stratified sampling by gender and major
- Cleaned the data, checking for missing values and detecting outliers using the IQR method
- Standardized numerical variables and encoded categorical data (gender) for analysis
- Calculated descriptive statistics, standard error, and a 95% confidence interval for mean GPA
- Ran correlation analysis and a linear regression model to identify the strongest predictors of GPA
- Applied hypothesis testing to evaluate individual predictors (attendance) and group differences (gender)
- Visualized relationships using scatterplots, histograms, and box plots

## Limitations & Future Work

Since the dataset is synthetic, it may not capture the variance or noise present in real-world data. Future versions of this analysis could incorporate additional factors like stress, social life, or work responsibilities, and ideally validate these findings against a real student sample.

## Tools & Libraries

Python, Pandas, NumPy, Matplotlib, SciPy, Seaborn

## Repository Contents

- [`notebook.ipynb`](./notebook.ipynb) — full analysis and code, viewable directly on GitHub
- [`presentation.pdf`](./presentation.pdf) — final presentation summarizing the approach and findings

## About This Project

This was completed as part of my B.S. in Data Science at the University of North Texas, as an exercise in applying statistical inference, correlation, and regression to a realistic dataset.
