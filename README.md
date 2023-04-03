# Amazon Vine Analysis
## Overview of the analysis
I have been asked to work on a project in which I analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy, the finctional company asking me to make this analysis, pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

My assignment was to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

After creating the separate data frames for Vine members and non-Vine members, I used these processes to calculate the results:
![Paid Account Calculations](https://github.com/machudpicchu/Amazon_Vine_Analysis/blob/main/Paid_Account_Calculations.png)
![Unpaid Account Calculations](https://github.com/machudpicchu/Amazon_Vine_Analysis/blob/main/Unpaid_Account_Calculations.png)

## Results
After reviewing the data collected in the category of musical instruments, I determined answers to the following.
### How many Vine reviews and non-Vine reviews were there?
There are a total of 60 paid Vine reviews and 14,477 unpaid, non-Vine reviews.
### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
Of the reviews posted, there were 34 5-star reviews among the paid Vine reviews and 8,212 unpaid, non-Vine reviews.
### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
When comparing the percentage of 5-star reviews between paid and unpaid reviews in the musical instruments category, 56.667% of the paid Vine reviews were 5 stars, and 56.724% of the unpaid, non-Vine reviews were 5 stars.
## Summary
Given that there was only a difference of .057% between paid and unpaid 5-star reviews, it is safe to say that in the field of musical instruments, there is no discernable positivity bias between the two different account types.

### Recommendation
When thinking about the possibilities of positivity bias between paid and unpaid users, there was no discernable difference between the two in the category of musical instruments.  To further investigate the question, I would would want to compare the account reviews across 1, 2, 3, and 4-star reviews to see how they compare across the full spectrum of reviews.  Is there more of a positivity bias for 4-star reviews?  How do they compare for 1-star reviews?
