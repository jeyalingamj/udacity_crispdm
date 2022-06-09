# udacity_crispdm
### Table of Contents

1. [Libraries](#libraries)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing & Authors](#licensing)

## Libraries <a name="libraries"></a>
* Python 3.9
* Pandas
* Seaborn
* Sklearn
* Folium

## Project Motivation <a name="motivation"></a>
This assignment is part of the Udacity "Become a Data Scientist" nanodegree.
In this project the author focuses on the following:
* Analyse Airbnb listing data for the Seattle are in the USA 
* Propose questions of interest based on the data provided. Specifically the questions asked are:
  * *What are the most expensive months of the year to vist Seattle?*
  * *Where are the expensive listings in Seattle?*
  * *How accurately can we predict a listing's price?*
  * *What contributes to the price of a listing and how does it impact the price?*
* Using standard industry data analys practices (CRISP-DM) answer these questions

A blog post relating to this analysis can be found [here]()
## File Descriptions <a name="files"></a>
* Raw data of Airbnb listings (orginally sourced [here](https://www.kaggle.com/datasets/airbnb/seattle/version/1/metadata))
 * listings.csv
 * reviews.csv
 * calendar.csv
* airbnb_analysis.ipynb, contains:
 * Analysis of data
 * Listing price modelling
 * Visualisations
## Results <a name="results"></a>
The analysis provided answers the questions posed above. 
Based on this we can see that the most expensive period to visit Seattle is summer (specifically July). Prices peak again, relative to neighbouring months, in December. This is likely due to christmas holidays and new year.

The most expensive listings by far are found in Belltown with an average price of $824. However, it should be noted that not a lot of data exists for this price range compared to other much cheaper neighbourhoods.

A Random Forets Regression model was used to predict listing prices in the Seattle region and is able to achieve an r2_score of upt to 94% on a test set. Based on this model we can see that the largest contributor to price, according to the model used, is the number of bedrooms. Second are the number of bathrooms available. Additional fees make the listings more expensive, such as cleaning fees or secutiry deposits (who would've thought).

## Licensing & Authors <a name="licensing"></a>
Data: All data used is provided by Airbnb, Inc.
Author: J Jeyalingam
