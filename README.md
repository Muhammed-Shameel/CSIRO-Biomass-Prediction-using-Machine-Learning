# 🌿 CSIRO Image2Biomass Prediction

## 📌 Project Overview
This project focuses on predicting **plant biomass** using machine learning models on the **CSIRO Image2Biomass dataset**. Biomass estimation is important for ecological monitoring, agriculture, and understanding vegetation productivity.

The objective of this project was to analyze biomass-related variables and build regression models capable of accurately predicting biomass values.

---

## 🎯 Objectives
- Perform exploratory data analysis (EDA) on biomass data
- Investigate distribution of the biomass target variable
- Train regression models using different loss functions
- Compare model performance
- Improve predictions using an ensemble approach

---

## 📊 Dataset
The dataset comes from the **CSIRO Image2Biomass challenge** and includes environmental and plant-related variables.

Key variables include:

- NDVI (Normalized Difference Vegetation Index)
- Average plant height
- Species information
- Location/state
- Biomass measurements (target variable)

The biomass variable showed **positive skew**, which was explored during analysis.

---

## 🔎 Exploratory Data Analysis

Key observations:

- Biomass values were **right-skewed**, meaning larger biomass values were less frequent.
- Vegetation-related variables such as **NDVI and plant height** showed relationships with biomass.
- Data visualization helped understand the relationship between **true vs predicted biomass values**.

---

## 🤖 Models Implemented

The following regression models were implemented:

- **MSE Model** (regression optimized using Mean Squared Error)
- **Huber Model** (robust regression less sensitive to outliers)
- **LogCosh Model** (smooth loss function similar to MSE but more robust)

### Ensemble Model
A **weighted ensemble model** was created by combining predictions from the individual models to improve stability and prediction accuracy.

---

## 📈 Model Evaluation

Model predictions were evaluated using:

- Root Mean Squared Error (**RMSE**)
- Prediction error distribution
- Visual comparison of **true vs predicted biomass**

### Observations

- The **ensemble model produced predictions closest to the ideal diagonal line** in the True vs Predicted plot.
- Error distribution plots showed most prediction errors **centered around zero**, indicating reasonable predictive performance.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn


## 📚 Key Learnings

- Understanding biomass prediction problems
- Exploring skewed environmental datasets
- Comparing regression models using different loss functions
- Improving predictions using ensemble modeling

---

## 👤 Author

**Muhammed Shameel**  
MSc Data Science & Machine Learning Enthusiast

