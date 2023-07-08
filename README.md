# DataScience_Excel_dashboards
I crafted Excel dashboards using data science methodologies for precise data analysis and cleansing, ensuring accurate and reliable insights.

This README file details the process we followed to analyze and visualize bike sales data using an interactive Excel dashboard. Our analysis journey encompasses data cleaning, feature engineering, and the creation of pivot tables for interactive visual analytics. We aim to derive valuable insights from the data and facilitate data-driven decision-making by employing these steps.

The dataset used for this analysis is sourced from the 'Alex the Analyst' repository on GitHub. It consists of 13 columns and 1001 rows, representing information on 1000 customers and their demographic and sales data. The columns in the dataset include:

ID
Marital Status (Single/Married)
Gender (Female/Male)
Income
Children
Education (Bachelors, Masters, College)
Occupation (Skilled manual, Professional, Clerical, Manual, Management)
Home Owner (Yes/No)
Cars
Commute Distance (0-1, 2-5, 5-10, More than 10 miles)
Region (Europe, North America, Pacific)
Age
Bike Purchase (Yes/No)
These columns capture various aspects of the customers' profiles, such as their demographics, income, education, occupation, and purchase behavior. The dataset provides a rich source of information to explore and analyze bike sales patterns and customer characteristics.

Before we could analyze the data, we had to ensure it was clean and free of inaccuracies. Here are the key Excel techniques we employed:

Find & Replace (Ctrl+H): Used to replace category codes with their full meaning (e.g., 'M' with 'Married' and 'S' with 'Single' in the Marital Status column).
Remove Duplicates: Excel's built-in function was used to ensure all customers' data is unique.
Currency Formatting: We specified the currency for the 'Income' column to provide clarity on income values.

As part of our analysis, we utilized Excel's IF function to create a new column called 'Age Brackets.' This column categorizes customers into three groups: 'Adolescent,' 'Middle Age,' and 'Old.' Feature engineering plays a crucial role in data analysis as it enhances data understanding and can improve model performance if predictive analysis is conducted later.

The formula used to create the 'Age Brackets' column is as follows:
=IF(L2>54, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))

By applying this formula, we classified customers based on their age into respective brackets. This new feature allows for a more detailed analysis of bike sales across different age groups, providing valuable insights into customer preferences and behavior within specific age ranges.

To facilitate the analysis and visualization of the bike sales data, three additional sheets were created:

Workspace: This sheet is a duplicate of the original dataset, serving as a working space for performing operations without modifying the original data. It provides a clean and safe environment to conduct various analyses and transformations.

Pivot Tables & Visuals: This sheet contains multiple pivot tables that summarize and analyze the dataset. Pivot tables offer a powerful way to aggregate and analyze data, providing insights into various aspects of bike sales. Corresponding visuals, such as charts and graphs, were created alongside each pivot table to visually represent the summarized data.

Dashboard: In this sheet, we consolidated key insights into an interactive dashboard. The dashboard utilizes Excel's built-in filter feature, allowing users to filter the data based on specific criteria such as Marital Status, Region, and Education. This interactive functionality enables users to dynamically explore the data and gain valuable insights by narrowing down the analysis to specific segments or categories.

By creating these additional sheets, we streamline the analysis process and provide a comprehensive view of the data through pivot tables, visuals, and an interactive dashboard, making it easier to derive meaningful insights and communicate the findings effectively.

Data exploration and cleaning are indeed essential steps in any data analysis process. These steps are crucial for ensuring the quality and accuracy of the data, which in turn leads to reliable and meaningful insights. By conducting thorough data exploration and cleaning, we were able to:

Avoid skewed results: Data cleaning helps identify and handle any outliers, missing values, or inconsistencies in the dataset. By addressing these issues, we prevent skewed results and ensure that our analysis is based on accurate and representative data.

Identify important trends: Through data exploration, we gain a deeper understanding of the dataset, allowing us to identify key patterns and trends. By cleaning the data, we can remove any noise or irrelevant information that may hinder the identification of important trends. This enables us to focus on the most significant insights and make informed business decisions.

Build a robust, interactive dashboard: Data cleaning provides a solid foundation for building an interactive dashboard. By ensuring the accuracy and reliability of the data, we can confidently create visualizations and interactive elements that effectively communicate insights to stakeholders. A robust dashboard enables users to explore the data, uncover hidden insights, and make data-driven decisions with confidence.

In summary, data exploration and cleaning are vital steps that contribute to the overall success of the data analysis process. By ensuring data quality and accuracy, we can generate reliable insights and build powerful visualizations and dashboards that drive informed business decisions.

With the clean dataset, the addition of enriched features, and the comprehensive dashboard, we are equipped to analyze and gain a deeper understanding of the sales performance of bikes across various demographics and geographical locations. This wealth of information empowers strategic business decisions by providing valuable insights into customer preferences, regional trends, and demographic influences. The analysis enables businesses to identify target markets, optimize marketing strategies, and make data-driven decisions that align with their goals and objectives. The combination of a clean dataset, enriched insights, and a comprehensive dashboard significantly enhances the ability to extract valuable information and unlock opportunities for growth and success.
