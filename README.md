# Hospital Readmission Analysis

## Table of Contents

- [1. Business Problem Definition and Data Description](#1-business-problem-definition-and-data-description)
  - [1.1 Business Problem - Introduction and Motivation](#11-business-problem---introduction-and-motivation)
  - [1.2 Data Source - Description](#12-data-source---description)
- [2. Project Objective/Proposal](#2-project-objectiveproposal)
- [3. Project Contributors](#3-project-contributors)
- [4. Project Overview](#4-project-overview)

## 1. Business Problem Definition and Data Description

### 1.1 Business Problem - Introduction and Motivation

Hospitals have a strong incentive to avoid patient readmissions due to both reputational and financial reasons. Readmission, defined as patients being re-admitted to a hospital within 30 days of their initial visit, can lead to complications such as reduced insurance coverage, particularly from programs like Medicare. This can result in significant financial issues for both hospitals and patients themselves. The objective of this project is to analyze data to identify patterns and factors that contribute to readmissions, with the aim of reducing readmission rates by taking preventive measures for at-risk patients.

#### Project Objective/Proposal

The primary objective of this project is to analyze demographic information, diabetic diagnoses, and medication histories to gain insights into their impact on readmission types. By understanding the factors that influence readmission, we can take informed actions to reduce the occurrence of readmissions.

### 1.2 Data Source - Description

- **Data Source**: [Diabetic Patient Data](https://data.mendeley.com/datasets/nntck7ddgt/2)

The dataset used for this analysis is sourced from Clinical and Translational Research at Virginia Commonwealth University. It provides 10 years (1999-2008) of clinical care data from 130 US hospitals and integrated delivery networks. The dataset includes information on inpatient encounters of diabetic patients with durations ranging from 1 to 14 days. Each encounter is labeled to indicate whether the patient was readmitted (No, > 30 days, < 30 days). This dataset contains 55 variables and 101,766 instances. Some of the variables may have missing values marked as '?'. The variables can be broadly categorized into four segments:

1. Demographic information
2. Diabetic diagnoses
3. Medication history
4. Other relevant data

## 2. Project Objective/Proposal

The core objective of this project is to explore the provided dataset and analyze the data to gain insights into the factors influencing readmissions. Our analysis will focus on demographic attributes, diabetic diagnoses, and medication histories. We aim to answer questions such as:

- What demographic factors are associated with higher readmission rates?
- Are specific diabetic diagnoses more likely to result in readmissions?
- Does medication history play a significant role in readmission rates?

By answering these questions, we can provide healthcare professionals and institutions with valuable insights to help them make informed decisions and take actions to reduce readmission rates.

## 3. Project Contributors

This project was collaboratively developed by the following contributors:

- Victor Floriano
- Ya Chu Hsu
- Honglin Jiang
- Luca Matteucci
- Adarsh Prajapat
- Jessica Tong

## 4. Project Overview

This report presents a comprehensive analysis of a medical dataset with the aim of understanding the factors influencing hospital readmission for diabetic patients. The analysis begins with extensive data exploration, examining variables such as age, gender, A1C results, and medication usage to uncover patterns and correlations. Notably, it reveals a decrease in A1C abnormal results with patient age and a gender-based disparity in A1C readings. The study further delves into the length of hospital stays, diagnoses, and the relationship between these variables and readmission rates. Next, predictive machine learning models are introduced, including a Random Forest model, Decision Trees model, and Logistic Regression. These models are evaluated based on performance metrics such as accuracy, recall. Both the Decision Tree and the Random Forest models emphasize important features, while the Decision Trees model provides insights into how decisions are made. The Logistic Regression model offers a straightforward binary classification approach. This holistic approach provides valuable insights for medical practitioners and stakeholders in predicting patient readmission and improving patient care and outcomes.

---

This updated README now includes the information about the project's overview, which highlights the analysis and the machine learning models used. Feel free to further customize this template as needed for your project.
