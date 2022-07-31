# Amazon_Vine_Analysis
 PySpark, Google Colab, PgAdmin, AWS RDS and S3

# Project overview
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We picked one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Also, we used PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

## Resources
("https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Home_Entertainment_v1_00.tsv.gz")

# Results

- The customers_table DataFrame

- The products_table DataFrame

- The review_id_table DataFrame

- The vine_table DataFrame

## DataFrames into pgAdmin

- customers_table
- products_table
- review_id_table
- vine_table

# Summary: Determine Bias of Vine Reviews.