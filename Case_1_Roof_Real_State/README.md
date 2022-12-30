
# Case 1 - Roof Real State

Data analyses about real state in King County - Washington USA

The case was the fist chalenge of DEX - Data Expert Course from "Escola DNC"








## Authors

- [@henriqueborgo](https://github.com/henriqueborgo)


## Task

Evaluate and indicate the top 5 houses to invest and the top 5 to doesn't invest at County Kind - Washington, USA.
## References

 - [Dataset](https://www.kaggle.com/harlfoxem/housesalesprediction)
 - [Detailed Dataset](https://geodacenter.github.io/data-and-lab/KingCounty-HouseSales2015/)



 
 


## Summary of Tech Stack

This data analyses was built using Python. 
The work was elaborated in Google colabority IDE.

To run this project import:

- Pandas
- Seaborn
- Matoplolib.pyplot
## Project Description

The project was built through CRISP-DM methodology.

#### Business Understanding + Data Understanding
1. Renamed features to improve Understanding

#### Data Preparation
1. Evaluated the usefull data
2. Erased features: 'latitude' and 'longitude'
3. Adjusted the date to date sintax
4. Integrated data: list of cities of County King by zipcode
5. Constructed data: calculated the cost per area of each house
6. Constructed data: calculated the cost per area of the the entire property of each house

#### Modeling

1. Set that I don't want to pay more than price/size_living = 150$/ft² (based on GRAPH 2)
2. Set that better cost-benefit houses are newer than 1960 (based on GRAPH 4)
3. Set that cheaper houses have two or less floors
4. Set that I dont' want houses above 'condition' 4 
5. Set that I want houses with more than 2 bedroomns
6. Set 'view' better than 2
7. Verified correlation between atributes by seaborn heatmap
8. Verified the correlation between the city and the price/m² of the property
9. Verified the correlation between the city and the price of the property (houses below 150$/ft²)
10. Verified the correlation between the year built and the price/m² of the property
11. Verified the correlation between the number of floors and the price/m² of the property
12. Verified the correlation between the number of bedrooms and the price/m² of the property
13. Verified the correlation between the quality of view and the price/m² of the property
14. Verified if the top 5 cheaper houses (houses_adjust) have been sold more then one time
15. Verified the houses that were sold multiple times
  

    
    

    
    
## Conclusion

The top 5 houses to invest are:

* houses_adjust['id'] == 2113700360
* houses_adjust['id'] == 5152100060
* houses_adjust['id'] == 8159300050
* houses_adjust['id'] == 4167800130
* houses_adjust['id'] == 3121069038

The top 5 worst houses to invest are:

* houses_adjust['id'] == 3331001995
* houses_adjust['id'] == 6788200605
* houses_adjust['id'] == 1498302783
* houses_adjust['id'] == 2572400100
* houses_adjust['id'] == 3599600276