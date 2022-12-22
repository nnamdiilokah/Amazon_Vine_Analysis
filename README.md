# Amazon_Vine_Analysis
**Analysis on Amazon's Vine Program using Amazon Web Services, PySpark and Postgres SQL**

## Overview of Project

The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we’ll  pick one of the Amazon review dataset and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards, we’ll use PySpark to determine if there is any bias towards favorable reviews from Vine members in the dataset.

This will be achieved in two deliverables:

+ **Perform ETL on Amazon Product Reviews:** 
In this deliverable, we’ll create an AWS RDS database with tables in pgAdmin, and extract the dataset into a DataFrame. We’ll then transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin and then upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

+ **Determine Bias of Vine Reviews:** 
Using PySpark we’ll determine if there is any bias towards reviews that were written as part of the Vine program. For this analysis we’ll determine the total number of reviews, the number of 5-star reviews, and the percentage of 5-star reviews. This will enable us find out if having a paid Vine review makes a difference in the percentage of 5-star reviews.


## Results

**How many Vine reviews and Non-Vine reviews were there?**
+ Vine Reviews: 22
+ Non-Vine Reviews: 27,710

**How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
+ 5-Star Vine Reviews: 13
+ 5-Star Non-Vine Reviews: 14,569

**What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
+ 5-Star Vine Reviews: 59.09&
+ 5-Star Non-Vine Reviews: 52.57%


## Summary

