Football Match Prediction & Power BI Dashboards
This project applies machine learning and data visualization to predict and analyze Premier League match outcomes. It combines:
1. A Python Notebook for feature engineering, model training, and evaluation
2. Power BI Dashboards for interactive insights into both model predictions and season performance
Dataset
The dataset is publicly available here:
👉 Football Data (Premier League): https://www.football-data.co.uk/englandm.php

It includes detailed match results, goals, and outcomes across multiple Premier League seasons.
Part 1: Machine Learning Notebook (Football_prediction.ipynb)
Workflow
1. Data Preparation
- Combined 5 seasons of CSV files into one dataset
- Created target variable HomeWin (1 = home win, 0 = otherwise)

2. Feature Engineering
- Rolling averages for team stats before each match: Goals For, Goals Against, Win Rate
- Difference metrics between home & away teams

3. Model Training
- Train/Test split
- Pipeline: StandardScaler + Logistic Regression

4. Evaluation
- Accuracy & ROC AUC (≈ 0.71)
- Confusion Matrix
- Calibration Curve (Predicted vs Observed win probabilities)

5. Insights
- Model performs moderately well, better than random guessing
- Teams like Liverpool, Man United, and Tottenham show strong home advantage
- Predicted probabilities need better calibration
  
Part 2: Power BI Dashboards
1. Match Predictions & Model Evaluation
- ROC Curve & AUC → classification performance
- Confusion Matrix → predicted vs actual outcomes
- Calibration Curve → reliability of probabilities
- Home Advantage Analysis → teams performing stronger at home
- Match-Specific Predictions → select matches and view winning chance

Purpose: Explain how accurate and reliable the model is.
2. Season Performance Dashboard
- League Table with wins, losses, goals, points
- Best Team Highlight (e.g., Man City this season)
- Goals For vs Against chart → attacking vs defensive balance
- Win Rate Comparison across all teams
- Last 10 Matches for trend insights
- Season & Team Filters (2021–2026) for flexible exploration

Purpose: Explore team performance and league-wide trends.

Tools & Technologies
- Python: Pandas, Scikit-learn, Matplotlib, Seaborn
- Power BI: Interactive dashboards & data visualization
- Dataset: Premier League results from football-data.co.uk
  
How to Run
Python Notebook
1. Clone this repository
2. Download CSV files and store in Football/ folder
3. Run Football_prediction.ipynb to train & evaluate model
   
Power BI Dashboards
1. Download .pbix file from this repository
2. Open in Power BI Desktop
3. Explore dashboards using filters

 
Future Enhancements
- Try advanced models: Random Forest, XGBoost, Deep Learning
- Add external features (player stats, injuries, betting odds)
- Live data integration for real-time predictions
- Expand dashboards to other leagues
- 
Author
Created by Manasi KS – passionate about Sports and Data  Analytics.
Let’s connect on LinkedIn  - https://www.linkedin.com/in/manasi-ks-0b697327a/
