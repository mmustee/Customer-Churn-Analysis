# Customer-Churn-Analysis
### This is a detailed report dissecting why customers churn in Databel - a fictional telecommunications company using Power Query, Power BI and DAX. This dataset was obtained from Datacamp.

## Importance of Analysing Churn Rate
The following are reasons why analysing churn rate is very important for any company:

1. High Churn Rate can reflect poor competiveness
2. Churn rate tracks customer retention
3. Reducing churn is a key business goal as it can influence profit maximisation
   
## Project Outline
1. Prepare the Data
2. Explore the Data
3. Analyse & Visualise
4. Dashboarding


## Prepare the Data

Before analysing the data, it has to be cleaned and structed in order to make sure we derive accurate results.  The dataset was obtained from Datacamp and uploaded on Power Query. There was an option to load the data directly into Power BI but I chose to transform the data first. The following are things I did to prepare the data:

- Remove Duplicates
There should be at most one customer per row. Multiple rows of the same customer would negatively affect the analysis
- Remove Errors
Wrong Inputs were either rectified or deleted
- Remove redundant columns
It is a large dataset with several columns. some of these columns were removed because they have no use in this project and it improves the performance of the report
- Make sure all columns have the correct data types

### Transforming dataset ![](images/PowerQuery.png)

### Now that the data has been prepared, it was time to save the changes made and explore the data!

Despite completing the preparation process, I still wanted to make sure the number of customers were unique. There should only be one distinct customer per row. To do this, I created a measure to calculate the distinct number of customers to compare with another measure that counts the number of customers. i.e Number of Unique Customers = DISTINCTCOUNT('Databel - Data'[Customer ID]). Fortunately, both measures were exactly the same so I was good to go!





