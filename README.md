# play_store_eda
EDA on Play Store Data

## Summary

In this project we will perform Exploratory Data Analysis on Play Store Data. Play Store dataset contains information like reviews, ratings, size, category, etc. on around a 10,000 apps. In this project we will do some data cleaning, wrangling to clean and ready the data for exploratory analysis. Then, we will chart various variable to find any relationships between them, and identify top performing categories.

## Dataset information
1. The dataset contains following columns:
App, Category, Rating, Reviews, Size, Installs, Type, Price, Content Rating, Genres, Last Updated, Current Ver, Android Ver

2. Dataset shape: (10841, 13)

3. Libraries used: pandas, numpy, matplotlib, seaborn, missingno

## Data Wrangling

1. De-duplication:
The dataset contains duplicate rows. We first remove the duplicate rows. Then, we identify duplicate app names, which are listed in more than one categories. We keep the most reviewed app in each category.

2. Missing values:
We visualize missing values with the missingno library. There are missing values in the dataset. We don't choose to impute the values right now. We will drop them or fill them with zeros when we do the plotting.

3. Custom performance metric:
We add a column for a custom performance metric, which measures performance by calculating ***(rating * reviews / installs)***

## Charting:

We plot various graphs to find relationships between variables and identify top performing categories.

## Conclusion:

The EDA performed above reveals top categories by various metrics among which the top categories by our custom performance metric are:

Game
Social
Medical
Weather
Family
The focus should be on developing apps in these top categories for maximum reach and number of installs. Also, in order to get high number of installs, developers should focus on getting more number of positive reviews with positive rating. The price of the app should be kept as low as possible, and preferrably the app should be free.
