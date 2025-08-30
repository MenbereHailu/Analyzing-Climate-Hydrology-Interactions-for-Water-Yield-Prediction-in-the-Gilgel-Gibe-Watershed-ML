# 🌊 Evaluating Water Yield and the Combined Effects of Climate and Hydrology on the Gilgel Gibe Watershed with Machine Learning Models  

## 📖 Introduction  
The **Gilgel Gibe Watershed**, located in Western Ethiopia, is a critical area for water resource management due to its important role in regional hydrology and agriculture. Analyzing water yield in this watershed requires a comprehensive understanding of both **climatic and hydrological factors**.  

In this study, four advanced machine learning techniques were employed to model and predict water yield:  
- 🌲 **Random Forest (RF)**  
- 📈 **Support Vector Machine (SVM)**  
- ⚡ **Extreme Gradient Boosting (XGB)**  
- 💡 **Light Gradient Boosting Machine (LGBM)**  

These models were used to assess the **synergistic impacts of climate and hydrology** on the watershed.  

---

## ⚙️ Methodology  

### 1. Data Collection and Preprocessing  
- **Climate Data (1993–2023):** Precipitation, temperature, solar radiation, wind speed.  
- **Hydrological Data (1993–2023):** Daily streamflow, runoff measurements, and discharge values.  

### 2. Machine Learning Models  
- **Random Forest (RF):** Ensemble of decision trees, effective for non-linear relationships.  
- **Support Vector Machine (SVM):** Finds optimal hyperplane for classification/regression; handles high-dimensional data.  
- **Extreme Gradient Boosting (XGB):** Sequential boosting with regularization for improved performance.  
- **Light Gradient Boosting Machine (LGBM):** Histogram-based gradient boosting, highly efficient on large datasets.  

### 3. Model Training and Testing  
- **Dataset Split:**  
  - Training: January 1995 – December 2019 (90%)  
  - Testing: January 2020 – December 2023 (10%)  
- **Input Features:** Daily mean, daily flow (m³), max/min discharge, runoff (m³).  
- **Output:** Mean daily discharge.  

### 4. Performance Evaluation  
Models were evaluated using:  
- 📊 Root Mean Square Error (**RMSE**)  
- 📉 Mean Absolute Error (**MAE**)  
- 📈 Coefficient of Determination (**R²**)  
- 🌍 Nash–Sutcliffe Efficiency (**NSE**)  
- ✅ Willmott’s Index of Agreement (**d**)  

---

## 📊 Results  

### 1. Model Performance  
- **Random Forest (RF):**  
  - Training: MAE = 0.38, RMSE = 0.61, R² = 0.76, NSE = 0.76, d = 0.93  
  - Testing: Slight improvements, confirming strong generalization.  
  - ✅ Best performance among all models.  

- **Support Vector Machine (SVM):**  
  - Moderate performance; strong with high-dimensional data, weaker in capturing water yield dynamics compared to RF.  

- **Extreme Gradient Boosting (XGB):**  
  - Training R² = 0.72, Testing R² = 0.80.  
  - Good correlation but slightly lower accuracy than RF.  

- **LightGBM:**  
  - Similar performance to XGB with slight metric variations.  
  - Very efficient for large datasets.  

### 2. Synergistic Impact of Climate and Hydrology  
- **Climate Impact:** Precipitation and temperature strongly affect water yield. RF and XGB captured these effects best.  
- **Hydrological Impact:** Daily flow and runoff significantly influence yield and interact synergistically with climate variables.  

---

## 💡 Discussion  
The integration of machine learning allowed for a **detailed analysis of water yield dynamics** in the Gilgel Gibe Watershed.  

- RF was the **most accurate**, capturing complex non-linear climate–hydrology interactions.  
- XGB and LGBM performed well, especially in explaining variance in discharge values.  
- SVM was effective for high-dimensional data but less accurate overall.  

📌 The findings highlight the **importance of combining both climatic and hydrological factors** in predictive models to ensure reliable water resource forecasting.  

---

## ✅ Conclusion  
This study demonstrates the **effectiveness of advanced machine learning models** in analyzing water yield and understanding the complex interactions between climate and hydrology in the Gilgel Gibe Watershed.  

**Key Contributions:**  
- RF, XGB, and LGBM provide **robust and reliable predictions** of water yield.  
- Results support **better water resource management** and policy planning.  
- Provides a **framework for future studies** in similar hydro-climatic regions.  

---
