# Obesity and Cancer: the association between body fat composition derived from DEXA scans and cancer and all-cause mortality risk
This was a 3-month long R-based MSc dissertation project.

## Project aim
Obesity is a well-established risk factor for health which we have seen a rise in globally. Cancer is also a major global health issue and links to obesity and at least 13 cancer types have been established. There is therefore a growing interest in studying these obesity-cancer links. BMI is the most commonly used in studies, however since it is does not distinguish between body fat and lean mass and rather acts as a summary statistic, researchers have started to look at alternatives such as DEXA scan derived data as a potentially more accurate metric for measurement of body fat. This study investigated whether DEXA-derived fat measures are associated with obesity-related cancer mortality and all-cause mortality risk.

## Data 
The UK Biobank. The cohort used in this study was the cohort of patients for which DEXA scans had been completed (47,711 participants).

## Statistical methods used
Stratified by sex due to known body composition differences.

Time to event analysis using standard cox models for all-cause, and fine and grey models for events with competing risks.

Exposure: body composition metrics: VAT mass, total fat mass, total fat free mass and total tissue fat %

Follow-up period- time from DEXA scan to event or censoring. Median of 4.6 years. 

Events- all-cause mortality, obesity-related cancer mortality, non-obesity-related cancer mortality and non-cancer specific mortality.

Confounders- adjusted for age, socioeconomic status (townsend deprivation index), lifestyle factors (e.g. smoking status, alcohol intake and physical activity) and comorbidities (e.g. cancer, diabetes)

## Statisical Packages used

Statistical analysis was conducted within the UK Biobank Research Analysis Platform (UK-
RAP) in order to be in compliance with the data confidentiality and governance guidelines provided.

The analysis was performed using R statistical software (v4.4.0; R core team 2024).

base r functions and the dplyr package (v1.1.4; Wickham et al 2023). 

ggplot2 package (v3.5.2; Wickham 2016)

mice package (v3.18.0; Burren and Groothuis-Oudshoorn 2011)

survival package (v3.8.3; Therneau 2024) 

cmprsk package (v2.2.12; Gray 2024)

