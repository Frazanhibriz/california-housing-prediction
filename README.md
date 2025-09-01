# 🏡 California Housing Price Prediction

## 📖 Project Overview
This project aims to predict the **median house value** in California based on socio-economic, demographic, and geographic factors.  
The dataset used is the **California Housing Dataset** provided by `scikit-learn`.

---

## 📊 Dataset Description
| Column       | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| MedInc       | Median income of households (in tens of thousands of US dollars)            |
| HouseAge     | Median age of houses in the area (years)                                    |
| AveRooms     | Average number of rooms per house                                           |
| AveBedrms    | Average number of bedrooms per house                                        |
| Population   | Total population of the area                                                |
| AveOccup     | Average number of occupants per household                                   |
| Latitude     | Latitude of the area                                                        |
| Longitude    | Longitude of the area                                                       |
| MedHouseVal  | Median house value (in hundreds of thousands of US dollars) → **Target**    |

---

## 🛠️ Workflow
1. **Data Loading**
   - Load the dataset from `scikit-learn` into a pandas DataFrame.
   
2. **Exploratory Data Analysis (EDA)**
   - Descriptive statistics and distribution analysis
   - Correlation heatmap between features

3. **Data Preprocessing**
   - Splitting data into training and testing sets
   - Feature scaling (optional)

4. **Modeling**
   - **Linear Regression** → used as the baseline model
   - **Random Forest Regressor** → ensemble method to capture non-linear relationships

5. **Model Evaluation**
   - Metrics: R² Score, Root Mean Squared Error (RMSE)
   - Compare baseline (Linear Regression) with Random Forest

6. **Visualization**
   - Heatmap of feature correlations
   - Feature importance (Random Forest)
   - Scatter plot of Actual vs Predicted values

---

## 📈 Results
- **Linear Regression**
  - R² = 0.6411
  - RMSE = 0.1592 (~ \$15,900)

- **Random Forest**
  - R² = 0.8006
  - RMSE = 0.1187 (~ \$11,800)

✅ The Random Forest model outperforms Linear Regression, achieving higher accuracy and lower error.

---

## 📷 Visualizations
### Correlation Heatmap
![heatmap](images/heatmap.png)

### Feature Importance (Random Forest)
![feature-importance](images/feature_importance.png)

### Actual vs Predicted
![actual-vs-predicted](images/actual_vs_predicted.png)

---

## ✨ Insights
- **Median Income (MedInc)** is the most influential factor in determining house prices.  
- **Latitude & Longitude** play a significant role, reflecting the importance of geographical location.  
- **HouseAge** has a moderate impact, while features like `AveRooms`, `AveBedrms`, and `Population` contribute less.  
- The model struggles slightly with extreme outliers but performs well overall.  

---

## 📦 Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Frazanhibriz/california-housing-prediction.git
   cd california-housing-prediction
