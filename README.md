# Project Readme: Manchester City Football Club Performance Analysis Dashboard

## Overview
This project involves analyzing the performance of Manchester City Football Club using a dataset (`spi_matches.csv`) from [FiveThirtyEight's Soccer Power Index (SPI)](https://fivethirtyeight.com/). The dataset is transformed, cleaned, and enriched with additional columns to provide insights into the team's performance across different seasons. A dashboard is then created to visualize key metrics such as points tally, goals scored, clean sheets, and more.

Below is a step-by-step explanation of the project workflow:

---

## Step 1: Upload the CSV File
- The dataset `spi_matches.csv` is uploaded into the project environment.
- This dataset contains information about football matches, including team performance metrics, dates, and match outcomes.

---

## Step 2: Transform the Dataset
### 2.1 Remove Unimportant Columns
- Columns that are irrelevant to the analysis (e.g., columns not related to Manchester City or match outcomes) are removed to streamline the dataset.

### 2.2 Rename Columns
- Columns are renamed for better readability and consistency. For example:
  - `team1` → `Home Team`
  - `team2` → `Away Team`
  - `score1` → `Home Goals`
  - `score2` → `Away Goals`

### 2.3 Add New Columns
- New columns are added to enrich the dataset:
  - **Points**: Calculated based on match results (3 for a win, 1 for a draw, 0 for a loss).
  - **Opponents**: The opposing team in each match.
  - **Result**: The outcome of the match (Win, Loss, or Draw).
  - **Match Type**: Whether the match was played at home or away.
  - **Season**: The season in which the match was played (e.g., 2020-2021).

---

## Step 3: Extract Manchester City Matches
- The dataset is filtered to include only matches involving Manchester City.
- This ensures the analysis focuses solely on the team's performance.

---

## Step 4: Divide Matches into Tables
- The filtered dataset is divided into smaller tables based on:
  - **Match Type**: Home or Away.
  - **Season**: The season in which the match was played.
- This division allows for more granular analysis of performance across different contexts.

---

## Step 5: Append All Tables into One
- After transforming and dividing the data, all smaller tables are combined into a single table.
- This consolidated table is used for further analysis and dashboard creation.

---

## Step 6: Create New Measures
- Key performance metrics are calculated for each season:
  - **Points Tally**: Total points accumulated in a season.
  - **Clean Sheets**: Matches where Manchester City conceded no goals.
  - **Wins per Opponent**: Number of wins against each opponent.
  - **Losses per Opponent**: Number of losses against each opponent.
  - **Draws per Opponent**: Number of draws against each opponent.
  - **Goal Difference**: Difference between goals scored and conceded.
  - **Total Goals**: Total goals scored in a season.
  - **Goals Conceded**: Total goals conceded in a season.

---

## Step 7: Build the Dashboard
The dashboard is created using a Power BI. It includes the following visualizations:

### 7.1 Line and Stacked Column Charts
- **Points Tally and Goal Difference per Season**:
  - A line chart shows the points tally across seasons.
  - A stacked column chart shows the goal difference (goals scored vs. goals conceded) for each season.

- **Total Goals and Projected Goals per Season**:
  - A line chart shows the total goals scored each season.
  - A stacked column chart compares actual goals with projected goals (if available in the dataset).

- **Clean Sheets and Conceded Goals per Season**:
  - A line chart shows the number of clean sheets each season.
  - A stacked column chart shows the total goals conceded each season.

### 7.2 Doughnut Charts
- **Top 6 Most Wins Against Opponents**:
  - A doughnut chart visualizes the top 6 opponents Manchester City has won against the most.

- **Top 6 Losses Against Opponents**:
  - A doughnut chart visualizes the top 6 opponents Manchester City has lost against the most.

- **Top 6 Draws Against Opponents**:
  - A doughnut chart visualizes the top 6 opponents Manchester City has drawn against the most.

---

## Step 8: Finalize and Share the Dashboard
- The dashboard is finalized by ensuring all visualizations are clear, labeled, and interactive.
- The dashboard is shared with stakeholders for insights into Manchester City's performance over the seasons.

---

## Tools Used
- **Data Cleaning and Transformation**: Power BI's Power Query Editor.
- **Dashboard Creation**: Power BI.
- **Dataset**: `spi_matches.csv` from FiveThirtyEight.

---

## Key Insights
- The dashboard provides a comprehensive view of Manchester City's performance, including:
  - Trends in points tally and goal difference over seasons.
  - Performance against specific opponents.
  - Defensive performance (clean sheets and goals conceded).
  - Offensive performance (goals scored and projected goals).

---

## How to Use This Project
1. Clone the repository or download the dataset and scripts.
2. Run the data transformation script (if using Python) or open the cleaned dataset in your preferred tool.
3. Open the dashboard file  `Mancity Analysis.pbix` to explore the visualizations.
4. Customize the dashboard as needed for further analysis.

---

## Future Enhancements
- Incorporate additional datasets (e.g., player statistics, transfer data) for deeper insights.
- Add predictive analytics to forecast future performance.
- Include more interactive features in the dashboard (e.g., filters for specific opponents or seasons).

---

## Contact
For questions or feedback, please reach out to [Your Name] at [Your Email].

---

Thank you for exploring this project!
