Customer Segmentation Project

This project aims to perform unsupervised clustering of customer records from a groceries firm's database. The goal is to divide customers into segments that reflect similarities among them, enabling the optimization of product modifications and better catering to the diverse needs and behaviors of different customer types.

Data Cleaning & Feature Engineering

To prepare the dataset for analysis, the following steps will be taken:

Handling missing values: The income column contains missing values, which will be addressed during the data cleaning process.
Parsing date: The "Dt_Customer" column, indicating the date a customer joined the database, will be converted to a DateTime format.
Encoding categorical features: The data frame includes categorical features represented as objects. These features will be encoded into numeric forms for further analysis.
Creating a new feature: A new feature will be generated based on the "Dt_Customer" column to indicate the number of days a customer has been registered in the firm's database. This value will be relative to the most recent customer in the record to maintain simplicity.
Extracting age: The "Age" of a customer will be extracted by calculating the difference between the current year and the "Year_Birth" column, which indicates the birth year of the respective person.
Creating "Total_Spending": A new feature called "Total_Spending" will be created to indicate the total amount spent by the customer in various categories over the span of two years.
Creating "Household_Size": The "Marital_Status," "Kidhome," and "Teenhome" columns will be used to create a new feature called "Household_Size" that captures the living situation of individuals.
Simplifying "Education": The "Education" column will be categorized into three simplified categories to facilitate analysis.
Dropping redundant features: Certain features that are no longer necessary for the analysis will be dropped from the dataset.
Adding "Has_Used_Campaign": A boolean category variable called "Has_Used_Campaign" will be included to indicate whether a customer has participated in any campaigns.

Clustering Analysis

After the data cleaning and feature engineering steps, clustering analysis will be performed to group customers based on their similarities. The resulting clusters will provide insights into customer segmentation, enabling the business to optimize its strategies and cater to the distinct needs and behaviors of different customer types.

Please refer to the project code and documentation for detailed implementation and analysis.

Dependencies

The following dependencies are required to run the project:

Python (version 3.10.9)
Pandas (version 2.0.1)
Scikit-learn (version 1.0.2)
NumPy (version 1.24.3)
Matplotlib (version 3.7.0)
Seaborn (version 0.12.2)
Yellowbrick (version 1.5)
Please make sure to install the necessary dependencies before running the project.

Usage

To replicate the project, follow these steps:

Clone the repository.
Install the required dependencies listed in the "Dependencies" section.
Run the project code, ensuring that the dataset file is located in the correct directory.
Analyze the clustering results and interpret the customer segments.
For more detailed instructions and usage examples, please refer to the project documentation.
