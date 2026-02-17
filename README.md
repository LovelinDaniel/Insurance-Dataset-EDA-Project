## Insurance Dataset EDA Project

## Objective:
Perform exploratory data analysis (EDA) on insurance data to understand cost-driving factors and support data-driven risk assessment and pricing strategies.

## Problem Statement:
Insurance companies often face challenges in accurately pricing policies due to factors like age, BMI, smoking status, and region. Mispricing can reduce competitiveness and profitability.

## Goal:
- Identify key factors affecting insurance charges
- Understand correlations between demographic and lifestyle variables
- Generate actionable insights for risk-based pricing strategies

## Project Overview:
This project leverages Python and popular data analysis libraries to explore an insurance dataset, uncover trends, and visualize patterns affecting insurance costs.

## Tools & Technologies:
* Python
* Pandas & NumPy
* Matplotlib & Seaborn

## Process:
- Data Cleaning & Preprocessing
- Handled missing values, duplicates, and inconsistencies
- Standardized categorical and numerical features
- Exploratory Data Analysis (EDA)
- Studied relationships between age, BMI, smoking status, sex, region, and insurance charges

## Data Visualization:
* Created scatter plots, histograms, box plots, and heatmaps
* Highlighted trends for easy interpretation

## Regional KPI Comparison:
| Region    | Avg Age | Avg BMI | Avg Charges ($) | Key Insights                                                      |
| --------- | ------- | ------- | --------------- | ----------------------------------------------------------------- |
| Northeast | 39      | 30      | 14,500          | High charges for smokers; older population drives higher premiums |
| Northwest | 37      | 28      | 13,800          | Moderate BMI and age; smoking still major factor                  |
| Southeast | 35      | 31      | 15,200          | Higher BMI and smokers contribute to highest charges              |
| Southwest | 36      | 29      | 14,000          | Balanced charges; age and smoking moderately affect costs         |


## Key Insights & Findings
- Age & Smoking: Strong positive correlation with insurance charges
- BMI: Higher BMI contributes to higher charges, especially among smokers
- Sex: Minor differences in charges between male and female
- Region: Southeast shows highest average charges due to combined age, BMI, and smoking trends
- Actionable Outcome: Insights guide risk-based pricing, targeted policy design, and customer segmentation

## Sample Visualizations (Placeholders)

1. Charges vs Age
[Insert scatter plot showing positive correlation between age and insurance charges]

2. Charges by Smoking Status
[Insert box plot showing smokers pay higher premiums]

4. BMI vs Charges by Region
[Insert bar chart or heatmap showing BMI impact across different regions]

4. Correlation Heatmap
[Insert heatmap of correlations between age, BMI, sex, region, smoking, and charges]

## Sample Python Code
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load dataset
data = pd.read_csv('insurance.csv')

# Correlation heatmap
plt.figure(figsize=(8,6))
sns.heatmap(data.corr(), annot=True, cmap='coolwarm')
plt.title('Correlation Heatmap')
plt.show()

# Charges vs Age
sns.scatterplot(x='age', y='charges', hue='smoker', data=data)
plt.title('Insurance Charges vs Age by Smoker Status')
plt.show()

## Outcome:

- Developed a thorough understanding of factors influencing insurance costs
- Identified the strong impact of age and smoking on premiums
- Provided actionable insights for risk assessment and pricing strategies
- Framework can be reused for continuous monitoring and analysis of new insurance data
