*Project Overview

This project focuses on cleaning and preparing the Bank Marketing Dataset for analysis.
The dataset contains information on customer demographics, financial details, and campaign-related metrics. 
Proper data cleaning ensures the data is accurate, consistent, and ready for meaningful analysis and visualization.


Dataset Information:

The dataset contains the following columns:

* age: Age of the customer.
* Age group: Categorized age groups (e.g., Young, Middle Age, Old Age).
* job: Job role of the customer.
* marital status: Marital status of the customer.
* education: Type of education (e.g., basic, high school, university degree).
* education level: Level of education.
* default: Whether the customer has credit in default (yes or no).
* housing loan: Whether the customer has a housing loan.
* personal loan: Whether the customer has a personal loan.
* contact: Type of contact used for the campaign (cellular or telephone).
* month: Last contact month of the year.
* day of week: Day of the week when the last contact occurred.
* Duration (seconds): Duration of the last contact in seconds.
* campaign: Number of contacts performed during this campaign.
*previous days: Number of days since the client was last contacted.
*previous: Number of contacts performed before this campaign.
*previous outcome: Outcome of the previous campaign.
*emp.var.rate: Employment variation rate (economic indicator).

Data Cleaning Steps:
1. Handling Missing Values
Checked each column for missing or null values.
Replaced missing values with appropriate measures:
Numerical Columns: Used median or mean values.
Categorical Columns: Imputed using the mode or labeled as Unknown.

3. Standardizing Categorical Data:
Standardized text-based columns like job, marital status, education, and default to ensure consistency (e.g., lowercasing and removing extra spaces).
Mapped categorical values to more descriptive labels where necessary.

5. Creating Age Groups:
Binned the age column into distinct age groups:
Young Age (18-30)
Middle Age (31-60)
Old Age (60+).

7. Removing Duplicates:
Identified and removed duplicate rows to ensure unique records.

9. Outlier Treatment:
Reviewed numerical columns (Duration (seconds), emp.var.rate, etc.) for outliers using statistical methods (e.g., IQR).
Capped extreme outliers to a reasonable range or removed them if irrelevant.

11. Converting Data Types:
Ensured that numerical data was in the correct format (e.g., int or float).
Converted columns like Outcome (y/n) to binary values (e.g., 1 for yes, 0 for no).

13. Renaming Columns:
Renamed columns for better clarity and readability:
housing loan → Housing Loan.
personal loan → Personal Loan.
Duration (seconds) → Contact Duration.

Pivot Table Highlights

1. Percentage of Term Deposit Subscriptions:
Displays the count of customers who subscribed (yes) versus those who did not (no) to the term deposit product.

3. Correlation Between Age and Outcomes:
Age groups are categorized into Middle Age, Old Age, and Young Age, showing how age impacts subscription outcomes.

5. Outcome by Job Roles:
Highlights subscription trends across various job categories (e.g., Admin, Blue-collar, Entrepreneur).

7. Outcome Based on Month:
Shows monthly trends in customer subscriptions, with a detailed comparison of successful (yes) and unsuccessful (no) outcomes.

9. Proportion of Calls Made Each Month:
Displays the total number of calls made in each month to gauge campaign intensity and performance.

11. Distribution of Customers and Loans:
Explores the relationship between customer demographics (age groups) and their loan types (housing and personal loans).

13. Outcomes Based on Marital Status:
Analyzes how marital status (Married, Single, Divorced, Unknown) correlates with campaign subscription results.

15. Mode of Contact for Customer Outcomes:
Examines the effectiveness of contact methods (Cellular, Telephone) used during the campaign.
Visualizations
The following charts were created based on the pivot table data for better insights:
1)Pie Chart: Displays the percentage of yes and no outcomes for term deposit subscriptions.
2)Bar Charts: Highlight key trends like:
3)Age-wise and job-role-wise outcomes.
4)Monthly subscriptions and call proportions.
5)Combination Charts: Present a summary of customer loans distribution and outcomes.


*Dashboard Overview
The dashboard provides a comprehensive visualization of the bank marketing campaign's performance. It focuses on customer behavior, campaign outcomes, and key demographic insights to support strategic decision-making. Below are the key sections:

Term Deposit Outcomes

* A pie chart showing the percentage of customers who subscribed (yes) versus those who did not (no) to term deposits.
Age-wise Outcomes

* A bar chart displaying the subscription distribution across age groups (Middle-aged, Old-aged, Young-aged).
Outcome by Job Role

* A bar chart comparing term deposit outcomes across different job roles (e.g., Admin, Blue-collar, Entrepreneur, Housemaid).
Month-wise Outcome

* A bar chart illustrating subscription outcomes across different months.
Month-wise Calls

* A pie chart representing the proportion of marketing calls made during each month.
Outcomes vs Marital Status

* A bar chart showing the campaign's effectiveness for different marital statuses (Married, Single, Divorced, Unknown).
Customers and Loans

* A bar chart analyzing the relationship between customer loans (housing and personal loans) and their subscription outcomes across age groups.
Contact Methods

* A bar chart highlighting the effectiveness of customer contact methods (cellular, telephone) for the campaign.

** Key Insights

1) Middle-aged customers dominate the term deposit subscriptions.
2) The months of April and May showed high campaign activity.
3) Cellular communication proved to be the most effective contact method.
4) Married individuals were the most responsive to the campaign.
