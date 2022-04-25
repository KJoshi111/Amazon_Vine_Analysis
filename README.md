# Amazon_Vine_Analysis

## Project overview:

* Delivarable 1:
Using our knowledge of the cloud ETL process, we created an AWS RDS database with tables in pgAdmin, picked a dataset from the Amazon Review datasets (Links to an external site.), and extracted the dataset into a DataFrame. We transformed the DataFrame into four separate DataFrames that match the table schema in pgAdmin. Then, uploaded the transformed data into the appropriate tables and ran queries in pgAdmin to confirm that the data has been uploaded.

* Deliverable 2:
With our knowledge of PySpark, Pandas, or SQL, determined if there is any bias towards reviews that were written as part of the Vine program. For this analysis, we determined if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Resources used:

### Data Source:
* Amazon Vine Reviews for outdoors items
### Softwares:
* Google Colab
* PgAdmin
* AWS
### Languages:
* PySpark

## Results:
Here are the screenshots of our Postgres SQL tables:

![customersDF](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/customersDF.png)

![productDF](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/productDF.png)

![reviewID](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/reviewID.png)

![vineDF](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/vineDF.png)

In this analysis we analyzed reviews that have more than 20 total votes and the percentage of helpful votes is equal or greater than 50.
### Determine the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews for the two types of review (paid vs unpaid).
They are as below:

![totalvinereview](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/nonvinereview.png)

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![5starvine](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/5starvine.png)

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
![percentage](https://github.com/KJoshi111/Amazon_Vine_Analysis/blob/main/images/percentage.png)

## Summary:
The purpose of this analysis is to analyze and determine if there is any bias towards favorable reviews from Vine members in the dataset. We analyzed reviews that have more than 20 total votes and the percentage of helpful votes is equal to greater than 50.This selection was made in order to pick reviews that are more likely to be helpful.
Positivity bias for review in the Vine program.
Here we analyzed 5-Star reviews within conditions mentioned above. Calculations show that there is no positivity bias for reviews in the Vine program. 

Additional Analysis and Suggestions:
We could expand this analysis bycalculating percentages for all stars reviews. Based on the results- there is a larger difference in percentages for 1 start reviews than for 5 star reviews.
