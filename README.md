# 🌿 CSIRO Biomass Prediction using Machine Learning

## 📌 Project Overview
This project focuses on predicting **plant biomass using machine learning techniques** on the **CSIRO Image2Biomass dataset**. Biomass estimation is an important problem in agriculture, ecology, and environmental monitoring, helping researchers understand vegetation productivity and ecosystem health.

The goal of this project was to build predictive models that estimate biomass accurately using vegetation indices, plant measurements, and species information.

---

## 🎯 Objectives
- Perform Exploratory Data Analysis (EDA) on biomass-related variables
- Handle skewed biomass distributions
- Engineer meaningful features from environmental variables
- Train and evaluate machine learning models
- Improve prediction performance using ensemble techniques

---

## 📊 Dataset
The dataset used in this project comes from the **CSIRO Image2Biomass Challenge**.

It contains:

- NDVI (Normalized Difference Vegetation Index)
- Average plant height
- Species information
- Location/state
- Biomass measurements (target variable)

The biomass target variable showed a **highly skewed distribution**, requiring transformation before modeling.

---

## 🔎 Exploratory Data Analysis

Key observations:

- Biomass distribution had **skewness ≈ 1.70**, indicating a strong right skew.
- Applying **log transformation** helped stabilize variance and improve model performance.
- Vegetation indices like **NDVI** and plant height showed strong correlation with biomass.

---

## 🤖 Models Used

Several machine learning models were trained and compared:

- Random Forest Regressor
- Gradient Boosting Models
- XGBoost
- Ensemble Model

Models were evaluated using:

- RMSE (Root Mean Squared Error)
- R² Score

---

## 📈 Results

| Model | RMSE | R² |
|------|------|------|
| Baseline Model | 25.82 | — |
| ML Model | 11.66 | — |
| ML Model | 11.26 | — |
| Gradient Boosting Model | 12.20 | 0.776 |
| **Best Model** | **9.12** | **0.875** |

### Ensemble Model
**Weighted Ensemble RMSE:** 9.21

### Improvement Over Baseline
The final model improved prediction accuracy by approximately **64% compared to the baseline model**.

---

## 💡 Key Insights

- **NDVI** and **plant height** were among the most important predictors of biomass.
- **Log transformation** significantly improved model learning due to skewed biomass values.
- Ensemble learning helped reduce prediction error and improve model stability.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

---

## 📂 Project Structure

```
csiro-biomass-prediction
│
├── csiro-Image2Biomass.ipynb
├── README.md
```

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/yourusername/csiro-biomass-prediction.git
```

Install dependencies:

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
```

Run the notebook to reproduce the analysis.

---

## 📚 Key Learnings

- Handling skewed scientific datasets
- Feature engineering for environmental variables
- Model comparison and evaluation
- Ensemble modeling for improved predictive performance

---

## 👤 Author

**Muhammed Shameel**  
MSc Data Science & Machine Learning Enthusiast

---

## 🔗 Future Improvements

- Hyperparameter tuning
- Feature importance analysis
- Model explainability using SHAP
