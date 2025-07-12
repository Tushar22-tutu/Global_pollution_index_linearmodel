# 🌍 Global Pollution Analysis and Energy Recovery

## 🎯 Objective
The objective is to analyze global pollution data and build models to both:
- Predict **energy recovery** from pollution levels using **regression**, and
- Classify countries into pollution categories (Low, Medium, High) using **classification**.

---

## 📊 Phase 1: Data Collection and Exploratory Data Analysis (EDA)

### 🔹 Step 1 - Data Import and Preprocessing
- Load dataset: `Global_Pollution_Analysis.csv`
- Handle missing values using suitable imputation techniques (mean, median, forward fill, etc.)
- Encode categorical features like `Country`, `Year` using Label Encoding or One-Hot Encoding
- Normalize pollution indices:
  - `Air_Pollution_Index`
  - `Water_Pollution_Index`
  - `Soil_Pollution_Index`

### 🔹 Step 2 - Exploratory Data Analysis (EDA)
- Compute **descriptive statistics** for key variables like `CO2_Emissions` and `Industrial_Waste_in_tons`
- Generate a **correlation heatmap** to explore relationships between pollution and energy recovery
- Use bar plots, line plots, and box plots to:
  - Track pollution trends by year and country
  - Visualize energy recovery potential across regions

### 🔹 Step 3 - Feature Engineering
- Extract **year-wise trends** for pollutants and energy production
- Calculate **Energy Consumption per Capita** using population and energy data
- Combine multiple pollution indices into a composite pollution severity score

---

## 🔧 Phase 2: Predictive Modeling

### ✅ Step 4 - Linear Regression Model (Energy Recovery Prediction)
- **Goal**: Predict `Energy_Recovery_GWh` using features such as:
  - `Air_Pollution_Index`
  - `CO2_Emissions`
  - `Industrial_Waste_in_tons`
- **Model**: Linear Regression
- **Evaluation Metrics**:
  - R² (coefficient of determination)
  - Mean Squared Error (MSE)
  - Mean Absolute Error (MAE)

### ✅ Step 5 - Logistic Regression Model (Pollution Classification)
- **Goal**: Classify countries into pollution severity classes: Low, Medium, High
- **Model**: Logistic Regression
- **Input Features**: `Air_Pollution_Index`, `CO2_Emissions`, `Industrial_Waste_in_tons`, etc.
- **Evaluation Metrics**:
  - Accuracy
  - Precision, Recall
  - F1-Score
  - Confusion Matrix

---

## 📌 Summary
This project provides a comprehensive approach to understanding pollution severity and its impact on energy recovery. Using **regression** for prediction and **logistic classification** for categorization, this model can aid in global policy-making, environmental monitoring, and sustainable energy planning.

📈 Future extensions could include:
- Deployment via Flask for real-time forecasting
- Integrating satellite and real-time IoT sensor data
- Comparative analysis with ensemble learning methods
