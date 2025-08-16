#AI Football Analyst: EPL Home & Away Performance
An analysis of English Premier League match data to classify team performance, identifying the strongest home "fortresses" and best away "travelers" using the IBM Granite LLM.

Project Overview
This capstone project dives into over two decades of English Premier League (EPL) match data to uncover patterns in team performance. The core objective is to determine which clubs have a significant home-field advantage and which excel on the road.

The analysis process involves:

Data Processing: Using Python and the Pandas library to calculate the win, draw, and loss percentages for every club, separated into home and away fixtures.

AI-Powered Classification: Feeding this structured statistical data into the ibm-granite/granite-3.2-8-instruct Large Language Model (LLM).

Insight Generation: Leveraging the LLM to classify each team's performance with qualitative labels (e.g., "Fortress," "Inconsistent," "Excellent Traveler") and generate expert-level summaries.

This project demonstrates a modern workflow where traditional data analysis is enhanced by the contextual understanding and summarization capabilities of a powerful AI.

Raw Dataset Link
The dataset used for this analysis is epl_final.csv, which contains detailed match-by-match statistics for the English Premier League from the 2000/01 season to the 2024/25 season.

View the dataset here: epl_final.csv

(Note: You'll need to upload the epl_final.csv file to your repository for this link to work.)

Insight & Findings
The analysis from the IBM Granite model provided a clear classification of each team's performance. Below are the key findings.

Top Home Teams (Fortresses)
These clubs have demonstrated formidable strength at their home stadiums, making them incredibly difficult for visiting teams to beat.

[Team Name 1]: [Enter the model's summary for this team's home performance here. Example: Classified as a 'True Fortress' with a home win percentage of XX%. The model noted their consistent ability to dominate possession and score early goals at home.]

[Team Name 2]: [Enter the model's summary here.]

[Team Name 3]: [Enter the model's summary here.]

Top Away Teams (Best Travelers)
These clubs have shown remarkable resilience and tactical awareness, securing impressive results on the road.

[Team Name 1]: [Enter the model's summary for this team's away performance here. Example: Labeled an 'Excellent Traveler' with an away win percentage of XX%. The AI highlighted their effective counter-attacking strategy as a key factor in their success away from home.]

[Team Name 2]: [Enter the model's summary here.]

[Team Name 3]: [Enter the model's summary here.]

General Observations
[Add any other interesting findings here. For example: The model observed a league-wide trend where the home-field advantage has slightly decreased in the last five seasons.]

[Another finding. For example: Teams finishing in the top four consistently had an away win percentage above XX%.]

AI Support Explanation
The IBM Granite LLM (ibm-granite/granite-3.2-8-instruct) was a critical component of this analysis, serving as an AI-powered data analyst. Its role went beyond simple computation and involved classification, summarization, and contextual interpretation.

Here’s how the AI was utilized:

Structured Prompting: A detailed prompt was engineered to provide the AI with the pre-processed data (home and away win/draw/loss percentages for all teams) and a clear set of instructions. This ensured the output was structured, relevant, and consistent.

Performance Classification: The primary task for the AI was to classify each team's performance using descriptive labels. This transforms raw percentages into meaningful insights that are easier to understand (e.g., turning a "68% home win rate" into a "Fortress" classification).

Insight Summarization: The model was instructed to generate a brief, expert-level summary for each team and to identify the top 3 performers in both home and away categories. This automates the process of drawing final conclusions from the data.

The following parameters were used to ensure a deterministic and focused response from the model:

{
  "temperature": 0.2,
  "top_p": 0.9,
  "top_k": 0,
  "repetition_penalty": 1.1,
  "max_tokens": 512
}

By leveraging the LLM, this project was able to produce a richer, more qualitative analysis than would be possible with statistical calculations alone.
