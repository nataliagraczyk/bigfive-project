# Employability analysis using logistic regression model
The analysis below is part of the Master's thesis defended at University of Warsaw in June 2022 by Natalia Graczyk.

Title: *Relationship of personality traits with the probability of being employed in Poland*

## Project Objective
The aim of this study was to examine the relationship of Big Five personality traits with the likelihood of employment in Poland. 

There is no doubt that cognitive skills (such as education or experience) have a significant impact on people's situation in the labour market and this is proven by numerous scientific studies. However, referring only to a person's cognitive skills in the context of employment, is a somewhat simplistic view of their skills in general. 

Knowing the relationship between an individual's non-cognitive skills (i.e. personality traits) and the likelihood of getting a job would provide more information on the employability of individuals and thus contribute to a better understanding of labour market processes.

## Installation

1. Create a virtual environment:
```
 python3 -m venv .venv
```
2. Activate the virtual environment:
```
.venv\Scripts\Activate.ps1
```
3. Install dependencies:
```
pip install -r requirements.txt
```

## Data

The analysis was based on individual data from the from the Programme for the International Assessment of Adult Competencies (PIAAC) by OECD for Poland, as well as its national follow-up (postPIAAC), in which additional information was collected from those who participated in the first edition of the survey. 

This data was chosen because it is the only survey on the labour market situation of Poles that provides information not only on the cognitive skills of respondents, but also on their personality traits.

More information on the study itself can be found on the following website: [oecd-piaac](https://www.oecd.org/skills/piaac/)

## Methods
The relationship of personality traits with the probability of employment was estimated using logistic regression model, in which the employment status during post-PIAAC study is the dependent variable, and takes the values of 1 in case of being employed and 0 in case of being unemployed or professionally inactive during that period. 

It was decided to use the logit model because for the purposes of this study, it was important to compare the model with the results of other studies conducted in other countries.

### Stages of the project:
- Exploratory Data Analysis
- Data cleaning and feature engineering
- Train-Test Split
- Feature Scaling
- Handling imbalanced data using SMOTE
- Multicollinearity check
- Logistic Regression Model
- Model Evaluation
- Analysing the coefficients
