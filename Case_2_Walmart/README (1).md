
# Case 2 - Walmart

Data analyses about USA Walmart Stores.


## Autores

- [@henriqueborgo](https://github.com/henriqueborgo)


## Task

To carry out an information survey about the revenue of the stores in USA and point wich store would be better to expand the size.
## Referência

 - [Dataset](https://www.kaggle.com/yasserh/walmart-dataset)

## Summary of Tech Stack

This data analyses was built using Python. The work was elaborated in Google colabority IDE.

To run this project import:

- Pandas
- Seaborn
- Matplotlib.pyplot
- Plotly.express
- Numpy
- Interact (from ipywidgets)
## Project Description

The project was built through CRISP-DM methodology.

#### Business sucess criteria

The projet will be a success if there is a store that worth it to invest on expansio


#### Business Understanding

Walmart, Inc., is an American multinational grocery store Department. The company was founded by Sam Walton in 1962, incorporated on October 1969 and listed on the New York Stock Exchange in 1972.

In the year 2021, it made a profit of $13.51 Billion. Being one of the main retail stores in the world, the data includes weekly sales from 45 stores across the United States. Walmart runs several discount promotional events throughout the year. year. These markdowns precede major holidays, the four major everyone, which is the Super Bowl, Labor Day, Thanksgiving and Christmas. Weeks that include these holidays carry greater weight.


#### Data Understanding

- Reading the dataset info, it's possible to see that there's no missing values.
- The date may be coverted to datetime
- Holiday flag may be converted in category
- The titles area easy to understand, not necessary to change
- CPI: An index that measures the monthly change in prices paid by U.S. consumers, based on a weight average of prices for a basket of goods and services representative of aggregated U.S. consumers spending. Source: [investopedia](https://www.investopedia.com/terms/c/consumerpriceindex.asp)


#### Data Preparation and Modeling

For this step were used the following technics:

- Filtering and sorting
Converted the 'Date' from object to datetime.
Converted the 'Holiday_Flag' and 'Store' from int64 to category.
Removed the scienctific notation of the 'Weekly_Sales column'. 
Modified the date to %Y-%M format.

- Detection of outliers
Dropped 10/Jan and 12/Nov/Dez data (low grouped sales in month - outlier).
Dropped Stores 3, 5, 30, 33, 36, 37, 38, 42, 43, 44 (low weekly sales - no high outliers).

- Data visualization
Created a dataframe with the top 10 stores.
Created a bar plot with historic store month sales (top 10 stores).
Created a bar plot with historic store month sales (without top 10 stores).
Construct data: created a dataframe without holidays.

#### Evaluation

- Stores 20, 4, 14, 13, 2, 10, 27, 6, 1 have the best mean store sales, in this specific order.
- The top store (20) overpass 11/33 (33%) times the store_mean_sale.
- The second store (4) overpass 11/33 (33%) times the store_mean_sale.
- The third store (14) overpass 13/33 (40%) times the store_mean_sale.
- Store 14 has the top mean sales (without hollidays sales).
- Stores 3, 5, 30, 33, 36, 37, 38, 42, 43, 44 are not superior outliers, that is, no historic of sales increase.
- Stores 40, 35, 8, 17, 45, 21, 25, 15, 7, 9, 29, 16 are bellow the walmart_mean_sale.




## Conclusion

- The top store to expand is the Store 14.
- It has margin to expand and more stability at non hollidays season