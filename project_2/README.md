
# Project 2 
### Housing price prediction for Ames, Iowa

## Problem Statement 
I am part of a data team in a real estate company and we have been tasked to build a model that allows real estate agents to predict an accruate pricing for their clients. The model will also add extra values by providing features that would lead to highers sales price. We aim to develop a regression model that can accruately predict home prices in Ames, lowa.

## Background
As home ownership is on the rise post financial crsis, there is a gradual increase in homeownership.([*source*](https://www.statista.com/statistics/184902/homeownership-rate-in-the-us-since-2003/)) 

However with the rise in property price, it would be benificial for buyers and sellers to identify what are the key features people are looking out for. ([*source*](https://www.reuters.com/business/us-house-prices-rise-another-10-this-year-2022-03-02/#:~:text=Prices%20are%20forecast%20to%20rise,on%20the%20Case%2FShiller%20index.))

Having a realiable and accruate prediction on the houses will help buyers and seller to gauge and whether if the features/remodification of certain aspect would lead to higher returns on its investment. 

### DataSet selected:
- train.csv
- test.csv

This dataset provides the relevent data of specific features that may or may not have an impact on residential property sales price.

## Data Dictionary 

|Method|R2 Score|RMSE Score|
|---|---|---| 
|Lasso Regression - Train|0.8097|34077| 
|Lasso Regression - Test||0.8555|30687
|Ridge Regression - Train|0.8103|34020|
|Ridge Regression - Test|0.8561|30629|
|Linear Regression - Train|0.8113|33932|
|Linear Regression - Test|0.8558|30662|

## Findings:
- There is a strong positive correlation between Overall Quality and the property sales price. For property with higher quality ranking, they can usually fetch a higher sale price than property with lower ranking. 
- There is a negative correlation between the lifespan of the property. As the longer the property owner holds the property, the lower the sales price. This indicates that for speculative buyers of residential properties, they should sell whenever they can fetch a decent profit instead of holding and hoping for higher price in the future. 
- Most of the properties that are able to fetch a higher price are built after the year 2000. The price range is between 120k to 600k. Generally for properties before 1960s, they can usually can only fetch below 300k 
- Many buyers are also willing to pay a higher price for properties with larger ground living space. This is also applicable for properties with large basement areas as well. 
- Home buyers are also more inclined to pay more for personal garage areas that comes together with the property. 


## Conclusion

Features such as overall condition of the property, ground living area, external quality, kitchen quality and Masonry veneer area are highly correlated to the sales price. This indicates that generally buyers/sellers who focus on these aspect have a higher chance in selling the property at a higher price. While the 3 regression model were able to predict price at a high accruacy, there is a requirement to obtain more data and constantly update the features as more and more young adults are becoming homebuyers which may have a different view of features in relation to features. On top of that, although the accruacy is above benchmark of 80%, collection of more data may help in providing more insight leading to better results. Homesellers who aims to sell the house can also be remainded that the long the property is held without remodifications, the lower the future salesprice they might receive. 

## Recommendation 

- Sellers of the property is to look into the key features that could result in selling the properties at a higher price. 
- While for speculative buyers, they can look into features that leads to a lower sales price and focus on remodifying the key features  in hope for a good chance to flip the property at a profit. 
- I would also recommend for the data collection to make the answers for survey/data entry mandatory to avoid having a large amount of empty values which might lead to low correlation/skewed result. 
- I would also include interest rates data/government intervention(eg: ABSD for Singapore) to see if there is a strong correlation between higher mortgage rates with lower property price. The rational for such idea is to see if higher mortgage rate would reduce the demand of properties which may lead to a drop in prices. 




## Authors

- [@zacharykwek15](https://github.com/zacharykwek15/GA-projects)

