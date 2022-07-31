# Amazon_Vine_Analysis
 PySpark, Google Colab, PgAdmin, AWS RDS and S3

# Project overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We picked one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Also, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

## Resources
"https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Home_Entertainment_v1_00.tsv.gz"

# Results

- The customers_table DataFrame

![image](https://user-images.githubusercontent.com/92646311/182047272-a19e99ee-d122-4a17-8829-649393e2b9c2.png)

- The products_table DataFrame

![image](https://user-images.githubusercontent.com/92646311/182047353-38760a90-b8a6-4f25-8ae5-5cf6ffa3cc64.png)

- The review_id_table DataFrame

![image](https://user-images.githubusercontent.com/92646311/182047314-5cb1a9cf-9b26-4b00-a0c5-977498ff6387.png)

- The vine_table DataFrame

![image](https://user-images.githubusercontent.com/92646311/182047323-2b6948b0-3937-4ddf-9fed-178ee055241c.png)


## DataFrames into pgAdmin

- customers_table

![image](https://user-images.githubusercontent.com/92646311/182047414-768769d6-3a7d-40b3-99f2-1c749ea86bce.png)

- products_table

![image](https://user-images.githubusercontent.com/92646311/182047427-e688a892-fc65-436b-99d7-bd6a1b87cbee.png)

- review_id_table

![image](https://user-images.githubusercontent.com/92646311/182047438-1025d08a-63a9-427e-99f8-6d438df0e57b.png)

- vine_table

![image](https://user-images.githubusercontent.com/92646311/182047448-6200437e-ba77-4be5-a871-d0789507a4b8.png)

# vine_table analysis

-  Vine reviews   261   and  non-Vine reviews  24040

![image](https://user-images.githubusercontent.com/92646311/182047854-d31d1af9-2e9b-4c51-afd0-1b8de29ce438.png)
![image](https://user-images.githubusercontent.com/92646311/182047872-a08b3389-e045-4496-83a1-77e802f51c8d.png)

-  There were total 11005 five star reviews.  Vine reviews were five stars 106 and non-Vine reviews were five stars 10899
  
![image](https://user-images.githubusercontent.com/92646311/182047931-c3806b50-01e0-47bc-97e9-fda5edd243fd.png)


- Percentage of Vine reviews there were five stars is 40.61% and for non-Vine reviews five stars is 45.34%.

- ![image](https://user-images.githubusercontent.com/92646311/182048054-a06580f1-443a-4f42-8dc9-ff2ed868fd43.png)


# Summary: Determine Bias of Vine Reviews.

The output of both percentages does not have enough margin to decide whether they contain any bias or not in the Vine program. 
The vine sample size still has a decent number while it is important to note that the non-vine sample has not much difference. The output of both percentages does not have enough margin to decide whether they contain any bias or not in the Vine program. We can perform further analysis on verified purchases to determine the percentage and compare them to see if we can decide if this reveals any positivity bias.

