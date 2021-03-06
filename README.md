# BT5153_Group10_yelp
Review Quality Based Recommendation for Yelp

## Data
The representative subset of the original data can be found in Data folder.

## Code
There are total 8 ipynb notebooks. The notebook sequence is denoted in titles.

1. Data Preparation

We first converted the json files downloaded from Yelp to csv file. Then joins Review, Business and User table together. By joining 3 tables, there are a total of 43 variables and 8,021,122 records. 
We then filtered data by selecting open restaurants (is_open = 1 & Category contains "restaurant") in Nevada.
The output filtered file is named as "filted_nv.csv"

2. EDA

Preliminary data exploration is conducted.

- Word Cloud For Reviews
- Star rating distribution of both reviews and businesses
- Lat-Long Plotting For Nevada
- Review Deep Dive

3. Useful Review Classification_nontext

Compare all model classification result for nontext features:

- Read/Split Data
- Data Preprocessing (nontext)
- Modeling
- Evaluation

4. Useful Review Classification_withtext

Compare all model classification result for nontext features:

- Read/Split Data
- Data Preprocessing (nontext & text)
- Modeling
- Evaluation

5. Content-Based Filtering

6. recommendation_collaborative_filtering

- GMM

7. recommendation_collaborative_filtering_km&hr

- K-means
- Hierachical Clustering

8. Recommendation_Pipeline

Combining Content-based filtering and collaborative filtering. Finally output recommendation result and conducted evaluation in terms of diversity, personalization, number_in_actual, satisfaction, coverage
