# Sales-Prediction


Predict future sales from advertising spend and other features. This repository includes data preparation, modeling (Linear Regression & Random Forest), simple time-series forecasting with lag features, evaluation and visualizations.


## Quick start


1. Create a virtual environment and install dependencies:


```bash
python -m venv venv
source venv/bin/activate # Linux / macOS
venv\Scripts\activate # Windows
pip install -r requirements.txt
##Results
<img width="986" height="986" alt="image" src="https://github.com/user-attachments/assets/a1aa6de7-f43d-4351-b1e8-9dc44c506968" />
<img width="486" height="374" alt="image" src="https://github.com/user-attachments/assets/651fdad9-7e44-4685-a8d9-0158265d99c4" />
Linear Regression Performance:
RMSE: 1.782
R² Score: 0.899

Random Forest Performance:
RMSE: 0.769
R² Score: 0.981


Linear Regression Coefficients:
     Feature  Coefficient
1      Radio     0.189195
0         TV     0.044730
2  Newspaper     0.002761

Random Forest Feature Importances:
     Feature  Importance
0         TV    0.624810
1      Radio    0.362201
2  Newspaper    0.012989
<img width="592" height="393" alt="image" src="https://github.com/user-attachments/assets/f2c6c7b6-ae86-415e-a587-8effde0886b8" />
Time Series Style Model:
Linear Regression with Lag Feature Performance:
RMSE: 1.683
R² Score: 0.894


Business Insights:
1. TV advertising has the strongest positive impact on sales, followed by Radio.
2. Newspaper spend shows little to no impact, suggesting budget can be reallocated.
3. Regression and Random Forest both confirm diminishing returns after certain ad spends.
4. Including past sales as a feature improves forecasting, useful for demand planning.
5. Marketing strategy: prioritize TV and Radio spend, reduce Newspaper allocation.
