# Amazon_Vine_Analysis

## Overview
Amazon Vine is a service that allows manufacturers and publishers to receive reviews for the products. Companies pay a small fee to Amazon and provide Amazon Vine members with products. In return, they receive a guaranteed review from the customer. The purpose of this analysis is to see if there is any bias towards good reviews from Vine members in the dataset. I analyzed a dataset of watch reviews for this purpose. I used PySpark to perform the ETL process, connected to an AWS RDS instance and loaded the transformed data into pgAdmin.

## Results
### Vine Reviews
 - There was a total of 47 vine reviews in the dataset.
 - 15 of these were 5 star reviews.
 - 32% of the total vine reviews were 5 stars.
 <img src = "https://github.com/Kee2u/Amazon_Vine_Analysis/blob/master/pictures/Paid_df.PNG?raw=true">

### Non-Vine Reviews
 - There was a total of 412169 normal reviews in the dataset.
 - 247221 of these were 5 star reviews.
 - 60% of the total non-vine reviews were 5 stars.
 <img src = "https://github.com/Kee2u/Amazon_Vine_Analysis/blob/master/pictures/Unpaid_df.PNG?raw=true">
 
## Summary
On comparing the percentages of 5 star ratings for both vine and non-vine reviews, it seems that there is no bias towards favourable reviews from vine members.
We must be careful to make this conclusion since there are only 47 reviews from vine members compared to 412169 reviews from non-vine members. There could be a sampling error at play here. We might see different results if the sample size of the vine member reviews was increased.

We could repeat the analysis by omitting the helpful votes filter. We are trying to see if there is a bias towards positive reviews from vine members and it would be helpful if we increase our dataset. 
