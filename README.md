# University of Maryland Baseball Team Performance Analysis

## Data source
[University of Maryland Baseball Website](https://umterps.com/sports/baseball)

## Overview
This project employs **Microsoft SQL Server** and **Tableau** to analyze critical factors affecting the University of Maryland baseball team's win rate. The analysis focuses on player distribution (height and weight) and the influence of temperature conditions on performance.

- **Microsoft SQL Server**: Used for database management, integrating multiple data sources, data cleansing, and querying.
- **Tableau**: Used to create intuitive visualizations and interactive dashboards, providing insights to optimize the team’s win rate.

**Insights generated from the analysis can guide the coaching staff in optimizing player selection based on physical attributes and environmental factors, ultimately improving the team's performance.**

## Project goal
The primary goal of this project is to **optimize decision-making** by analyzing key performance indicators, such as player distribution and temperature trends, that contribute to game outcomes. The analysis specifically targets:
- Player distribution based on height and weight.
- Identifying performance trends influenced by temperature.

## Tools Used
- **Database Management**: Microsoft SQL Server
- **Visualization**: Tableau

## ER Diagram for Database Structure
<img width="535" alt="ER diagram" src="https://github.com/user-attachments/assets/b7e546ae-4851-4552-861d-044f24ea8da1">


## Relational schema
The project’s relational schema defines the following entities and their relationships:
- **Player**: (playerId, playerFirstName, playerLastName, playerHeight, playerWeight)
- **Weather**: (weatherDate, weatherTemperature, gameId)
- **Schedule**: (gameId, gameOpponent, gameStadium, gameDate)
- **Position**: (positionId, playerPosition)
- **Result**: (gameDate, winnerTeam, loserTeam, result)
- **Play**: (playerId, gameId)
- **Assign**: (playerId, positionId)

## Visualizaiton on Tableau
Below are the insights derived from the visualizations built in Tableau.

### 1. Player Distribution Based on Height and Weight

- **Objective**: Analyze how the coaching staff distributes players by height and weight.
- **Key Insight**: The chart highlights the average height and weight for each position—pitching, fielding, and batting.

<img width="533" alt="heights1" src="https://github.com/user-attachments/assets/cc2caa89-2aac-4344-8001-61b2345650fd">


### 2.1 Height's Impact on Winning
   
- **Objective**: Determine the role of player height in winning games.
- **Key Insight**: Taller players are predominantly chosen as pitchers, particularly in winning games. Height has less impact on batting and fielding success, suggesting its critical importance for pitching.

<img width="531" alt="heights2" src="https://github.com/user-attachments/assets/c4f2cb3a-030a-427e-ab89-9f4f79d2ab08">


### 2.2 Weight's Impact on Winning
- **Objective**: Analyze the impact of player weight on game outcomes.
- **Key Insight**: Heavier pitchers tend to win more games compared to batters and fielders. Weight plays a significant role in pitching success, while batting and fielding positions show less variation in weight between winning and losing.

<img width="531" alt="heights2" src="https://github.com/user-attachments/assets/8f1422c9-8fe6-45bd-a1f9-ec4857c3309b">


### 3. Temperature’s Impact on Performance
- **Objective**: Examine the correlation between temperature and team performance.
- **Key Insight**: Warmer temperatures, particularly during June, correlate with increased win rates, while colder weather in March leads to a dip in performance.

<img width="363" alt="temperature" src="https://github.com/user-attachments/assets/b0d12b84-421d-424a-acdd-8ac13936dd97">


### 4. Win Rate Trends Across Seasons
- **Objective**: Identify win rate trends in different temperature conditions over several seasons.
- **Key Insight**: Colder temperatures tend to result in lower win rates across seasons, while warmer conditions correlate with better outcomes.

<img width="505" alt="winning rates" src="https://github.com/user-attachments/assets/4164e2d2-8ce0-4498-b9e1-3704a1be11b2">


# Conclusion
By identifying critical factors such as height, weight, and temperature, this analysis provides actionable insights to guide the team's strategy. Adjustments in player selection and game scheduling could significantly enhance the team’s win rate, with warmer weather appearing to be a key factor for better performance.
