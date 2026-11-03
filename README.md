# Ames Housing Price Prediction

ECPI University coursework completed in June 2026 by Jerald Bradley.

I used 1,460 Ames housing records to predict home sale prices and explore how neighborhood, renovation history, and property size relate to prices. The project combines Python modeling with an interactive Power BI report.

## Modeling workflow

- Prepared 24 predictors with missing-value handling, feature engineering, standardization, and one-hot encoding, yielding 88 model inputs.
- Compared a scikit-learn linear regression baseline with a TensorFlow/Keras neural network using MAE, RMSE, and R².
- Linear regression performed better on the 292-record evaluation subset, with an MAE of $18,609, an RMSE of $29,571, and an R² of 0.886.

## Power BI report

The report has four pages covering the executive overview, feature relationships, model performance, and scenario analysis. The scenario page compares modeled price changes for neighborhood, renovation, and property expansion. Expansion had the largest change, increasing average predicted sale price by 11.26% under the simulated inputs.

## Files and setup

- [Housing_Modeling.ipynb](Housing_Modeling.ipynb) contains preprocessing, model training, and evaluation.
- [Ames_Housing_Report.pbix](Ames_Housing_Report.pbix) opens in Power BI Desktop.

To run the notebook, install pandas, NumPy, Matplotlib, scikit-learn, and TensorFlow in your Jupyter environment. Download train.csv from the [Kaggle House Prices competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data), place it next to the notebook, and update the data-loading cell to use a relative path.
