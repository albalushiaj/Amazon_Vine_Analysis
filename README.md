# ****Amazon_Vine_Analysis****
## Overview of Project
- The purpose of this project is to analyze customer review dataset from Amazon revolving around member of the paid Amazon program which is a service that allows manufacturers and publishers to receive reviews for their products. Using PySpark, AWS RDS, PGAdmin, and Pandas, the ETL process is performed then determined if there is any bias towards favorable reviews from Amazon Vine members in the dataset. 

## Results
- To determine if there is any Bias review, Pandas (Jupyter Notebook) is used to filter, and create new dataframes that can help enlighten the scenario.
- Filter one is used to only show rows where the number of total votes that is greater or equal to 20. By doing so, this helps select reviews that are more likely to be helpful by avoiding error. 

![image](https://user-images.githubusercontent.com/106709942/192177990-43ce67fd-9ecb-4f59-be69-118399f49b6b.png)

- Filter two is used to retreive all rows where the number of helpful votes/the total votes is greater than 50 percent.

![image](https://user-images.githubusercontent.com/106709942/192178240-ccb52dae-7ffa-42ad-9ae1-f4a299c868fb.png)

- Filter three, and four are coducted to separate filter two between reviews written as _part of the Vine Program (Paid)_, and reviews not _part of the Vine Program (Unpaid)_. After filter three, and four, the following results are determined:
  - The number of 5 star reviews
  - The percentage of 5 star reviews (Paid/Unpaid)
  - The total number of reviews/
 - The final results are the following:
   - There is 49 Vine Reviews
   - 48 of Vine Reviews gave 5 stars.
   - ~51.06% of Vine Reviews were 5 stars.
   - There is 40,471 non Vine Reviews
   - 15,663 non Vine Reviews gave 5 stars.
   - ~38.7% of non Vine Reviews were 5 stars. 
   
## Summary
- Based on the results, there is seen to be a postive bias among Video Game reviews in the Amazon Vine Program. There was ~38% of regular reviews that  gave 5 stars while ~51% of vine reviews gave 5 Stars.
- The dataset is large variety of products containg 40,565 data points where only under one percent are Vine Reviews (~0.23%). Thus, the small amount of reviews is not impactful to the overall rating of products listed on Amazon. 
- Recommendation:
- Additional analysis on the 5 star scale would be insightful to seeing what other star reviews are given to products, and if provides any additional postivity bias. 

