# EV-Battery-Project

This project develops a regression-based machine learning framework to model and predict lithium-ion battery prices and average battery electric vehicle (BEV) prices in the United States. Using publicly available datasets sourced from Kaggle, we analyze historical cost trends and evaluate the predictive performance of linear, polynomial, and neural-network regression models. The study leverages PyTorch for custom model development, scikit-learn for preprocessing and evaluation, and Matplotlib for exploratory analysis and visualization. This work is intended as a foundational research effort that can be extended toward EV adoption modeling and energy systems analysis.

1. Introduction

The affordability of electric vehicles is a central determinant of large-scale EV adoption. Two of the most influential cost components in the EV ecosystem are battery pack prices and vehicle purchase prices. While battery costs have declined significantly over the past decade, uncertainty remains regarding future price trajectories and their broader implications for transportation electrification.

This research seeks to quantify historical trends and assess the extent to which regression-based machine learning models can accurately predict battery and EV prices in the U.S. market. Emphasis is placed on methodological transparency, reproducibility, and interpretability, making the framework suitable for academic research and future policy-oriented studies.

2. Research Objectives

The primary objectives of this project are:

To analyze historical trends in U.S. lithium-ion battery prices

To model average electric vehicle price dynamics over time

To evaluate the effectiveness of regression-based ML models for price prediction

To compare linear and nonlinear regression approaches in terms of accuracy and stability

3. Research Questions

How have battery prices evolved in the United States?

What long-term trends are present in average electric vehicle prices?

Can supervised regression models reliably forecast future battery and EV prices?

How does model complexity affect predictive performance and generalization?

4. Data Sources

All datasets used in this study are obtained from Kaggle and consist of aggregated, publicly available data.

Dataset Categories

Historical lithium-ion battery prices (e.g., USD per kWh)

Average electric vehicle prices in the U.S.

Temporal variables (year)

These datasets compile information from industry reports, manufacturer disclosures, and market analyses.

5. Data Preprocessing

The preprocessing pipeline includes:

Handling missing or incomplete values

Feature normalization and scaling

Temporal alignment across datasets

Train–validation–test splits to avoid data leakage

All preprocessing steps are implemented using scikit-learn and documented to ensure reproducibility.

6. Methodology
6.1 Modeling Approach

This project applies supervised regression techniques, including:

Linear Regression as a baseline model

Polynomial Regression to capture nonlinear trends

Neural Network Regression implemented using PyTorch

The objective is to model price trajectories over time rather than establish causal relationships.

6.2 Libraries and Tools

PyTorch

Custom neural network regression models

Gradient-based optimization

scikit-learn

Data preprocessing

Baseline regression models

Cross-validation and evaluation metrics

Matplotlib

Exploratory data analysis

Trend visualization

Residual and prediction plots

7. Evaluation Metrics

Model performance is evaluated using standard regression metrics:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Coefficient of Determination (R²)

These metrics enable consistent comparison across modeling approaches.

8. Results Summary

Key findings from the analysis include:

Battery prices exhibit a strong long-term downward trend consistent with technological learning effects.

Average EV prices show a slower decline with periods of market volatility.

Nonlinear regression models outperform linear baselines in capturing complex pricing dynamics.

Increased model complexity must be carefully managed to avoid overfitting and reduced generalization.

Detailed plots and numerical results are provided in the repository.

9. Repository Structure
├── data/
│   ├── raw/                 # Original Kaggle datasets
│   └── processed/           # Cleaned and normalized datasets
│
├── notebooks/
│   ├── exploratory_analysis.ipynb
│   ├── regression_models.ipynb
│   └── evaluation.ipynb
│
├── models/
│   ├── sklearn_models.py
│   └── pytorch_regression.py
│
├── figures/
│   ├── trends/
│   ├── predictions/
│   └── residuals/
│
├── requirements.txt
├── README.md
└── LICENSE

10. Reproducibility

To reproduce the results:

Clone the repository

Install dependencies

pip install -r requirements.txt


Run the notebooks in sequence

Review generated figures and evaluation metrics

All experiments are deterministic when random seeds are fixed.

11. Limitations

Data is aggregated and may obscure regional or model-level variation

The study focuses on correlation rather than causal inference

External factors such as policy incentives, fuel prices, and supply chain disruptions are not explicitly modeled

Forecast uncertainty increases over longer time horizons

12. Future Work

Potential extensions of this research include:

Incorporating vehicle range and battery capacity as explanatory variables

Integrating EV sales and adoption data

Applying panel data or fixed-effects regression

Comparing results with time-series and diffusion-based models

Scenario-based forecasting under alternative battery cost trajectories

13. Research Relevance

This project is relevant to:

Energy systems and sustainability research

Transportation electrification studies

Battery economics and cost forecasting

Applied machine learning in climate and energy domains
