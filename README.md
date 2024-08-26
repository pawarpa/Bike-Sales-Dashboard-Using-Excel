# Bike Sales Dashboard Project

## Project Overview

The "Bike Sales Dashboard" project is designed to analyze and visualize bike sales data using Excel. The primary goal is to identify factors influencing bike purchases and to create customer profiles based on demographic and behavioral data. The final output is an interactive dashboard that allows users to explore the data and uncover insights about bike sales across different regions, occupations, age groups, and other factors.

## Dataset

The dataset contains information on 1,000 individuals and includes the following 13 columns:

- **ID**: Unique identifier for each buyer.
- **Marital Status**: Marital status of the buyer (e.g., Married, Single).
- **Gender**: Gender of the buyer (Male, Female).
- **Income**: Annual income of the buyer.
- **Children**: Number of children the buyer has.
- **Education**: Educational level of the buyer.
- **Occupation**: Occupation of the buyer.
- **Home Owner**: Indicates if the buyer owns a home.
- **Cars**: Number of cars owned by the buyer.
- **Commute Distance**: Distance the buyer commutes to work.
- **Region**: Geographic region where the buyer lives.
- **Age**: Age of the buyer.
- **Purchased Bike**: Indicates if the buyer purchased a bike (Yes/No).

## Objectives

1. **Identify Factors Influencing Bike Purchases**: Understand which factors (such as income, age, or occupation) are most strongly associated with bike purchases.
2. **Create Customer Profiles**: Develop profiles of typical bike buyers based on their demographic and behavioral characteristics.

## Data Cleaning and Preparation

The dataset was cleaned and prepared for analysis through the following steps:

1. **Remove Duplicates**: Identified and removed 26 duplicate entries to ensure data uniqueness.
2. **Re-format Income Column**: Standardized the income values for consistency.
3. **Clarify Abbreviations**: Expanded abbreviations in the "Marital Status" and "Gender" columns to improve clarity (e.g., 'M' to 'Married,' 'F' to 'Female').
4. **Create Age Brackets**: Added a new "Age Brackets" column using a Nested IF statement to categorize buyers into three age groups:
   ```excel
   =IF(L2>54, "Old", IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))
  - **Young Adults**: Under 31 years
  - **Middle-aged Adults**: 31-45 years
  - **Old-aged Adults**: Over 45 years
5. **Standardize Commute Distance**: Replaced "10+ Miles" with "More than 10 Miles" to allow for correct data sorting and analysis.

## Analysis and Visualization

- **Pivot Tables**: Created to summarize the data and identify patterns, such as bike purchases by gender, income, and age group.
- **Charts and Graphs**: Developed various visualizations to represent the data, including bar charts, pie charts, and line graphs.
- **Interactive Dashboard**: Built a dashboard in Excel featuring slicers, which allow users to filter and interact with the data dynamically.

## Key Insights

- **Income and Gender**: Males, with an average income of $60,124, purchased more bikes than females, who earned 7% less on average.
- **Age Group Analysis**: Middle-aged adults (31-45 years) purchased four times more bikes than younger or older adults.
- **Education Level**: Graduate degree holders were more likely to purchase bikes compared to high school graduates.

## Conclusion and Recommendations

- **Targeting Middle Agers**: Focus marketing efforts on middle-aged adults, who are the most active bike buyers.
- **Tailored Strategies**: Develop specific strategies to engage younger and older adults, adapting marketing tactics to their unique needs and preferences.

