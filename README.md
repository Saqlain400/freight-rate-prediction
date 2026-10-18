# freight-rate-prediction
Freight Rate Prediction using Machine Learning

## Project Overview
This project predicts freight rates using machine learning based on shipment details, including pickup and delivery locations, distance, equipment type, weight, date, market index, and quote signal.

## Model Performance
The selected model is **Ridge Regression**.

| Metric | Result |
|---|---:|
| Mean Absolute Error (MAE) | 142.76 |
| Root Mean Squared Error (RMSE) | 637.58 |
| R² Score | 0.8252 |

These results are from the project's reported train/test evaluation.

## Project Files
- `main.ipynb` — Model development and analysis notebook.
- `score.py` — Assessment scoring and validation script.
- `Requirements.txt` — Python dependencies.
- `best_freight_rate_model.pkl` — Saved model artifact.
- `validation_predictions.csv` — Predictions for 12,000 validation records.
- `december_chart_inputs.csv` — December prediction inputs and results.
- `candidate_december.png` — Generated December prediction chart.
- `Freight_Rate_Prediction_Final_Report.docx` — Final project report.

## Installation
Python 3.10 or later is recommended.

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Validation
Run the assessment validation script:

```bash
python score.py --predictions validation_predictions.csv --december-predictions december_chart_inputs.csv
```

The script validated 12,000 validation predictions and 31 December predictions, and generated the December chart.

## Notes
Final validation metrics are calculated by Spotter after submission. The reported train/test metrics should not be interpreted as official final validation results.

