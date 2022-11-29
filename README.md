# Wine Rating Project 2
Data Science Bootcamp Project 2

**Author**: Susan Shin

### Goal:
The goal of this project was to predict wine ratings based on multiple attributes.


### Data:
The data inclues attributes such as Winery, Wine, Year, Number of Reviews, Region, Price, Type, Body and Acidity


## Methods
- Data was preprocessed using column transfer and simple imputer pipelines.
  - Missing objects were filled using the most frequent occurance.
  - Missing numbers were filled using mean.
  
- Three models were used for this project.
  - Bagging Regressor: Grid search was performed to understand optimal N_estimators.
  - KNeighborrs: Grid search was performed to understand optimal N_neighbors.
  - Random Forest: Grid search was performed to understand optiomal depth and 
- After being tuned, metrics (RMSE and r^2) were compared to decide which model would be the recommended model.
- Once choosing the best model, feature engineering (PCA and combining columns) were performed to see if results and time could improve.

## Results
- The Bagging Regressor model had the best r^2 and RMSE scores.
  - 51% R^2 score and a RMSE of 0.098
- Once this model was chosen, PCA was applied to try and decrease the time required to run. This unfortunately produced the opposite results that we would want.
- With combining columns, we were able to improve R^2 score to 52% with an RMSE of 0.098 (98% accuracy)

## Price vs. Rating Visualization
![](https://github.com/susansunshin/FoodPredictionProject/blob/main/photos/sku%20count%202.png)
> This graph shows the correlation between Price and Rating.
> This is useful to understand how price highly affects rating. It's important to understand that ratings can be highly biased to someone's taste and that although it's been said that the price of wine is arbitrary, it's still something that consumers take into consideration when rating a wine.

## Rating by Type Visualization
![](https://github.com/susansunshin/FoodPredictionProject/blob/main/photos/sum%20of%20sales.png)

> This graph shows the average rating by wine type.
> When looking at the data this way we can see that the average rating ranges from 4.3-4.5, which is a relatively small range. 
> Given that one would think that the type of wine would be the highest correlation between if someone likes a wine, this graph actually shows that it's not something that swings a rating as much as price.
> Furthermore, the correlation head map shows only a 24% correlation between rating and type.
> Both graphs show that ratings are highly biased to someone's tastes or preconceptions of what one thinks is a "good" wine.

## Limitations & Next Steps
- Limitations to this data would be around the circumstances of the testing. I would want to understand how the wine was administered. Ie. did people get to choose which wine they wanted to try or did everyone get the same sampling?
- The next steps would be to understand testing circumstances.

### For further information

For any additional questions, please contact **susansunshin@gmail.com**
