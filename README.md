# Maven Market Analysis

![](Image_1.webp)

## Introduction
Using Power BI, I performed a high-level examination of a **Maven Market** dataset and employed various techniques such as DAX measures and data modeling to gain insights. Additionally, I delivered valuable business insights and visualizations to present the findings.  Specifically, I utilized DAX measures like calculated columns, related functions, iterator functions (such as SUMX), and time intelligence formulas to explore the dataset. Furthermore, I implemented data modeling techniques like snowflake schemas, one-to-many relationship cardinality, and one-way filter flows. 

The analysis was framed by a set of questions that aimed to solve business problems, such as identifying revenue trends between 1997 and 1998, improving the presence of countries with low business presence, pinpointing the most profitable brand and suggesting which brands should be discontinued, analyzing the impact of costs on gross profit and recommending measures to control them. The ultimate goal of this analysis was to provide insights that can be acted upon to enhance business performance and promote growth.

## Data Sourcing
For this project, I utilized a dataset from an Udemy course project called **Maven Market** and used Power BI to shape and connect the data. A total of 7 tables were used:
- CALENDER: 730 rows, 7 columns
- CUSTOMERS: 10,281 rows, 19 columns
- PRODUCTS: 1,560 rows, 10 columns
- REGION: 109 rows, 3 columns
- RETURNS: 7,087 rows, 4 columns
- STORES: 24 rows, 13 columns
- TRANSACTIONS: 269,720 rows, 6 columns

## Data Transformation and Cleaning
To guarantee the precision and uniformity of the data, I leveraged Power Query Editor in Power BI to perform data transformation and cleansing tasks. The following are some of the measures I took:
- Named all tables and confirmed that headers were appropriately promoted.
- Checked and corrected all data types.
- ncorporated calculated columns into tables where appropriate.
- Implemented Time Intelligence Formulas, such as Performance To-Date and Previous Period formulas, to facilitate common time comparisons.
- Deployed different DAX measures, including Related, Calculate, and Iterate function (Sumx).

## Data Modelling
To establish meaningful connections between the tables in the dataset, I conducted a thorough analysis of the primary and foreign keys in each table. Although Power BI generated some relationships automatically, I detected some missing relationships. To address this, I established a relationship between the primary key "DATE" in the "Calendar" table and the corresponding key "DATE" in the "Transactions" table.

Throughout this process, I verified the relationship between the "Region" table and the "Transactions" table. However, I noticed that there was no primary key to link the "Region" and "Transactions" tables. To remedy this issue, I employed a "Snowflake Schema" to link the "Region" and "Stores" tables. Additionally, I ensured that all relationships followed a "One to Many Cardinality" and that all filters were "One-Way," which meant that there were no "Two-Way Filters."

![](Data_modelling_snapshot.JPG)



