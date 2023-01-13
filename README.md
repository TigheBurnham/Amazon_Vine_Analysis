# Amazon_Vine_Analysis

## Overview of the analysis: 

In this project we were tasked with analyzing "Amazon reviews written by members of the paid Amazon Vine program." Currently, the Amazon Vine program allows manufacturers and publishers to receive reviews for their products. In exchange for a small fee Amazon will provide products to Amazon Vine members, who are then tasked to publish a review.

After looking at the 50 Data sets to choose from, this project looks into reviews of US Digital Video Downloads. The tools used in this project were AWS, PySpark, and SQL. The three deliverables for this were to:

-Deliverable 1: Perform ETL on Amazon Product Reviews

-Deliverable 2: Determine Bias of Vine Reviews

-Deliverable 3: A Written Report on the Analysis (README.md)

## Results: 

Link to the Vine dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Video_Download_v1_00.tsv.gz

The data was cleaned, as well as rows with less than 20 votes and the rows where the number of helpful votes divided by total votes is equal to or greater than 50% we also filtered out. 

### How many Vine reviews and non-Vine reviews were there?

<img width="599" alt="vine_yes" src="https://user-images.githubusercontent.com/112028534/212218979-04453e9a-c535-4251-b86d-6a37354470cb.png">
There were no vine reviews for the US Digital Video Downloads.

<img width="588" alt="nvp_count" src="https://user-images.githubusercontent.com/112028534/212220617-01a406a2-fca4-4c6c-9cc7-16ad9a00e778.png">
There were 11,362 total non vine reviews.

### How many Vine reviews were 5 stars? 

Since there were no vine reviews there are no 5 star reviews that were part of the vine program.

### How many non-Vine reviews were 5 stars?

<img width="122" alt="total_5_star" src="https://user-images.githubusercontent.com/112028534/212221389-0382ca40-d617-4c3e-87ea-274aa8139168.png">

There were 4,670 total 5 star reviews that were non-Vine. 

### What percentage of Vine reviews were 5 stars? 

The percentage of Vine reviews that were 5 stars is 0%.

### What percentage of non-Vine reviews were 5 stars?

<img width="107" alt="5 star %" src="https://user-images.githubusercontent.com/112028534/212222620-7eda96f3-864b-44de-9d0b-f8174061d3d3.png">

The percentage of non-Vine reviews that were 5 stars is 41.1%.

## Summary: 

Based on the results there was no positivity bias for reviews in the Vine program. This is because there were no Vine program reviews in Amazon's US Digital Video Downloads dataset. 41.1% of the programs non-Vine reviews were 5 star. Additional analysis could be done within the non-Vine reviews regarding summary statistics and the distribution of the reviews. 
