# ML_FluPRINT
# Evaluating Random Forest and XGBoost Models for Predicting High and Low Responders to Influenza Vaccination
---
## Project Description

Seasonal flu remains a major global health challenge despite decades of vaccination efforts. The effectiveness of flu vaccines varies significantly from year to year due to the virus’s high mutation rate, posing a serious threat to vulnerable populations.

Understanding what contributes to a strong immune response is crucial for improving vaccine design, but traditional immunology studies have been hindered by small sample sizes and limited analytical tools. With the emergence of large-scale immunoprofiling datasets like FluPRINT (1), which contains harmonised immune data from over 740 individuals across multiple clinical studies, there is an opportunity to apply ML to uncover predictors of vaccine response. These predictors or "biomarkers" can help us understand what drives high response, and apply the insights to improve vaccine design.

This project uses ML models (Random Forests and XGBoost) to predict vaccine responsiveness based on cellular, molecular, and serological features from the FluPRINT dataset. We address challenges such as class imbalance, high dimensionality, and missing data through preprocessing and apply SHAP-based interpretability to gain biological insights from model predictions. The goal is to identify potential biomarkers that could improve future vaccine development and personalisation.

## Dataset: FluPRINT

FluPRINT is a public database developed by Tomic et. al. (2019), and includes harmonised immune response data from over 740 individuals across multiple influenza vaccine studies (flu seasons 2007-2015). It combines:
- Cellular (e.g. flow cytometry, cell subset frequencies)
- Molecular (e.g. gene expression, cytokine levels)
- Serological (e.g. antibody titers)

The dataset contains over 3,000 features and is ideal for ML tasks due to its size, diversity, and complexity. It also includes demographic and clinical data, enabling analysis across age groups and health statuses.

Key challenges with FluPRINT:
- High dimensionality
- Missing values
- Class imbalance between high and low responders
- Multimodal data types

## Approach
We used a two-pronged approach to tackle this problem:
- Prediction: We built and trained two powerful machine learning models, Random Forest and XGBoost, to predict vaccine response.
- Interpretation: To avoid the "black box" problem, we used a tool called SHAP to understand why our models made their predictions. This allows us to identify the most influential biomarkers.

## How to run
This code provides a guide on how databases, such as FluPRINT, can be utilised for vaccine response analysis. It can be downloaded and edited as needed. The raw data has not been uploaded here but can be easily accessed via the link - https://fluprint.com/#/database-access. 
The code has been created in VScode, but can be run on any software with Python. Python 3.12.10 version was used for this analysis.

## References
1. Tomic A, Tomic I, Dekker CL, Maecker HT, Davis MM. The FluPRINT dataset, a multidimensional analysis of the influenza vaccine imprint on the immune system. Sci Data. 2019 Oct 21;6(1):214. 
