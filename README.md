# 🎮 SQL Analysis of Video Game Sales

This project analyzes the [Video Game Sales with Ratings dataset](https://www.kaggle.com/datasets/rush4ratio/video-game-sales-with-ratings) using SQL in a Jupyter Notebook with SQLite.

## 📌 Objective
To extract actionable business insights using SQL queries, focusing on game sales trends by genre, platform, publisher, and score-based performance.

## 🧰 Tools Used
- Python (Pandas)
- SQLite
- Jupyter Notebook

## 📊 Key SQL Analyses

1. **Average Sales by Genre**
   - Platform, Shooter, and Sports genres have the highest average sales.
2. **Platform Trends Over Years**
   - Sales spikes observed for platforms like Wii and PS2 during specific years.
3. **Top 3 Titles by Publisher**
   - Nintendo and Rockstar have the most commercially successful top titles.
4. **Critic Score vs Sales**
   - High critic score doesn't guarantee high sales; other factors intervene.
5. **Critic vs User Score Gaps**
   - Notable score gaps reveal misalignment between expert reviews and public reception.

## 🔍 Sample Query

```sql
SELECT Genre, ROUND(AVG(Global_Sales), 2) AS Avg_Sales
FROM games
GROUP BY Genre
ORDER BY Avg_Sales DESC;

## 📊 Tableau Visualizations

Explore the interactive dashboards by clicking the images below:

### 1. Genre vs Average Global Sales
[![Genre Sales](images/genre_sales.png)](https://public.tableau.com/views/VideoGameGenreSales/Chart1)

### 2. Platform Sales Over Time
[![Platform Sales](images/platform_trend.png)](https://public.tableau.com/views/PlatformSalesOverYears/Chart2)

### 3. Publisher Top Games
[![Top Games](images/publisher_top_games.png)](https://public.tableau.com/views/TopPublisherGames/Chart3)

### 4. Critic Score vs Global Sales
[![Score vs Sales](images/critic_vs_sales.png)](https://public.tableau.com/views/CriticScoreVsSales/Chart4)

### 5. Critic vs User Score Gap
[![Score Gap](images/score_gap.png)](https://public.tableau.com/views/ScoreGapAnalysis/Chart5)
