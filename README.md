# Soil Measures: Crop Prediction 🌱

## Project Overview
This project uses machine learning to identify the most predictive soil feature for classifying the optimal crop based on soil measurements.

## Dataset
The `soil_measures.csv` dataset contains:
- **N:** Nitrogen content
- **P:** Phosphorus content
- **K:** Potassium content
- **pH:** Soil pH value
- **crop:** Target variable

## Methodology
A multiclass classification model was trained and evaluated using the F1-score to determine the predictive performance of each soil feature individually.

## Results

| Feature | F1-score |
|---|---:|
| N | 0.1222 |
| P | 0.1682 |
| K | 0.2691 |
| pH | 0.0748 |

**Best predictive feature:** Potassium (`K`), with an F1-score of **0.2691**.

```python
best_predictive_feature = {'K': 0.2691443992676175}
```

## Conclusion
Potassium (`K`) achieved the highest F1-score among the four soil features, making it the best individual predictor of crop type in this evaluation.
