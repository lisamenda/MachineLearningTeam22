# MachineLearningTeam22
# Good Neighbors, Quieter Nights: Modeling Noise Complaint Patterns Using 311 Data

This repository contains a Jupyter notebook and associated data analysis aimed at predicting spikes in noise complaints using Allegheny County's 311 noise complaint data. The goal is to help local authorities proactively allocate resources and manage community disturbances effectively.

## Project Overview

The analysis utilizes machine learning to predict weeks when noise complaints exceed operational thresholds (≥ 3 complaints per week per census tract). Temporal, spatial, and demographic data from census tracts have been integrated to ensure robust and equitable predictions.

## Requirements

To run this notebook, ensure you have Python 3 installed along with the following libraries:

- pandas
- numpy
- scikit-learn
- imblearn
- matplotlib
- seaborn
- xgboost
- holidays
- jupyter

You can install all required libraries using pip:

```bash
pip install pandas numpy scikit-learn imblearn matplotlib seaborn xgboost holidays jupyter
```

## Data Preparation

- Obtain the dataset (`311Full.csv`) and census data from the API key in the notebook, placing them in the same directory as your notebook.
- The notebook automatically filters for noise-related complaints and performs extensive feature engineering.

## How to Use the Notebook

1. **Clone the Repository**:
   ```bash
   git clone [repository-url]
   cd [repository-folder]
   ```

2. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Run the notebook cells sequentially**:
   - Start from the top, executing cells to load data, preprocess it, train models, and evaluate performance.
   - Modify hyperparameters and feature sets within the notebook cells if further tuning or analysis is needed.

## Understanding the Results

The notebook outputs detailed metrics (Accuracy, Precision, Recall, F1-Score), emphasizing recall to ensure critical complaint spikes are detected. A bias audit funciton is included to evaluate equitable model performance across demographic groups.
