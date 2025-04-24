# P7 Custom BI Project: NBA Player Impact Analysis

## Overview
I’m Bin Ware, and this document outlines my P7 Custom BI Project for the course, building on my D7.1 discussion. My project analyzes NBA player performance to identify those with the greatest impact on game outcomes, using metrics like points scored, Player Efficiency Rating (PER), and plus-minus, segmented by quarter and opponent team. Due to time constraints and a strong course grade, I’m focusing on planning, documentation, and ethical considerations rather than implementing code or visualizations, aiming to secure partial credit. This project aligns with my passion for basketball analytics and applies business intelligence (BI) concepts such as data warehousing, OLAP, and visualization to support NBA coaching decisions.

## 1. Business Goal
The business goal is to identify which NBA players have the most significant impact on game outcomes based on performance metrics (points scored, PER, and plus-minus) by quarter and opponent team. This is critical for NBA teams, particularly during the playoff season, as it informs strategic decisions like player rotations and matchup planning. By pinpointing high-impact players in specific scenarios, teams can optimize performance and gain a competitive edge.

## 2. Data Sources
The analysis would rely on the following hypothetical data sources:
- **NBA Game Logs**: Player performance data including points scored, PER, and plus-minus by game, quarter, and opponent, sourced from platforms like [Basketball-Reference](https://www.basketball-reference.com/) or [NBA.com Stats](https://www.nba.com/stats/).
- **Team Schedules**: Game dates and opponent teams to provide temporal context.
- **Player Profiles**: Player names, positions, and team affiliations for segmentation.
- **Hypothetical Dataset**: A file named `nba_player_stats.csv` with columns: `player_id`, `player_name`, `game_date`, `quarter`, `opponent_team`, `points_scored`, `per`, `plus_minus`, `shot_type`.

## 3. Tools Planned
Based on my experience from prior coursework (e.g., Smart Store Project, April 18, 2025), I would use:
- **Python (Pandas, Seaborn)**: For data processing and visualization. Pandas is ideal for aggregations, and Seaborn produces clear, analytical plots.
- **Power BI**: For creating interactive dashboards with slicers and drilldowns, suitable for presenting insights to stakeholders like coaches.
- **SQL**: For querying a data warehouse to extract and aggregate player statistics efficiently.

## 4. Workflow and Logic
The planned workflow includes the following steps:
1. **Data Preparation**: Load `nba_player_stats.csv` into Pandas or Power BI. Clean the data by addressing missing PER values (e.g., via imputation), standardizing opponent team names, and ensuring `game_date` is in datetime format.
2. **Aggregation**: Group data by `player_name`, `quarter`, and `opponent_team` to compute:
   - Sum of `points_scored` and `plus_minus`.
   - Average `per` per game or season.
   - Percentage of team points contributed (`points_scored / team_total_points * 100`).
3. **Analysis**: Perform the following:
   - **Slicing**: Isolate data by player to compare individual contributions.
   - **Dicing**: Break down data by quarter and opponent to examine performance in specific scenarios.
   - **Drilldown**: Explore high-impact games to analyze shot types and scoring efficiency.
4. **Visualization**: Develop:
   - Line charts to track PER trends over the season.
   - Bar charts to compare points scored by quarter.
   - Heatmaps to visualize plus-minus by quarter and opponent.
5. **Insights**: Derive actionable recommendations for coaching strategies based on performance patterns.

## 5. Expected Results
Since I did not implement the code due to time constraints, the following are anticipated outcomes:
- **Narrative**: Star players are expected to exhibit higher PER in the fourth quarter against weaker opponents, indicating clutch performance. Bench players may show unexpectedly high plus-minus in specific quarters, suggesting undervalued contributions. PER likely peaks mid-season but declines in back-to-back games due to fatigue.
- **Planned Visualizations**:
   - **Line Chart**: PER over the season to highlight performance trends for key players.
   - **Bar Chart**: Points scored by quarter to identify clutch contributors.
   - **Heatmap**: Plus-minus by quarter and opponent to reveal matchup strengths.
- **Note**: Visualizations were not created due to time limitations but are outlined to demonstrate the analytical approach.

## 6. Suggested Business Actions
Based on the expected insights, NBA teams could take the following actions:
- Prioritize clutch performers in fourth-quarter lineups to maximize game-closing impact.
- Adjust defensive strategies for opponents where players underperform to mitigate weaknesses.
- Schedule rest for key players during back-to-back games to maintain performance levels and prevent PER declines.

## 7. Challenges
The primary challenges include:
- **Time Constraints**: Limited availability prevented coding, visualization development, or data collection.
- **Data Access**: Obtaining granular per-quarter statistics requires advanced scraping or API access, as noted in my D7.1 submission.
- **Data Normalization**: Variations in team playing pace complicate cross-player comparisons, requiring adjustments for fair analysis.

## 8. Ethical Considerations
To ensure ethical BI practices, I considered the following:
- **Data Privacy**: Use only publicly available statistics from reputable sources (e.g., NBA.com, Basketball-Reference) to avoid ethical concerns.
- **Bias Mitigation**: Validate the dataset to include bench players and smaller-market teams, preventing insights skewed toward high-profile players.
- **Responsible Use**: Avoid over-reliance on PER, which may undervalue defensive contributions, to ensure fair player evaluations and prevent biased coaching decisions.
- **AI Transparency**: If predictive models were used (e.g., to forecast player impact), ensure coaches understand the methodology to avoid opaque, automated decision-making.

## Resources
As required by D7.1, I recommend the following resources for basketball analytics:
1. [Basketball-Reference](https://www.basketball-reference.com/) – Comprehensive source for NBA player and game statistics.
2. [NBA.com Stats](https://www.nba.com/stats/) – Official platform for game logs and advanced metrics like PER and plus-minus.
