# ⚽ Fantasy-Premier-League-Predictor

## 📌 Overview
 - A data science project that includes data preparation, feature engineering, machine learning modelling and results visualisation, all in Python. 

 - XGBoost models used predict the points a player will get in the upcoming FPL gameweek based on player and team performance data for the season so far.

## 🏆 Outcome
A model was trained for each position (GK, DEF, MID, FWD), with values of **R^2 0.32-0.37**, **MAE 1.1-1.4**, and **RMSE 1.9-2.3**.
| Position | R² | MAE | RMSE |
|----------|----|-----|------|
| GK       | 0.324 | 1.145 | 1.985 |
| DEF      | 0.348 | 1.399 | 2.172 |
| MID      | 0.366 | 1.212 | 2.016 |
| FWD      | 0.321 | 1.346 | 2.277 |

## 📝 Details

### What is Fantasy Premier League?

Fantasy Premier League (referred to commonly as FPL) is a game where players select real footballers to be in their fantasy team, who will score in-game points based on their real-life performance in matches. Footballers are assigned a value and players must remain within their budget when choosing their team. Points are earned by actions such as scoring goals, getting assists or getting clean sheets (i.e. not conceding any goals), amongst many others. Points can also be lost by negative actions, such as receiving a red card. Players can make a limited number of changes to their team throughout the 10-month season, meaning it would be very valuable to be able to predict whether a player will score high or low in their upcoming game. The key to success is to have a team filled with footballers who score high, particularly relative to their assigned value.
