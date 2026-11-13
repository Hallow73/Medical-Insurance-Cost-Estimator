# Medical Insurance Cost Prediction

A machine learning project that predicts annual medical insurance charges based on individual characteristics using regression models. Includes data analysis, model comparison, and an interactive Streamlit application.

## Technologies Used
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- Streamlit
- Jupyter Notebook, VS Code

## Dataset

The dataset includes age, sex, BMI, number of children, smoking status, geographic region, and medical insurance charges.

**Target Variable:** `charges` — Annual medical insurance costs.

## Project Workflow

1. **Data Exploration:** Analyzed insurance costs and relationships between features using visualizations.
2. **Preprocessing:** Handled missing values, encoded categorical variables, and engineered BMI categories.
3. **Model Training:** Trained Linear Regression, Random Forest, and Gradient Boosting models.
4. **Evaluation:** Compared models using R², MAE, and RMSE.
5. **Deployment:** Integrated the selected model into an interactive Streamlit application.

## Streamlit Application

The application allows users to:
- Enter age, sex, BMI, children, smoking status, and region.
- Predict annual medical insurance charges.
- Compare predictions with smoker and non-smoker reference averages.
- Visualize estimated charges using a bar chart.

**[Live Streamlit App]((https://medical-insurance-cost-estimator-mzplkv3xszmd3dr4opgcnj.streamlit.app/))**

## Repository Structure

```text
├── app.py
├── insurance_predictor.ipynb
├── insurance_model.pkl
├── model_features.pkl
├── model_name.pkl
├── requirements.txt
└── README.md
```

## Run Locally

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the application:

```bash
streamlit run app.py
```

## Disclaimer

This project is for educational purposes. Predictions are estimates and do not represent actual insurance quotes.
