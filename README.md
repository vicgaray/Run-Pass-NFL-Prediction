# Run-Pass-NFL-Prediction
2025 Superbowl hosted the Philidelphia Eagles vs. Kansas City Chiefs. The Chiefs' strategy to stop the onslought of Saquon Barkley was to run a lot of one high safety and load the box. However, they did not anticipate the Eagles' efficient passing game, which cost them the game. A teams ability to anticipate whether an opponenet is going to pass or run has huge advatages in defensive planning, offensive strategy, and in-game decision-making.

### Goal
Predict whether an NFL play is a run or pass using in-game, play-by-play contextual features.

**Keywords:** binary classification, logistic regression, naive bayes, KNN

## Further Improvements
- Keeping a rolling average or some count of the previous play success (epa, pass yards, etc)

## Data Cleaning
Most of the missing values features were features that are irrelavent. The only feature that had missing values was 'down' feature. Further inspection, we found that the missing values were due to extra point attempts. We decided to replace those NAs with 0s.
