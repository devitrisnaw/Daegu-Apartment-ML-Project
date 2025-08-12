# 🏢 Daegu Apartment

Proyek ini menganalisis harga apartemen di Daegu, Korea Selatan, menggunakan Machine Learning.  
Analisis meliputi data cleaning, preprocessing, pemodelan dengan berbagai algoritma, evaluasi performa, hingga penentuan faktor-faktor yang paling berpengaruh terhadap harga.

## 1. Business Problem Understanding
Apartemen di Daegu memiliki variasi harga yang signifikan. Penjual memiliki kebebasan penuh menentukan harga, namun risiko salah harga cukup tinggi:
- Terlalu mahal → sulit laku.
- Terlalu murah → rugi.

**Tantangan:** Menentukan harga jual yang tepat agar tetap kompetitif sekaligus menguntungkan.

## 2. Goals
1. Menentukan model prediksi harga apartemen dengan akurasi tinggi.
2. Mengidentifikasi faktor-faktor yang memengaruhi harga.
3. Memberikan rekomendasi strategi harga untuk pengembang dan penjual.

## 3. Analytics Approach
1. Data Understanding & EDA
2. Data Preprocessing
3. Modeling (Linear Regression, KNN, Decision Tree, Random Forest, XGBoost, Gradient Boosting)
Algorithm: Gradient Boosting (with hyperparameter tuning)
Used 5-fold cross-validation
4. Evaluasi Model : RMSE, MAE, MAPE
5. Feature Importance
6. Rekomendasi Bisnis

## 4. Dataset Overview
Dataset berisi informasi unit apartemen di Daegu, termasuk:
- **SalePrice** → Harga jual apartemen (target variabel).
- **YearBuilt** → Tahun pembangunan apartemen.
- **HallwayType** → Tipe desain koridor (*terraced*, *corridor*, *mixed*).
- **SubwayStation** → Stasiun subway terdekat.
- **DistanceToSubway** → Jarak ke stasiun subway (meter).
- **Area** → Luas bangunan (m²).
- **N_Facilities** → Jumlah fasilitas lingkungan sekitar.
- Variabel fasilitas lainnya (parkir, keamanan, taman, dll).

## 5. Conclusion
- Gradient Boosting dan XGBoost menjadi model terbaik dengan RMSE & MAE terendah.
- Faktor terpenting: luas bangunan, jarak ke stasiun subway, dan tahun pembangunan.

## 6. Recommendation
- Analisis Error – identifikasi 5% prediksi dengan error terbesar untuk menemukan pola dan melakukan feature engineering tambahan.
- Penambahan Fitur Relevan – seperti kondisi interior, kualitas bangunan, pemandangan, kedekatan pusat komersial, data demografi, dan tren harga wilayah.
- Eksperimen Model Lanjutan – uji LightGBM, CatBoost, stacking, atau deep learning jika dataset lebih besar.
- Perbarui model secara berkala dengan data terbaru untuk menjaga akurasi.
