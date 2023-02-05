# Amazon_Vine_Analysis
Module 17

### Overview of the analysis:
US outdoors review from of Amazon review datasets was picked and perform the ETL to extract the dataset, transform the data, connect to ny AWS RDS instance, and load the transformed data into pgAdmin. Next, I furthere perform analysis using Jupyternotebook to determine if there is any bias toward favorable reviews from Vine members in selected dataset.

### Results: 

![image](https://github.com/jilldvn/Amazon_Vine_Analysis/blob/main/image/Rview_Five_Star_Vine.png)

#### 1. How many Vine reviews and non-Vine reviews were there?
- paid_reviews_count (vine): 3137,
- unpaid_reviews_count (non-vine): 2299255

#### 2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- paid_five_star_count (vine): 1686, 
- unpaid_five_star_count (non-vine): 1433198

#### 3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- paid_five_star (vine): 0.12%, 
- unpaid_five_star (non-vine): 99.88%

### Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
