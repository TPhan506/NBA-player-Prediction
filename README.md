# NBA player points prediction

Machine learning project that predicts NBA players' single game points using historical performances

DATA:
Player game logs were downloaded using 'nba_api' and saved as CSV files in a local folder

-training: 2021-22 and 2022-23
-Validation: 2023-24
-Testing: 2024-25

APPROACH:
Features included
  -Recent and up to date scoring averages
  -Recent 2pt, 3pt, and free throw attempts
  -historical shooting percentages on the season
  -recent and season-to-date minutes
  -home court status
  -opponent points allowed over previous 10 games

RESULTS:
22,194 eligible player-games from the 2024-25 season

OVERALL MAE - Model 4.66 points | 5 Game average baseline 4.86 points
Highscorer MAE - Model 6.5 points | 5 Game average baseline 6.94 points

VISUALIZATION:
notebooks includes
  Model vs baseline MAE
  average avtual vs predicted scoring
  prediction error group by changes in playing time
  counts of predictios in absolute error ranges


LIMITATIONS
Unexpected changes in plahing time can produce large errors
Injuries, lineup changes, and teammate availabiity are not modeled
exceptional scoring performances are difficult to predict
direction accuracy is measured against historacl average


Run the project
1. Open the project notebook
2. Run the cells in order
Downloaded season csvs are reused

Future improvements
Incorporate information avaiable before games about player availability and expected roles
improve minute predictions
compare linear regression with other models
evaluate performance across additional seasons
