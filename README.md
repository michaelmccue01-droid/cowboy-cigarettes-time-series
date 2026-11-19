# Cowboy Cigarettes Time Series Case Study

This project completes Springboard's Tier 3 **Cowboy Cigarettes: A Time Series Investigation**. It uses monthly sales from January 1949 through December 1960 to estimate whether sales increased, decreased, or remained stable in the early 1960s.

## Result

The analysis predicts that sales continued to increase while retaining a strong annual seasonal pattern. A seasonal ARIMA model, `SARIMA(0,1,1)(0,1,1,12)`, produced the lowest error on the chronological 1959–1960 holdout period.

- Selected-model holdout MAE: approximately **39 cigarettes per month**
- Seasonal-naive holdout MAE: approximately **71 cigarettes per month**
- Forecast average monthly sales:
  - 1961: approximately **1,000,520**
  - 1962: approximately **1,000,573**
  - 1963: approximately **1,000,631**

## Files

- `Cowboy_Cigarettes_Time_Series_Tier_3.ipynb` — completed and executed analysis
- `CowboyCigsData.csv` — supplied monthly dataset
- `requirements.txt` — Python dependencies

## Run locally

```bash
pip install -r requirements.txt
jupyter notebook Cowboy_Cigarettes_Time_Series_Tier_3.ipynb
```

The notebook keeps the original sales totals for reporting, uses a chronological holdout rather than a random split, compares against a seasonal-naive benchmark, and clearly separates forecasting from causal explanation.

