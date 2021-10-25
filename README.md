# Amazon_Vine_Analysis

## Overview
For this project I analyzed Amazon reviews written by members of the paid Amazon Vine program. This program is a serviece that allows maufacturers and publishers to receive reviews for thier products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. From approximately 50 datasets I chose the __Sports__ apparel dataset. Then, using PySpark, I performed the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and finally load the transformed data into pgAdmin. Lastly, I used PySpark to determine if there was any bias toward facorable reviewes from Vine members in the dataset.

## Resources
* __Pyspark__
* __Apache Spark__
* __Google Colab__
* __Amazon Web Services (AWS)__
* __PostgreSQL and pgAdmin4__

## Results 
### Analysis of Vine Reviews:
![paidReviews](https://user-images.githubusercontent.com/85372441/138743243-2f4e072c-cd3f-4b3e-a33a-998fd232181a.png)
![paid5star](https://user-images.githubusercontent.com/85372441/138743783-cbdbee49-f68e-4637-a667-48989c376b3b.png)
![paid5perc](https://user-images.githubusercontent.com/85372441/138743831-4b47a7b5-baa3-438d-aa75-52763c6c3e4b.png)

### Analysis of non-Vine Reviews:
![unpaidReviews](https://user-images.githubusercontent.com/85372441/138743977-e6c773ce-96db-4ed7-9cd6-bdfa9d1e1fe5.png)
![unpaid5star](https://user-images.githubusercontent.com/85372441/138743981-cd562525-fd4d-42d1-9c24-edbd58ebf387.png)
![unpaid5perc](https://user-images.githubusercontent.com/85372441/138743980-8522d6e1-e833-441e-a607-aee76b2a79ce.png)

* The data above shows that members of the paid Amazon Vine program reviewed the sports dataset 334 times while giving a 5 star review 139 times (__~42%__ ).
* The data also shows that there were 61,614 non-Vine reviews who gave a 5 star review 32,665 times ( __~53%__ ).

## Summary
Based off the above data I have concluded that the paid Amazon Vine reviews do not have a bias towards favorable reviews since the non-Vine reviewers gave 5 star reviews ~53% of the time and the paid Vine reviewers gave a 5 star review ~42% of the time. 
