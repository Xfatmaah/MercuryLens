# MercuryLens: Predictive Modeling of Chemical Contaminants

**MercuryLens** is a machine learning framework designed to predict fish consumption safety levels (**Safe, Moderate, and High Risk**) across Ontario’s 250,000 lakes. By transitioning from static lookup tables to an automated predictive system, we provide a robust tool for public health and food safety.

## Key Results
- **Champion Model:** Stacking Ensemble (LightGBM + CatBoost + Random Forest).
- **Final Accuracy:** **83.25%**
- **Recall (High-Risk):** **0.83** (Prioritizing public safety to minimize False Negatives).

## Key Features & Methodology
- **Spatial Intelligence:** Implemented **Geospatial Scaling** and **Coordinate Binning** to identify localized "Pollution Pockets."
- **Numerical Transformation:** Converted text-based length ranges into quantitative risk drivers (**Mean_Length**).
- **Dual-Branch Pipeline:** Custom encoding for tree-based models vs. native categorical handling for CatBoost.
- **Stacking Ensemble:** Fused multiple architectures using a Logistic Regression meta-model to stabilize boundary predictions.

## Performance Leaderboard
| Model | Accuracy | F1-Score |
| :--- | :---: | :---: |
| **Stacking Ensemble** | **83.25%** | **0.83** |
| LightGBM | 83.14% | 0.83 |
| CatBoost | 81.24% | 0.82 |
| Random Forest (Baseline) | 76.00% | 0.76 |

---
*Developed as part of the CSAI 801-AI & Machine Learning Course.*
