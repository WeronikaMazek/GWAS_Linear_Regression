# GWAS_Linear_Regression
This repository contains the workflow for analyzing genetic data associated with disease susceptibility. The project includes data preprocessing, exploratory data analysis (EDA), and multiple linear regression modeling to assess the association of allelic variants with risk scores while accounting for ancestry.

## Objective

The primary aim of this analysis is to determine the influence of specific allelic variants at different SNP loci on disease susceptibility. By developing and evaluating linear regression models, we identify genetic and demographic factors that contribute to risk scores and understand how these associations vary across ancestry groups.

**Key Highlights:**

SNP2 demonstrated the strongest association with the risk score, with the presence of the risk allele (allele 1) significantly increasing the risk score.

Ancestry was identified as an important covariate, influencing risk score distribution and enhancing model accuracy.

Models for SNP1, SNP3, SNP4, and SNP5 were excluded from further analysis due to low explanatory power or non-significant results.

## Folder Structure

### data_preprocessing_and_eda/

Exploratory data analysis (EDA) to understand risk score distribution and ancestry group characteristics.

*Key Findings:*

Risk scores exhibit an approximately normal distribution, justifying the use of linear regression models.

Stratification by ancestry revealed variations in risk score distributions and SNP allele frequencies.

Categorical ancestry groups (A1 and A2) exhibit differences in risk scores and allele distributions, particularly for SNP2.

Welch’s t-test showed a trend toward higher risk scores in Ancestry 2, although not statistically significant.

SNP2 showed distinct allele distribution patterns between ancestry groups, with more individuals in Ancestry 2 carrying the risk allele.

### linear_regression_models/

Includes Jupyter notebooks for developing and evaluating linear regression models for each SNP.

*Highlights:*

***SNP2 Linear Regression Model***

*Optimal configuration:* Adjusted for ancestry as a covariate.

*Key results:*

Risk allele (allele 1) had the strongest effect on risk score (Estimate: 2.1664, p-value: 8.11e-12).

Ancestry 2 was also a significant predictor (Estimate: 0.8361, p-value: 0.00384).

Adjusted R-squared: 38.46%, indicating a moderate level of explained variance.

*Visualisations:*

Scatter plots and interaction plots highlighting the relationship between SNP2 and risk score.

***Other SNP Models***

Models for SNP1, SNP3, SNP4, and SNP5 were excluded due to low explanatory power or lack of statistical significance.


### Libraries and Packages Used

### Core Libraries



