# NFLdefensivelevers
The Impact of Defensive Sacks and Turnovers on Win Probability

This project analyzes how defensive sacks, turnovers, and home-field advantage affect an NFL team’s likelihood of winning a game using game-level data from 2020–2024.

**Problem and Stakeholder**
NFL defensive coordinators and analytics staff need clear evidence on which defensive actions most meaningfully influence win probability. With playoff positioning and job security often determined by narrow margins, understanding the relative value of generating pressure, forcing turnovers, and playing at home is critical for defensive strategy decisions.

**Dataset Overview**
Row Definition: One row represents a single team in a single NFL regular-season game
Time Span: 2020–2024 NFL regular seasons
Source Data: Play-by-play and team statistics from NFL Savant. Game outcomes from the NFLVerse GitHub repository
Scope: No major filters applied; all regular-season games included

**Method and Approach**
The analysis progressed from data cleaning and feature engineering in CP4, exploratory analysis in CP5, and model development and evaluation in CP6–CP7. A logistic regression model was used to predict whether a team won a game based on defensive sacks, defensive turnovers, and home/away status. This approach was selected for its interpretability and suitability for binary outcomes.

**Key Results**
Turnovers: Each defensive takeaway increases win probability by approximately 9 percentage points. Takeaways have the strongest impact on winning games.
Sacks: Each sack increases win probability by approximately 7 percentage points. Consistent pressure meaningfully shifts game outcomes.
Home-Field Advantage: Playing at home increases win probability by approximately 5 percentage points. Home field matters, but less than defensive production.

**How to View or Reproduce**
Cleaned Data: The cleaned CP4 dataset can be found in the /data folder under clean data.
Analysis Files: 
Requirements:

**Repository Map**
/data/ – Original source datasets and Clean analysis-ready datasets (CP4 output)
/figures/ – Charts and tables used in the final report
/reports/ – Project write-up and supporting documentation

**Limitations and Next Steps**
Limitations
  Offensive performance variables are not included, which may overstate defensive effects
  All turnovers are treated equally, despite interceptions and forced fumbles likely having different impacts
Next Steps
  Separate turnover types to compare their individual effects
  Run season-by-season models to evaluate result stability over time
