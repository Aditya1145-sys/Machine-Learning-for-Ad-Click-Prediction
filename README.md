# Machine-Learning-for-Ad-Click-Prediction
A Machine Learning Project for Predicting User Click Behavior in Digital Advertising

# Overview
This project builds a Click-Through Rate (CTR) Prediction System using machine learning models on the advertising.csv dataset.
CTR prediction is a crucial task in digital marketing, enabling advertisers to:

Identify high-value users
Optimize ad targeting
Improve campaign ROI
Personalize user experience

We designed a complete ML workflow including data preprocessing, EDA, model training, evaluation, and insights.

# Objectives

- Primary Goals

Predict the probability that a user will click an advertisement.
Identify key factors influencing ad clicks.
Evaluate models using Accuracy, AUC, Recall, Log Loss.
Provide actionable recommendations for advertisers.

- Success Metrics

High AUC (ranking capability)
Low Log Loss (probability calibration)
High Recall (capturing true click cases)

# Dataset Description

The dataset includes demographic, behavioral, and contextual features.

- Key Features:

Daily Time Spent on Site (mins)
Age
Area Income
Daily Internet Usage (mins)
Ad Topic Line
City / Country
Clicked on Ad (target: 0 or 1)

# Data Preprocessing

Handled missing values
Encoded categorical variables
Scaled numerical features
Checked for class imbalance (Clicks ≪ Non-clicks)

# Exploratory Data Analysis (EDA)
- Key Observations

Users spending less time on site → more likely to click ads
Older users show higher CTR
Lower area income → higher engagement
High daily internet usage reduces click likelihood

# Machine Learning Models
The following models were implemented and compared:

Model	Purpose	Strength
Logistic Regression	Baseline model	Fast, interpretable
Decision Tree	Non-linear patterns	Good interpretability
Random Forest	Ensemble	Handles mixed data well
Gradient Boosting (XGBoost/GBM)	Advanced ensemble	Best performance

# Best Performing Model

- Gradient Boosting
Delivered the strongest performance across AUC, Recall, and Log Loss due to its ability to model non-linear interactions and feature relationships.

# Feature Importance
Key drivers of ad-click behavior:

Daily Time Spent on Site (inverse correlation)
Daily Internet Usage
Age
Area Income

# Key Insights

Lower site engagement users are more responsive to ads.
Older demographics show stronger click behavior.
Income level influences engagement patterns.
Ensemble models significantly outperform linear models.

# Conclusion
This project demonstrates how machine learning can turn raw advertising data into actionable insights, helping digital advertisers:

Optimize audience targeting
Improve campaign performance
Increase profitability
Personalize user experience

Through feature analysis, modeling, and evaluation, we established an effective CTR prediction pipeline ready for enhancement or deployment.
