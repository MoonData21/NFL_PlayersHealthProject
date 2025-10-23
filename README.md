# NFL_PlayersHealthProject

Project Overview:
Built a machine learning classification system to predict NFL player health and availability for the 2025 season using historical performance, age, and injury data. The project introduces a data-driven “HealthGrade” and “RiskTier” system, quantifying player durability and projecting injury risk by position.

Key steps and features:

Created an AvgSeasonGames metric to normalize player availability (3-year average for veterans, 2-year for recent players, 2024 data for rookies).

Engineered custom health features:

HealthGrade – overall health score based on player availability.

HealthStatus – categorical indicator from 0 (Healthy) to 4 (Significant Injuries).

Developed InjuryRiskScore and AdjustedRisk variables combining injury history, age, and health grade.

Classified players into risk tiers (“Low,” “Moderate,” “High,” “Significant”) for interpretability.

Trained Random Forest Classifiers (with cross-validation) per position group to predict whether players will play more than 14 games in 2025.

Incorporated manual overrides for special cases (e.g., season-ending injuries).

The final model outputs both a binary health prediction and a risk classification for every player, supporting data-driven forecasting and player health analytics.

Tech Stack: Python, Pandas, Scikit-learn, Random Forest, Feature Engineering, and Cross-Validation.
