### Boston House Price Prediction – End-to-End ML Deployment

### Project Overview

This project demonstrates an end-to-end Machine Learning workflow, from data exploration and model training to deployment using Flask, and web apps. The goal is to predict median house prices in Boston using socio-economic and housing attributes.

### Mission

To build and deploy a production-ready regression model that predicts house prices while demonstrating best practices in ML preprocessing, evaluation, and inference consistency.

### Objective

- Train a regression model on the Boston Housing dataset

- Ensure consistent preprocessing during training and inference

- Deploy the model using a Flask web application

- Provide both REST API and web-based UI for predictions

### Problem Statement

Predict the median value of owner-occupied homes (in $1000s) based on 13 housing and socio-economic features such as crime rate, number of rooms, tax rate, and population status.

### Dataset

- Source: OpenML – Boston Housing Dataset

- Samples: 506

- Features: 13 numerical & categorical variables

- Target: MEDV (Median house price in $1000s)

### Software and Tools Requirements

1. [GithubAccount](https://github.com)
2. [HerokuAccount](https://www.heroku.com/)
3. [VSCodeIDE](https://code.visualstudio.com/)
4. [GitCLI](https://git-scm.com/)


### Create a new environment

```
conda create -p venv python==3.13.7 -y
```

### Tech Stack

- Python

- Pandas, NumPy

- Scikit-learn

- Flask

- HTML/CSS

- Pickle

### What I Did (Key Highlights)

- Performed Exploratory Data Analysis (EDA) with correlation analysis

- Identified key relationships between features and target

- Applied StandardScaler for feature normalization

- Trained a Linear Regression model

- Evaluated model using MAE, RMSE, R², Adjusted R²

- Serialized both model and scaler to ensure inference consistency

### Built:

- A REST API for programmatic predictions

- A web UI for user-friendly input and output

### Methodology / Workflow

- Data loading and cleaning

- Exploratory Data Analysis (EDA)

- Feature-target split

- Train-test split

- Feature standardization

- Model training (Linear Regression)

- Model evaluation

- Model & scaler serialization

- Flask-based deployment

### Model Performance
```

| Metric      | Value |
| ----------- | ----- |
| MAE         | ~3.16 |
| RMSE        | ~4.63 |
| R² Score    | ~0.71 |
| Adjusted R² | ~0.68 |

```
The model explains ~71% of variance in housing prices on unseen data.

### Application Features

- Web-based form for manual input

- REST API endpoint (/predict_api) for JSON requests

- Input standardization during inference

- Real-time prediction output

### Limitations

- Linear Regression has no lower bound, which may produce unrealistic values for extreme inputs

- Dataset is relatively small and historical

- No feature selection or regularization applied

- No production-grade monitoring or logging

### Future Improvements

- Use Ridge / Lasso / Random Forest

- Add input validation & constraints

- Apply cross-validation

- Improve UI/UX

### Key Learning Outcomes

- Importance of consistent preprocessing in ML deployment

- Real-world issues with model inference

- End-to-end ML pipeline implementation

- Practical experience with Flask + ML integration

### Why This Project Matters

- This project reflects real-world ML engineering challenges, not just model accuracy.
- It highlights deployment awareness, data preprocessing discipline, and full-stack ML thinking.

### Author

### Muhammad Usman
Aspiring Machine Learning / Data Science Engineer