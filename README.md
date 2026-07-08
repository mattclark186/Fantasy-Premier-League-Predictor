# ⚽ Fantasy-Premier-League-Predictor

[Python Code](https://github.com/mattclark186/Fantasy-Premier-League-Predictor/blob/main/FPL%20Predictor.ipynb)

## 📌 Overview
- Data preparation
- Feature engineering
- Machine learning
- Visualisation
- All done in Python

Developed four XGBoost regression models (one per position) to predict a player's points in the next Fantasy Premier League gameweek based on historical player & team performance data.

## 🏆 Outcome
The models achieved consistent performance across positions, with average prediction **errors of 1.1 to 1.4 points** per gameweek. Relatively low MAE values with higher RMSE values indicate that the predictions are fairly accurate on average but with occasional large errors.

| Position | R² | MAE | RMSE |
|----------|----|-----|------|
| GK       | 0.324 | 1.145 | 1.985 |
| DEF      | 0.348 | 1.399 | 2.172 |
| MID      | 0.366 | 1.212 | 2.016 |
| FWD      | 0.321 | 1.346 | 2.277 |


## 📝 Details

### Tools Used
Python, Pandas, NumPy, Matplotlib, SKLearn, XGBoost

### Key Steps
 1. **Data Preparation** Aligning formatting and merging data into a single dataframe, renaming columns, renaming positions, removing outliers, sorting data.
 2. **Feature Engineering** Creating multiple new features, including mathematically combining existing features and creating rolling lags.
 3. **Modelling** Tuning hyperparameters of XGBoost models using GridSearchCV.
 4. **Visualisation** Creating visualisations that show the performance of the models.

## 📊 Visualisations
### Predicted vs Actual
Predicted gameweek points vs the actual gameweek points, with the dashed black lines representing perfect predictions. The predictions follow the general trend of the points scored well. However, the models are far better at predicting lower scores, as the coloured points are generally closer to the dashed line towards the lower end. This means the best-scoring gameweeks will often be underestimated.

<img width="800" height="800" alt="image" src="https://github.com/user-attachments/assets/aa7ae4be-8077-4e30-8a5e-b64dc342080d" />

### MAE vs RMSE
This illustrates the broad consistency across positions. It also shows the RMSE is notably higher than the MAE for each position, again showing that the best-scoring gameweeks will be underestimated.

<img width="600" height="450" alt="image" src="https://github.com/user-attachments/assets/2b863269-5429-41a6-be3d-7296926127fa" />

## ⚽ What is Fantasy Premier League?

Fantasy Premier League (referred to commonly as FPL) is a game where players select real footballers to be in their fantasy team, who will score in-game points based on their real-life performance in matches. Footballers are assigned a value and players must remain within their budget when choosing their team. Points are earned by actions such as scoring goals, getting assists or getting clean sheets (i.e. not conceding any goals), amongst many others. Points can also be lost by negative actions, such as receiving a red card. Players can make a limited number of changes to their team throughout the 10-month season, meaning it would be very valuable to be able to predict whether a player will score high or low in their upcoming game. The key to success is to have a team filled with footballers who score high, particularly relative to their assigned value.

## 🔎 Data Sources

[FPL Data](https://www.fpl-data.co.uk/statistics)

[Premier League](https://www.premierleague.com)
