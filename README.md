# Amazon_Vine_Analysis

## Analysis Overview
The aim of this project was to analyze the Amazon Vine program and to deduce if there Vine members are more likely to have favorable reviews. 
Throughout this project we utilized PySpark to extract, transform data, as well as, connect to the AWS RDS isntance to load our data to pgAdmin.
For this project we utilized a data containing reviews on video games provided by Amazon.

## Resources
- Data: [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), [Video Games Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz)
- Programs Used: Google Colab Notebook, PostgreSQL 11.9, AWS RDS

## Results
- Referring to our PySparks queries uploaded above we produced the following results. 
### Vine vs Non Vine Reviews
- Based on our query we concluded that there were 94 Vine reviews (as shown under total paid reviews) and 40471 Non-Vine reviews (as shown under unpaid reviews). 
### Amount of 5 Star Reviews: Vine vs Non-Vine
- Our results showed that 48/94 Vine reviews were 5 star reviews where as 15663/40471 Non-Vine Reviews were 5 star reviews. 
### 5 Star Review Percentages: Vine vs Non-Vine
- Our query showed that of the Vine reviews (or paid reviews), 51% of the reviews were 5 starred vs only 38% of the Non-Vine reviews were 5 starred. 

## Summary
Based on our results, we can conclude that there is a slight tendency of paid reviews to have a 5 star review vs reviewers who were not vine users. However seeing that the difference was only about a 13% difference, we would conclude that this bias is very slight and might be just be statistically insignficant. To be sure that our data is truly biased, we should run regressional analysis (ANOVA, Hypothesis test, etc.) to determine the what factors are signficant and if this difference in percentages are affected truly by paid vs unpaid reviewers. There is still a chance that this is all random and affected by factors that are not related to Vine vs Non-Vine Reviews. 
