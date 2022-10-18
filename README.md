# Tech-Stock-Analysis

## Project Overview
The objective of this project is to collect and analyze the top tech stocks and see if there is any correlations to be made to forecast stock growth for the future. 

## Resources
- Pandas
- yfinance
- yahoo_fin
- sklearn
- Tensorflow

## ETL
Started with data initially from Kaggle to identify the tech companies I wanted to analyze. The data was divide among 6 differently files, below shows inner merging the files to get a completed dataset to start with.

![ETL](/screenshots/inner-join.png)

## API 
My initial dataset does not carry historical data so I needed to pull more data. I tested both the yahoo_fin and yfinance libraries to pull the necessary data. After testing I confirmed that yfinance was able to get the historical data I wanted. For testing I decided on pulling 1 week of records for each company.

![API](/screenshots/api-test-data.png)

# Machine Learning

## Test 1 - Linear Regression Test
I tested a linear regression model to see if there were any correlation between a stocks volume and stocks price. This proved to yield no correlation of volume vs price over the course of a week. 

![linear-regression](/screenshots/linear-regression.png)

## Test 2 - Testing single stock using NN
After testing linear regression, I decided to shrink the dataset for further testing. I settled on using Microsoft stock and expanded the length from 1 week to 3 months worth of data to ensure there was enough data to work with.

![microsoft-dataset](/screenshots/microsoft-dataset.png)