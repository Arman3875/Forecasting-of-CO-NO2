# Time-Series Forecasting of Carbon Monoxide and Nitrogen Dioxide Levels

## 📌 Project Overview
This project focuses on forecasting the levels of Carbon Monoxide (CO) and Nitrogen Dioxide (NO₂) using time-series modeling. The goal is to develop LSTM models that can predict pollutant levels based on historical data and environmental factors.

## 📂 Dataset Overview
### 📄 Dataset Description
The dataset includes hourly air pollution data with the following key attributes:
- `CO(GT)`: Carbon Monoxide concentration
- `NO₂(GT)`: Nitrogen Dioxide concentration
- `T`: Temperature
- `RH`: Relative Humidity
- `AH`: Absolute Humidity
- Timestamp features: Hour, Day of the week, Month

### 🎯 Objective
- Perform **Exploratory Data Analysis (EDA)** to understand patterns and trends.
- Engineer features to improve model performance.
- Build **LSTM models** for CO(GT) and NO₂(GT) prediction.
- Evaluate models and derive actionable insights.

---
## ⚙️ Feature Engineering
### ✅ Key Features Created
- **Lag Features:** Incorporate historical values of `CO(GT)` and `NO₂(GT)`.
- **Time-Based Features:** Extract `hour of the day`, `day of the week`, and `month`.
- **Environmental Factors:** Include `T`, `RH`, and `AH` as predictors.

---
## 🏗 Steps to Build LSTM Models for CO(GT) and NO₂(GT)
### **Step 1: Import Libraries**
- Import necessary libraries for data processing, visualization, and modeling.

### **Step 2: Data Preparation**
- Handle missing values and outliers.
- Normalize the data for better model performance.

### **Step 3: Create Time Series Data**
- Generate sequences for training and testing.
- Define a function to create sequences for LSTM.
- Create separate sequences for CO(GT) and NO₂(GT).
- Reshape inputs to fit LSTM requirements.

### **Step 4: Train-Test Split**
- Split data into training and testing sets.
- Separate splits for CO(GT) and NO₂(GT).

### **Step 5: Build LSTM Models**
- **For CO(GT):**
  - Define and train an LSTM model.
- **For NO₂(GT):**
  - Define and train an LSTM model.

### **Step 6: Evaluate Models**
- Plot training and validation loss for each model.
- Assess performance using RMSE and MAE.

### **Step 7: Make Predictions**
- Predict pollutant levels on test data.
- Inverse transform predictions to original scale.
- Plot predictions vs. actual values.

---
![image](https://github.com/user-attachments/assets/55170e2f-c5d9-415b-bb53-0fbab20447aa)

![image](https://github.com/user-attachments/assets/7d54a80c-35d3-428d-aae0-d3b0d36c15fb)

### **Random Forest Model Performance**
| Metric  | Value |
|---------|-------------|
| **MAE**  | 2.7380 |
| **RMSE** | 3.2156 |
| **R² Score** | -0.6818 |

---


## 📌 Actionable Recommendations Based on Predicted Trends
### **Steps:**
Based on forecasted trends and seasonal patterns, we suggest the following actions:

### **For Policymakers:**
- Implement **traffic restrictions** during peak pollution hours to reduce CO(GT) levels.
- Strengthen **industrial emissions regulations** during winter months to control NO₂(GT).

### **For the Public:**
- Avoid outdoor activities during peak pollution hours.
- Use masks or air purifiers in high-pollution periods.

### **For City Planners:**
- Increase **green spaces** in high-pollution areas.
- Optimize **traffic flow** to reduce congestion-related emissions.

---
## 📌 Future Work
🔹 **Enhance Feature Engineering:** Explore additional environmental and meteorological factors.
🔹 **Improve Model Performance:** Experiment with hybrid models like CNN-LSTM.
🔹 **Deploy Model:** Create a real-time air pollution forecasting system.

---
## 🚀 How to Run This Project
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/air-quality-forecast.git
   cd air-quality-forecast
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Train the LSTM models:
   ```bash
   python train_lstm.py
   ```
4. Evaluate the models:
   ```bash
   python evaluate.py
   ```

---
## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
## 📩 Contact
📧 **Your Name** - armanhossainiueee@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/arman-hossain-1413991a4/)  
🔗 [GitHub](https://github.com/Arman3875)  

---
> **Note:** This project is a learning exercise in time-series forecasting using deep learning techniques.
