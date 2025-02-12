# 🚴‍♂️ Bike Sharing Demand - Kaggle Competition  

This project is part of the **[Bike Sharing Demand Kaggle Competition](https://www.kaggle.com/competitions/bike-sharing-demand)**. The goal is to build a machine learning model to predict the number of bike rentals based on factors such as **weather conditions, time, and working days**.

---

## 📊 Dataset Overview  
The dataset comes from a bike-sharing system and includes hourly rental data along with time-based and weather-related features.  

### **🔹 Features:**  
- `datetime` - Timestamp (year, month, day, hour)  
- `season` - Season (1 = Spring, 2 = Summer, 3 = Fall, 4 = Winter)  
- `holiday` - Whether the day is a holiday (1 = Yes, 0 = No)  
- `workingday` - Whether the day is a working day (1 = Yes, 0 = No)  
- `weather` - Weather condition (1 = Clear, 4 = Heavy Rain/Snow)  
- `temp` - Temperature in Celsius  
- `atemp` - Feels-like temperature  
- `humidity` - Humidity level  
- `windspeed` - Wind speed  
- `casual` - Number of casual (non-registered) riders  
- `registered` - Number of registered riders  
- `count` - **Total bike rentals (Target variable)**  

📌 **Competition Link:** [Kaggle - Bike Sharing Demand](https://www.kaggle.com/competitions/bike-sharing-demand)  

---

## ⚡ Approach  
1️⃣ **Exploratory Data Analysis (EDA):**  
- Analyzed data distributions and relationships.  
- Found that most rentals occur on working days and in good weather conditions.  

2️⃣ **Feature Engineering:**  
- Extracted `hour`, `weekday`, and `year` from `datetime`.  
- Created new time-based features to improve model performance.  

3️⃣ **Model Training:**  
- Tested **AutoGluon** for automated hyperparameter tuning.  
- Compared different models and optimized hyperparameters.  

4️⃣ **Evaluation & Submission:**  
- Used **Root Mean Squared Error (RMSE)** as the evaluation metric.  
- Submitted the best predictions to Kaggle.  

---

## 🚀 Results  
- **Baseline RMSE:** -32  
- **After Feature Engineering:** Improved RMSE  
- **After Hyperparameter Tuning:** Kaggle score improved from 47 to **44**  

---

## 🛠️ How to Run the Project  
1️⃣ Clone the repository:  
```bash
git clone https://github.com/yourusername/bike-sharing-demand.git
cd bike-sharing-demand
