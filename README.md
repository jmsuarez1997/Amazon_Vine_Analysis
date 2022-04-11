# Amazon_Vine_Analysis

## Overview

This analysis takes a closer look at the reviews written by the Amazon Vine program members. The Vine program is a service to manufacturers and publishers that allows their products to receive product reviews. The manufacturer will pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 

The first part of this project uses PySpark to perform the ETL process to extract an AWS cloud-based dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. The second part of this project uses PySpark to determine if there is any bias toward favorable reviews from Vine members in our dataset.
## Results

Attached [here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) is a link to the S3 data used for the analysis. There are a few categories of reviews, and for this project, the "amazon_reviews_us_Camera_v1_00.tsv.gz" was used. There were a total of 607 Vine reviews and 50,522 non-Vine reviews.  

![Vine](https://raw.githubusercontent.com/jmsuarez1997/Amazon_Vine_Analysis/main/Resources/Vine.png "Vine")

![NonVine](https://raw.githubusercontent.com/jmsuarez1997/Amazon_Vine_Analysis/main/Resources/NonVine.png "NonVine")

There were 257 five-star Vine reviews and 25,220 five-star non-Vine reviews. 42.33 percent of total Vine reviews were five-stars, and 49.92 percent of total Non-Vine reviews were five-stars. 

## Summary

The results of the Vine program analysis indicate no evidence for positivity bias from Vine members in the camera category. 42.33% of Vine members left a five-star, and 49.92% of non-Vine members left a five-star review. Non-Vine members for the camera category leave more 5 star reviews, and Vine members are potentially more critical when reviewing products. An additional analysis I would add is repeating the same analysis across another amazon product category to see if the trend in our study stayed consistent with the results from the first analysis. 