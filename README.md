
# Olympic Medal Prediction

A data-driven project predicting the number of medals each country would win at the 2016 Summer Olympics using socio-economic and historical performance indicators.
Developed as part of the MSc Data Analytics program at the University of Glasgow.

Overview:

This project applies statistical modeling and dimensionality reduction to forecast Olympic medal counts using historical data (2000–2016).
A Zero-Inflated Negative Binomial (ZINB) model was selected to handle the overdispersion and excess zeros common in medal count data.

Methodology:

Data Sources: Historical Olympic results and socio-economic indicators (GDP, population, etc.)

Data Cleaning & Imputation: Missing values handled with KNN (k = 5)

Dimensionality Reduction: PCA applied, retaining 6 principal components

Modeling: Compared Negative Binomial vs. ZINB; the ZINB model outperformed with lower error metrics

Evaluation Metrics:

MAE = 3.329

MSE = 21.125

RMSE = 4.596

Key Findings:

Recent and historical performance are the strongest predictors of medal success.

GDP and population significantly influence total medals.

ZINB model effectively handles countries with few or zero medals.

Future Work:

Extend to gold medal predictions.

Perform deeper analysis using SQL (per-capita and per-athlete metrics).

Update data to include 2020 and 2024 Olympics for predicting 2028 results.

Tech Stack:

Python

pandas, numpy, statsmodels, matplotlib, seaborn, scikit-learn

Files:

Olympic_medal_prediction.ipynb — Main analysis and modeling
olympics2016 - dataset