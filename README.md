# Sales-Prediction

## Quick start

1. Create a virtual environment and install dependencies:


```bash
python -m venv venv
source venv/bin/activate # Linux / macOS
venv\Scripts\activate # Windows
pip install -r requirements.txt
Place your dataset in data/ (CSV). The code expects a Sales column and feature columns such as TV, Radio, Newspaper, Platform, Segment etc.

Run training:

python -m src.train --data data/your_file.csv --target Sales --test-size 0.2

Inspect results and visualizations in outputs/ (created at runtime).
##Results

<img width="501" height="496" alt="image" src="https://github.com/user-attachments/assets/90a4a138-7821-4c5b-b59f-cd98390a4730" />

<img width="518" height="392" alt="image" src="https://github.com/user-attachments/assets/8c7816d4-d193-4244-b0ea-a8d01f9299d5" />


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

<img width="367" height="490" alt="image" src="https://github.com/user-attachments/assets/f9850b11-476f-4f9e-9604-33db952107e0" />



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

![Result Plot](assets/download.png1)
