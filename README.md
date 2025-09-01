# 🏡 California Housing Price Prediction

## 📖 Deskripsi Project
Project ini bertujuan untuk memprediksi **harga median rumah** di California berdasarkan berbagai faktor sosial, demografi, dan geografis.  
Dataset yang digunakan adalah **California Housing Dataset** dari `scikit-learn`.

## 📊 Deskripsi Dataset
| Kolom       | Deskripsi                                                                 |
|-------------|---------------------------------------------------------------------------|
| MedInc      | Median income rumah tangga (dalam puluhan ribu dolar AS)                  |
| HouseAge    | Usia median rumah di area (tahun)                                         |
| AveRooms    | Rata-rata jumlah ruangan per rumah                                        |
| AveBedrms   | Rata-rata jumlah kamar tidur per rumah                                    |
| Population  | Jumlah penduduk di area                                                   |
| AveOccup    | Rata-rata jumlah penghuni per rumah                                       |
| Latitude    | Lintang geografis area di California                                      |
| Longitude   | Bujur geografis area di California                                        |
| MedHouseVal | Harga median rumah (dalam ratusan ribu dolar AS) → **Target Prediksi**    |

---

## 🧑‍💻 Metodologi
1. **Exploratory Data Analysis (EDA)**
   - Analisis distribusi data
   - Heatmap korelasi antar fitur
2. **Preprocessing**
   - Train-test split
   - Standarisasi (opsional)
3. **Modeling**
   - Linear Regression (baseline)
   - Random Forest Regressor
4. **Evaluasi**
   - R² Score
   - Root Mean Squared Error (RMSE)
5. **Visualisasi**
   - Korelasi antar fitur
   - Feature Importance
   - Scatter plot (Actual vs Predicted)

---

## 📈 Hasil Evaluasi
- **Linear Regression**
  - R² = 0.6411
  - RMSE = 0.1592 (~ \$15,900)
- **Random Forest**
  - R² = 0.8005
  - RMSE = 0.1187 (~ \$11,800)

✅ Random Forest menunjukkan performa lebih baik dibanding Linear Regression, dengan akurasi lebih tinggi dan error lebih rendah.

---

## 📷 Visualisasi
### Heatmap Korelasi
![heatmap](images/heatmap.png)

### Feature Importance (Random Forest)
![feature-importance](images/feature_importance.png)

### Actual vs Predicted
![actual-vs-predicted](images/actual_vs_predicted.png)

---

## ✨ Insight
- **Median Income (MedInc)** adalah faktor paling dominan yang memengaruhi harga rumah.  
- **Latitude & Longitude** juga sangat berpengaruh, menunjukkan lokasi geografis memainkan peran penting.  
- Faktor usia rumah (HouseAge) berpengaruh sedang, sementara variabel lain seperti jumlah ruangan/penduduk relatif kurang signifikan.  
- Model masih kesulitan memprediksi rumah dengan harga ekstrem (outlier).

---

## 📦 Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🚀 Cara Menjalankan
1. Clone repository ini:
   ```bash
   git clone https://github.com/username/california-housing-prediction.git
   cd california-housing-prediction
