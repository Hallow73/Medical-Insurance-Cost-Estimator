# Medical Insurance Cost Prediction

A machine learning project that predicts annual medical insurance charges based on individual characteristics using regression models. The project includes exploratory data analysis, feature engineering, model evaluation, and an interactive Streamlit web application.

## Project Overview

The goal of this project is to analyze factors influencing medical insurance costs and build a predictive model that estimates annual insurance charges.

The application allows users to enter personal information and receive an estimated insurance cost using a trained machine learning model.

## Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Joblib
- Streamlit
- Jupyter Notebook, VS Code

## Dataset

The dataset contains information about individuals and their medical insurance charges.

**Input Features:**

| Feature | Description |
|---------|-------------|
| Age | Age of the individual |
| Sex | Male or female |
| BMI | Body Mass Index |
| Children | Number of dependents |
| Smoker | Smoking status |
| Region | Geographic region |

**Target Variable:** `charges` — Annual medical insurance charges.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

- Examined dataset structure and statistical summaries.
- Analyzed distributions of insurance charges.
- Explored relationships between demographic characteristics and medical costs.
- Visualized relationships using Matplotlib and Seaborn.

### 2. Data Preprocessing and Feature Engineering

- Checked for missing values and duplicate records.
- Encoded categorical variables into numerical features.
- Created BMI categories based on weight classification.
- Prepared features for machine learning models.
- Applied a logarithmic transformation to insurance charges for model training.

### 3. Machine Learning Models

Trained and compared three regression models:

1. **Linear Regression** — Establishes a baseline for predicting insurance costs.
2. **Random Forest Regressor** — Captures nonlinear relationships using an ensemble of decision trees.
3. **Gradient Boosting Regressor** — Sequentially combines decision trees to improve predictive performance.

### 4. Model Evaluation

Evaluated regression performance using:

- **R² Score:** Measures the proportion of variance explained by the model.
- **Mean Absolute Error (MAE):** Average absolute difference between predicted and actual charges.
- **Root Mean Squared Error (RMSE):** Measures prediction error while penalizing larger errors.

The selected model is saved using Joblib and integrated into the Streamlit application.

## Streamlit Web Application

An interactive web application allows users to estimate annual medical insurance charges.

**Application Features:**

- Input age, sex, BMI, number of children, smoking status, and region.
- Generate estimated annual medical insurance charges.
- Display predictions in USD.
- Compare estimated charges with reference averages for smokers and non-smokers.
- Visualize results using an interactive bar chart.

### Live Demo

[Medical Insurance Cost Predictor](YOUR_STREAMLIT_APP_URL)

*Replace `YOUR_STREAMLIT_APP_URL` with your deployed Streamlit website link.*

## Repository Structure

```text
medical-insurance-cost-prediction/
│
├── app.py
├── insurance_predictor.ipynb
├── insurance_model.pkl
├── model_features.pkl
├── model_name.pkl
├── requirements.txt
└── README.md
```

## Installation and Usage

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/medical-insurance-cost-prediction.git
cd medical-insurance-cost-prediction
```

**2. Install required libraries**

```bash
pip install -r requirements.txt
```

**3. Run the Streamlit application**

```bash
streamlit run app.py
```

**4. Open the application**

The application will automatically open in your browser at:

`http://localhost:8501`

## Future Improvements

- Add additional predictive models and hyperparameter tuning.
- Incorporate more relevant insurance and health-related features.
- Improve model interpretability through feature importance analysis.
- Add additional visualizations and model performance comparisons.
- Expand the Streamlit dashboard with interactive analysis features.

## Disclaimer

This project is intended for educational and data science portfolio purposes. Predicted charges are estimates based on sample data and do not represent actual insurance quotes or guaranteed healthcare expenses.
