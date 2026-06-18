# Predictive Analytics for Brasileirão

## A Data Driven Business Strategy for Sports Intelligence

This repository contains my final assignment for the Omni Campus Data Science course. The project uses historical Brasileirão data to build a sports intelligence solution that estimates football match outcome probabilities and translates them into business insights.

The final notebook is not only a machine learning experiment. It is structured as a complete Data Science case study, moving from business context and data preparation to exploratory analysis, model evaluation, insights, strategy proposal, limitations, and conclusion.

## Project Objective

The project answers the following business question:

**Can historical standings and match results provide useful prediction signals for upcoming Brasileirão fixtures?**

The solution is framed for:

- Football clubs that need opponent and fixture intelligence.
- Sports media platforms that need data-driven match previews.
- Fantasy sports products that need fixture difficulty and engagement signals.

The project avoids a betting-centered approach. The model is presented as a decision-support tool for sports intelligence.

## Final Deliverables

- `final_assignment_brasileirao_strategy.ipynb`: final polished notebook in English.
- `brasileirao_strategy_presentation.pptx`: presentation slides for the final assignment.
- `references.md`: references used in the project.
- `IA_FUTEBOL_DADOS.zip`: local dataset used by the notebook.
- `model_predictive_brasileirao_ipynb.ipynb`: original notebook kept for reference.

## Notebook Structure

The final notebook is organized into the following sections:

1. Introduction
2. Business Problem
3. Market Context
4. Dataset Description
5. Data Cleaning and Preparation
6. Exploratory Data Analysis
7. Feature Engineering
8. Machine Learning Model
9. Model Evaluation
10. Business Insights
11. Business Strategy Proposal
12. Limitations
13. Conclusion
14. References

## Dataset

The notebook reads all data from the local file `IA_FUTEBOL_DADOS.zip`.

The ZIP contains:

- `dataset-2003-2022.csv`: season standings and team performance.
- `campeonato-brasileiro-full.csv`: match-level records.
- `campeonato-brasileiro-gols.csv`: goal-level records.

The analysis focuses on Brasileirão data from 2003 to 2022.

## Methodology

The project follows a standard Data Science workflow:

1. Load and inspect the datasets.
2. Clean and standardize team names.
3. Explore historical champions, runners-up, and average points.
4. Engineer simple match-level features.
5. Compare machine learning models.
6. Select the Support Vector Classifier as the final model.
7. Use the model to estimate match outcome probabilities.
8. Translate the results into business insights and a strategy proposal.

## Model Output

The final model estimates probabilities for three possible match outcomes:

- Home team win
- Away team win
- Draw

These probabilities can support dashboards, match previews, opponent analysis, and fantasy sports features.

## Key Business Insights

- Historical dominance helps explain long-term club strength.
- Match-level predictions are more actionable than season-position predictions.
- Probability outputs are easier to use in products than simple win/loss labels.
- Draw prediction remains difficult and should be communicated with uncertainty.
- The model should support human decision-making, not replace it.

## How to Run

1. Keep `IA_FUTEBOL_DADOS.zip` in the project root.
2. Open `final_assignment_brasileirao_strategy.ipynb`.
3. Run all notebook cells from top to bottom.

The notebook does not require Google Drive paths. It reads the local ZIP file directly.

## Main Technologies

- Python
- pandas
- NumPy
- seaborn
- Matplotlib
- scikit-learn
- XGBoost

## Limitations

The model uses a small feature set and does not include player-level data, injuries, transfers, tactical information, or recent form. For a production version, these features should be added and the model should be monitored over time.

## Author

Eduardo Oliveira

## Course

Omni Campus Data Science course final assignment.
