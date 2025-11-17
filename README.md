# Telco Churn Predictor

Short description
This repository contains a simple Telco customer churn prediction notebook that trains Logistic Regression and Random Forest models and saves the best model.

Requirements
- Python 3.8+
- pandas
- numpy
- scikit-learn
- joblib
- openpyxl (for reading Excel files)
Install quickly:
```
pip install pandas numpy scikit-learn joblib openpyxl
```

Files
- TelcoChurn.ipynb — Jupyter notebook that loads data, preprocesses, trains models, evaluates, and saves the best model.
- telco_customer_churn.xlsx — Place this dataset file in the notebook working directory before running.
- best_model_<model_name>.joblib — Output model file saved to the working directory after running.

How to run
- Open `TelcoChurn.ipynb` in JupyterLab / Jupyter Notebook and run all cells.
- Or open in Colab via the badge in the notebook and run there (upload the Excel file into the Colab session).

Notes
- The notebook expects a target column named `churn` with values 'Yes'/'No' (case-insensitive). It converts these to 1/0.
- Preprocessing: numeric columns are median-imputed and scaled; categorical columns are one-hot encoded.
- Model selection: the notebook saves the model with the higher F1 score as `best_model_<model_name>.joblib`.

License
MIT
