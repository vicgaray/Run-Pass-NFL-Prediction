# Run-Pass-NFL-Prediction
2025 Superbowl hosted the Philidelphia Eagles vs. Kansas City Chiefs. The Chiefs' strategy to stop the onslought of Saquon Barkley was to run a lot of one high safety and load the box. However, they did not anticipate the Eagles' efficient passing game, which cost them the game. A teams ability to anticipate whether an opponenet is going to pass or run has huge advatages in defensive planning, offensive strategy, and in-game decision-making.

### Goal
Predict whether an NFL play is a run or pass using in-game, play-by-play contextual features.

**Keywords:** binary classification, logistic regression, naive bayes, KNN

## Data Cleaning
Most of the missing values were irrelevant features. The only feature that had missing values was 'down' feature. Further inspection, we found that the missing values were due to extra point attempts. We decided to replace those NAs with 0s.

## Feature Engineering
The idea behind the features I selected is that we are building a model based on easily observable contexts, simulating real-time data. We avoid epa, completion percentage, pass play call rate, etc because I assume these metrics aren't available during real-time games. 
- 'prev_yards_gained' = the previous play's yards gained
- 'prev_run_pass' = the previous play's decision to run or pass
- 'success' = we defined success for a play based on the DVOA definition
- 'prev_success' = indicator on whether the previous play was considered successful
- 'is_redzone' = indicator on whether the offensive team is within 20 yards of the opponent's endzone

## Further Improvements
- Keeping a rolling average or some count of the previous play success (epa, pass yards, etc)


