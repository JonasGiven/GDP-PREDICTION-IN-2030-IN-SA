# Predicting GDP Growth Based on Educational Pass Rates: An Analytical Approach Using Historical Data

## Overview
This project explores the correlation between educational outcomes, specifically the official matric pass rates, and economic performance in South Africa. By analyzing historical data from 1995 to 2023, I aim to develop a predictive model to estimate the future GDP based on variations in the pass rates. The project culminates in predicting the GDP for the year 2030, assuming a 10% increase in the matric pass rate from 2022.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Collection](#data-collection)
3. [Data Exploration](#data-exploration)
4. [Data Preparation](#data-preparation)
5. [Model Training](#model-training)
6. [Prediction](#prediction)
7. [Results](#results)
8. [Conclusion](#conclusion)
9. [Acknowledgments](#acknowledgments)

## Introduction
Despite significant investments in education, understanding the direct relationship between educational outcomes and economic growth remains complex. This project investigates the correlation between historical pass rates and GDP growth to predict future GDP changes based on educational improvements. By employing machine learning techniques, this analysis aims to provide insights into how educational advancements can drive economic growth, aiding policymakers in informed decision-making.

## Data Collection
The data for this project was collected from a publicly available sources.<br/>
Official matric pass rate was obtained from [Mybroadband](https://mybroadband.co.za/news/government/431106-south-africas-matric-pass-rate-official-vs-real-from-1995-to-2021.html) and [South African government](https://www.gov.za/blog/2023-matric-results).
GDP figures for South Africa from 1995 to 2023 was collected from [Macrotrends](https://www.macrotrends.net/global-metrics/countries/ZAF/south-africa/gdp-gross-domestic-product). The dataset is stored in a CSV, [SA_matricratepass_gdp](https://github.com/JonasGiven/Datasets).

## Data Exploration
I started by examining the dataset to understand its structure and identify any potential outliers. A box and whisker plot was used to visualize the distribution of both the official matric pass rate and GDP values. The observations indicated a generally high pass rate and significant economic growth over the years, suggesting a potential positive correlation between the two variables.

## Data Preparation
The dataset was cleaned by removing any outliers, specifically the data for the year 2023, which was identified as an outlier. We then split the data into features (year and official matric pass rate) and the target variable (GDP). The data was further divided into training and testing sets to train the machine learning model.

## Model Training
A RandomForestRegressor model was used for this project due to its robustness and ability to handle complex relationships between variables. The model was trained using the training data, with the year and official matric pass rate as features and the GDP as the target variable. The training process involved splitting the data into training and testing sets, fitting the model, and ensuring that the feature names were consistent throughout.

## Prediction
To predict the GDP for 2030, I created a new input data point with the year set to 2030 and the official matric pass rate increased by 10% from the 2022 value. This input data was fed into the trained model to obtain the GDP prediction for 2030.

## Results
The model predicted that the GDP for South Africa in 2030, assuming a 10% increase in the official matric pass rate from 2022, would be approximately $394.42 billion.

## Conclusion
This project successfully demonstrated a positive correlation between educational outcomes and economic performance in South Africa. By using historical data and machine learning techniques, we were able to predict the future GDP based on an increase in the matric pass rate. These insights can help policymakers understand the potential economic benefits of investing in education.

## Acknowledgments

I would like to thank the creators of the dataset and the contributors to the various libraries used in this project, including pandas, numpy, matplotlib, seaborn, scikit-learn, and mlflow. Their tools and resources made this project possible.

## Contact

For any questions or further information, please contact me via [email](jonasgiven18@gmail.com).

Thank you for exploring this project! I hope it provides valuable insights into the relationship between education and economic growth in South Africa.
