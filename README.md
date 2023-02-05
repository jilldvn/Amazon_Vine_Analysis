# Amazon_Vine_Analysis
Module 17

### Overview of the analysis:
US outdoors review from of Amazon review datasets was picked and perform the ETL to extract the dataset, transform the data, connect to ny AWS RDS instance, and load the transformed data into pgAdmin. Next, I furthere perform analysis using Jupyternotebook to determine the proportion of vine reviews per favorable and unfavorable reviews. Finally there is a descriptive analysis based on overall 5 star reviews whether paid or unpaid.  

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

### Summary: 
A bias could be onserved due to an five star calculation based on the overall vine and non vine reviews is from overall reviews without filtering the dataset if other customers feel the star rating is helpful or not. Therefore the total 5 star reviews count could be subjective. Besides, the star rating count per vine or non vine is not grouped by product parent. With all being said, it is suggeested for further analysis:
  1. Vine and non vine 5 star analysis should be done afer filtering the data with higher portion of helpful votes. 
  2. Join the tables of Review_ID_Table and Vine_Table (as shown below) using review_ID as primary key, then regroup the data based on product parent, in this case, a comparison of star rating count with vine or non-vine under the same category of product might be more meaningful. 

- review_id_table

![image](https://github.com/jilldvn/Amazon_Vine_Analysis/blob/main/image/review_id_table.png)

- vine_table

![image](https://github.com/jilldvn/Amazon_Vine_Analysis/blob/main/image/vine_table.png)
