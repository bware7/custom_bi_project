P7 Custom BI Project Outline – Bin Ware
Overview
I’m Bin Ware, and this outline details my P7 Custom BI Project plan. My project analyzes NBA player performance to identify those with the greatest impact on game outcomes, building on my D7.1 discussion. Due to time constraints and a strong course grade, I’m focusing on planning, documentation, and ethical considerations rather than coding, aiming for partial credit. The project leverages my interest in basketball analytics and applies BI concepts like data warehousing, OLAP, and visualization to support NBA coaching decisions.
1. Business Goal
The goal is to identify which NBA players have the most significant impact on game outcomes based on performance metrics (points scored, Player Efficiency Rating [PER], and plus-minus) by quarter and opponent team. This is critical for NBA teams, particularly during the playoff season, as it informs strategic decisions such as player rotations and matchup planning, ultimately enhancing team performance and competitive advantage.
2. Data Sources
The analysis would use the following hypothetical data sources:

NBA Game Logs: Player performance data (points, PER, plus-minus) by game, quarter, and opponent, sourced from platforms like Basketball-Reference or NBA.com.
Team Schedules: Game dates and opponent teams for temporal context.
Player Profiles: Player names, positions, and team affiliations for segmentation.
Hypothetical Dataset: A file named nba_player_stats.csv with columns: player_id, player_name, game_date, quarter, opponent_team, points_scored, per, plus_minus, shot_type.

3. Tools Planned
I would utilize the following tools, based on prior coursework (e.g., Smart Store Project, April 18, 2025):

Python (Pandas, Seaborn): For data processing and visualization, leveraging Pandas for aggregations and Seaborn for clear, analytical plots.
Power BI: For creating interactive dashboards with slicers and drilldowns, suitable for presenting to stakeholders like coaches.
SQL: For querying a data warehouse to extract and aggregate player statistics efficiently.

4. Workflow and Logic
The planned workflow includes:

Data Preparation: Load nba_player_stats.csv into Pandas or Power BI. Clean data by addressing missing PER values, standardizing opponent team names, and ensuring game_date is in datetime format.
Aggregation: Group data by player, quarter, and opponent team to compute:
Sum of points scored and plus-minus.
Average PER per game or season.
Percentage of team points contributed (points_scored / team_total_points * 100).


Analysis: Perform slicing by player, dicing by quarter and opponent, and drilling into specific games to examine shot types and high-impact performances.
Visualization: Develop line charts for PER trends, bar charts for points by quarter, and heatmaps for plus-minus by opponent.
Insights: Derive recommendations for coaching strategies based on player performance patterns.

5. Expected Results
Without coding, here are the anticipated outcomes:

Narrative: Key players likely exhibit higher PER in the fourth quarter against weaker opponents, indicating clutch performance. Bench players may show unexpectedly high plus-minus in specific quarters. PER tends to peak mid-season but decline in back-to-back games due to fatigue.
Planned Visualizations:
Line Chart: PER over the season to highlight performance trends.
Bar Chart: Points scored by quarter to identify clutch contributors.
Heatmap: Plus-minus by quarter and opponent to reveal matchup strengths.


Note: Visualizations were not created due to time limitations.

6. Suggested Business Actions
Based on the insights, NBA teams could:

Prioritize clutch performers in fourth-quarter lineups.
Adjust defensive strategies for opponents where players underperform.
Schedule rest for key players during back-to-back games to maintain performance levels.

7. Challenges

Time Constraints: Limited availability prevented coding or visualization development.
Data Access: Obtaining granular per-quarter statistics requires advanced scraping or API access, as noted in D7.1.
Data Normalization: Variations in team playing pace complicate cross-player comparisons.

8. Ethical Considerations

Data Privacy: Use only publicly available statistics from reputable sources (e.g., NBA.com, Basketball-Reference) to ensure ethical sourcing.
Bias Mitigation: Validate the dataset to include bench players and smaller-market teams, preventing skewed insights favoring high-profile players.
Responsible Use: Avoid over-reliance on PER, which may undervalue defensive contributions, to ensure fair player evaluations.
AI Transparency: If predictive models were used, ensure coaches understand the methodology to avoid opaque decision-making.
