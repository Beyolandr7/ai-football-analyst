# AI Football Analyst: EPL Home & Away Performance
An analysis of English Premier League match data to classify team performance, identifying the strongest home "fortresses" and best away "travelers" using the IBM Granite LLM.

## Project Overview
This capstone project dives into over two decades of English Premier League (EPL) match data to uncover patterns in team performance. The core objective is to determine which clubs have a significant home-field advantage and which excel on the road.

The analysis process involves:

Data Processing: Using Python and the Pandas library to calculate the win, draw, and loss percentages for every club, separated into home and away fixtures.

AI-Powered Classification: Feeding this structured statistical data into the ibm-granite/granite-3.2-8-instruct Large Language Model (LLM).

Insight Generation: Leveraging the LLM to classify each team's performance with qualitative labels (e.g., "Fortress," "Inconsistent," "Excellent Traveler") and generate expert-level summaries.

This project demonstrates a modern workflow where traditional data analysis is enhanced by the contextual understanding and summarization capabilities of a powerful AI.

## Raw Dataset Link
The dataset used for this analysis is epl_match_stats.csv, which contains detailed match-by-match statistics for the English Premier League from the 2000/01 season to the 2024/25 season.

View the dataset here: [epl_match_stats.csv](https://github.com/Beyolandr7/ai-football-analyst/blob/410ea889b79aa6b7ea843324e418c90bceecae97/epl_match_stats.csv)

## Acknowledgements
This project utilizes the "English Premier League (EPL) Match Data 2000-2025" dataset, which was generously compiled and shared by Marco Hui on Kaggle.

Dataset Creator: Marco Hui

Source: [Kaggle Dataset Link](https://www.kaggle.com/datasets/marcohuiii/english-premier-league-epl-match-data-2000-2025)

A big thank you to the creator for making this valuable data publicly available.

## Insight & Findings
The analysis from the IBM Granite model provided a clear classification of each team's performance. Below are the key findings.

**Top 3 Clubs with the Best Home Record (Fortresses):**

1. **Manchester City** - 65.11% wins (65.11% wins, 16.0% draws, 18.89% losses)
   - Man City has an exceptional home record, winning over 65% of their matches at home, making them one of the strongest home teams in the Premier League.

2. **Manchester United** - 67.8% wins (67.8% wins, 17.48% draws, 14.71% losses)
   - Man United boasts the highest win percentage among home teams, winning nearly 68% of their home games. This demonstrates their formidable presence at Old Trafford.

3. **Chelsea** - 63.75% wins (63.75% wins, 23.45% draws, 12.79% losses)
   - Chelsea's home performance is also remarkable, with a win rate just below Manchester City and United. Stamford Bridge has traditionally been a tough place for opponents.

### Away Performance Analysis

**Top 3 Clubs with the Best Away Record (Best Travelers):**

1. **Manchester City** - 46.0% wins (49.89% wins, 24.52% draws, 25.59% losses)
   - Despite their dominance at home, Man City also performs well away from home, securing victories in nearly 46% of their away games, showcasing their ability to adapt to different venues.

2. **Manchester United** - 49.89% wins (46.0% wins, 21.78% draws, 32.22% losses)
   - Man United's away record is robust, with wins in just over 50% of their away matches, highlighting their consistency on the road.

3. **Chelsea** - 50.0% wins (50.0% wins, 22.44% draws, 27.56% losses)
   - Chelsea rounds out the top 3 away teams, with a win rate of 50% in their away fixtures, indicating they remain competitive regardless of the venue.

### Other Notable Findings:

- **Arsenal** stands out with a significant home advantage, even though they won 67.09% of their matches at the Emirates Stadium, they drew 20.73% of their home games.

- **Birmingham** has the worst home record, winning only 36.92% of their matches at St. Andrew's, and the poorest away record, winning just around 17% of their home games.
  
- **Huddersfield** and **Ipswich** have the lowest combined home and away win rates (42.11% and 32.73% respectively), suggesting overall poor performance.
  
- **Leeds** and **Norwich** show a considerable gap between their home and away performance, with Leeds performing significantly better at home (36.64% vs 33.85%) and Norwich worse (29.77% vs 11.45%).

## AI Support Explanation
The IBM Granite LLM (ibm-granite/granite-3.2-8-instruct) was a critical component of this analysis, serving as an AI-powered data analyst. Its role went beyond simple computation and involved classification, summarization, and contextual interpretation.

Here’s how the AI was utilized:

Structured Prompting: A detailed prompt was engineered to provide the AI with the pre-processed data (home and away win/draw/loss percentages for all teams) and a clear set of instructions. This ensured the output was structured, relevant, and consistent.

Performance Classification: The primary task for the AI was to classify each team's performance using descriptive labels. This transforms raw percentages into meaningful insights that are easier to understand (e.g., turning a "68% home win rate" into a "Fortress" classification).

Insight Summarization: The model was instructed to generate a brief, expert-level summary for each team and to identify the top 3 performers in both home and away categories. This automates the process of drawing final conclusions from the data.
