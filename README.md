# Gsk-Task

Project Overview
This project focuses on analyzing clinical trial data to evaluate the effectiveness of a new cancer treatment, Miraculon-B, compared to the standard of care. Using the provided datasets, the analysis aims to identify patient subgroups that benefit the most from the treatment. The analysis was conducted using R and/or Excel, leveraging techniques such as data cleaning, statistical aggregation, visualization, and predictive modeling.

Files Included
clinical-study.csv: Clinical trial data with patient demographics, treatment groups, and response outcomes.
protein-levels.csv: Protein concentration data for patients, potentially predictive of treatment response.
DigData–Step-Up-Presentation.pptx: Presentation summarizing the results.
excel_cheatsheet.pptx: Excel guidance document.
step_up_with_r.html: R task guide.
analytical_roles.pdf: Document discussing analytical roles in the pharma industry.
Solution Summary
The project was completed following these key steps:

Data Preparation

Read in the datasets.
Removed duplicate rows and excluded pediatric data (patients aged <18).
Handled missing values using appropriate imputation methods.
Data Enrichment

Calculated BMI for each patient using the formula:
𝐵
𝑀
𝐼
=
Weight (kg)
Height (m)
2
BMI= 
Height (m) 
2
 
Weight (kg)
​
 
Merged the clinical-study and protein-levels datasets on patient ID.
Exploratory Data Analysis (EDA)

Aggregated data to compare means for age, weight, and protein concentration across responders/non-responders and treatment groups.
Created visualizations, including:
Boxplots of age, weight/BMI, and protein concentration by treatment response.
Additional visualizations segmented by treatment group.
Predictive Modeling

Built a logistic regression model to predict treatment response based on age, weight, BMI, protein concentration, and treatment group.
Evaluated model performance using metrics like accuracy, precision, and recall.
Findings and Insights

Patients receiving Miraculon-B showed a higher response rate compared to the control group.
Protein concentration emerged as a strong predictor of treatment response.
Age and BMI also showed subtle predictive signals for specific subgroups.
Presentation

Results and insights were compiled into a PowerPoint presentation.
A 3-minute demo video was recorded to summarize the project.
Tools and Libraries
R: Data cleaning, visualization, and modeling.
Libraries used: dplyr, ggplot2, caret, randomForest.
Excel: Initial data exploration and basic visualization.
How to Use
Clone this repository to your local machine.
Open and explore the provided datasets (clinical-study.csv, protein-levels.csv).
If using R:
Load the project files into RStudio (Posit Cloud).
Run the analysis scripts following the steps outlined in step_up_with_r.html.
If using Excel:
Follow the guidelines in excel_cheatsheet.pptx for analysis.
Review the final results and visualizations in the presentation (DigData–Step-Up-Presentation.pptx).
Key Insights
Miraculon-B demonstrates significant effectiveness in shrinking solid tumors for certain patient subgroups.
High protein concentration is a potential biomarker for predicting positive treatment response.
Further analysis and validation are required to refine predictive capabilities and support regulatory submissions.
Acknowledgments
Special thanks to GSK and DigData for providing this opportunity and resources to work on a real-world dataset and gain insights into analytical roles in the pharmaceutical industry.
