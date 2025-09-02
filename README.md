Analysis of Reported Rape Cases in India (NCRB Dataset)
1. Problem Statement
Sexual violence is a serious public health and social issue in India, affecting both children and adults. There are significant variations in reported rape cases across states and age groups.

2. Task Chosen
Analyze a real-world public health and crime dataset from NCRB.
Steps performed:
Data cleaning and preprocessing
Exploratory Data Analysis (EDA) with visualizations
Feature engineering to reveal patterns
Summary of actionable insights

3. Features Implemented
Core Features:
Data Cleaning: Removed duplicates, standardized column names, removed aggregate rows (like "Total" and "All India").

 Data Preprocessing:
Converted numeric columns and handled missing values.
Replaced negative values with 0.
One-hot encoded categorical variable state_ut.
Scaled numeric columns using MinMaxScaler.

 EDA & Visualization:
Top 10 states with the highest reported rape cases (bar plot).
Age-wise distribution of victims (bar plot).
Child vs adult victim distribution (pie chart).

 Feature Engineering:
child_to_adult_ratio – identifies states with high child victimization.
severity_index – victims per reported case, prioritizing critical regions.
% of child victims below 12 – highlights child vulnerability.

4. Steps to Run the Project
a. Upload the dataset NCRB_Table_3A.3.csv to your environment (Google Colab recommended).
b. Install required packages: !pip install pandas numpy matplotlib seaborn scikit-learn
c. Run the notebook cell by cell:
Data Cleaning → Data Preprocessing → EDA & Visualizations → Feature Engineering.
d. Explore the visualizations to understand trends in reported cases.
e. Review actionable insights based on the engineered features.

5. Challenges Faced & Creative Additions
Challenges:
Handling messy data with commas, missing values, and aggregate rows like “Total India”.
Converting columns to numeric while avoiding errors from non-numeric entries.

Creative Additions:
Introduced a severity index to help prioritize regions for intervention.
Calculated child-to-adult ratio and % of child victims below 12 to highlight vulnerable age groups.
Created informative visualizations for decision-makers to quickly understand trends.
