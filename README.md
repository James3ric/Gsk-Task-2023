
# GSK-Task

## Project Overview
This project focuses on analyzing clinical trial data to evaluate the effectiveness of a new cancer treatment, Miraculon-B, compared to the standard of care. Using the provided datasets, the analysis aims to identify patient subgroups that benefit the most from the treatment. The analysis was conducted using R and/or Excel, leveraging techniques such as data cleaning, statistical aggregation, visualization, and predictive modeling.


## Solution Summary
The project was completed following these key steps:

### Data Preparation
- Read in the datasets.
- Removed duplicate rows and excluded pediatric data (patients aged <18).
- Handled missing values using appropriate imputation methods.

### Data Enrichment
- Calculated BMI for each patient using the formula:
  \[
  BMI = \frac{\text{Weight (kg)}}{\text{Height (m)}^2}
  \]
- Merged the clinical-study and protein-levels datasets on patient ID.

### Exploratory Data Analysis (EDA)
- Aggregated data to compare means for age, weight, and protein concentration across responders/non-responders and treatment groups.
- Created visualizations, including:
  - Boxplots of age, weight/BMI, and protein concentration by treatment response.
  - Additional visualizations segmented by treatment group.

### Predictive Modeling
- Built a logistic regression model to predict treatment response based on age, weight, BMI, protein concentration, and treatment group.
- Evaluated model performance using metrics like accuracy, precision, and recall.

### Findings and Insights
- Patients receiving Miraculon-B showed a higher response rate compared to the control group.
- Protein concentration emerged as a strong predictor of treatment response.
- Age and BMI also showed subtle predictive signals for specific subgroups.


## Tools and Libraries
- **R**: Data cleaning, visualization, and modeling.
  - Libraries used: `dplyr`, `ggplot2`, `caret`, `randomForest`.
- **Excel**: Initial data exploration and basic visualization.

## Key Insights
- Miraculon-B demonstrates significant effectiveness in shrinking solid tumors for certain patient subgroups.
- High protein concentration is a potential biomarker for predicting positive treatment response.
- Further analysis and validation are required to refine predictive capabilities and support regulatory submissions.

## Acknowledgments
Special thanks to GSK and DigData for providing this opportunity and resources to work on a real-world dataset and gain insights into analytical roles in the pharmaceutical industry.
