# Project 02 Proposal: <your project title>

**Team members:** Matthew Baxman

See the [Project 02 instructions](https://data385.github.io/project/proj02_wholegame.html) for what goes in each section. Bullet points are great. Put any images in an `img/` folder.

## 1. Problem statement

NBA teams, coaches, and analysts want to understand which aspects of team performance are most closely associated with winning basketball 
games. Identifying these factors can help teams make better decisions about offensive strategies, defensive strategies, and overall team 
performance.

This project will analyze NBA team statistics across multiple seasons to investigate which statistical factors are associated with winning. 
I expect teams with stronger shooting percentages, more assists, and more rebounds to have better winning records, while teams with more 
turnovers may have worse records.

## 2. Research question

Is an NBA team's game outcome (win or loss) associated with its field goal percentage, three-point percentage, rebounds, assists, 
turnovers, and home-court advantage?

## 3. Data acquisition

I plan to collect NBA team game statistics from the NBA's official statistics resources. I will use historical regular-season game data 
across multiple seasons to create a dataset with more than 200 team-game observations.

### a. Confirm viability

The primary data source will be NBA.com Stats:

https://www.nba.com/stats/teams/traditional

The NBA statistics website provides team statistics and performance information. I will scrape and investigate the available historical game data. I plan to use regular-season data from multiple NBA seasons to ensure that the dataset meets the minimum requirement of 200 observations.

### b. Variables of interest

TEAM: Categorical. The NBA team participating in the game.
SEASON: Categorical. The NBA season in which the game occurred.
GAME_DATE: Date. The date the game was played.
GAME_OUTCOME: Categorical. Whether the team won or lost the game.
POINTS: Quantitative. Total points scored by the team.
FG_PCT: Quantitative. Team field goal shooting percentage.
FG3_PCT: Quantitative. Team three-point shooting percentage.
REB: Quantitative. Total rebounds recorded by the team.
AST: Quantitative. Total assists recorded by the team.
TOV: Quantitative. Total turnovers committed by the team.
HOME_AWAY: Categorical. Whether the team played at home or away.

## 4. Data example

https://www.nba.com/stats/teams/traditional



## 5. EDA

I plan to use the following techniques:

read_csv() to import the data into R.
glimpse() and summary() to examine the dataset and understand the variables.
is.na() to identify missing values.
distinct() to check for duplicate observations.
filter() to select regular-season games.
mutate() to create or modify variables when necessary.
group_by() and summarise() to calculate team performance summaries.
ggplot() to create histograms, scatterplots, and bar charts.
Boxplots to compare statistics between winning and losing teams.
Correlation analysis to examine relationships between numerical variables.

These techniques will help identify patterns in team performance and determine which statistics may be associated with winning.

## 6. Modeling

I plan to use logistic regression because the response variable has two possible outcomes: win or loss.

Response variable: GAME_OUTCOME (win or loss).
Predictor variables: FG_PCT, FG3_PCT, REB, AST, TOV, and HOME_AWAY.
The model will estimate how team statistics and home-court advantage are associated with the probability of winning a game. I will evaluate 
the model using a confusion matrix, accuracy, and other appropriate classification measures.

## 7. Communicate

I plan to communicate my results through a short slide presentation. The presentation will include data visualizations, descriptive statistics, logistic regression results, and recommendations about which team performance factors are most strongly associated with winning NBA games.

## 8. LLM disclaimer

I plan to use ChatGPT to help brainstorm research questions, understand R functions, troubleshoot coding errors, and organize my project. I 
will review and verify AI-generated suggestions and code before using them. I will not upload private or sensitive information to AI tools.

