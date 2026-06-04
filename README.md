# Sales-Forecasting-Indonesia-AI
Sales forecasting merupakan proses penting dalam dunia bisnis karena membantu perusahaan memprediksi jumlah penjualan di masa mendatang berdasarkan data historis. Prediksi yang akurat memungkinkan perusahaan mengoptimalkan persediaan, merencanakan produksi, mengelola anggaran, serta mengambil keputusan bisnis yang lebih efektif

## 📌 Deskripsi
Proyek ini mengembangkan sistem Sales Forecasting berbasis machine learning dan deep learning untuk memprediksi penjualan pada periode mendatang berdasarkan data historis. Fokus utama proyek adalah membangun pipeline forecasting yang lengkap, mulai dari Exploratory Data Analysis (EDA), analisis tren dan seasonality, feature engineering, preprocessing data time series, hingga pelatihan dan evaluasi model menggunakan ARIMA, SARIMAX, LSTM-Bidirectional, LSTM-GRU dan LSTM lainnya

## 🎯 Tujuan Proyek

Proyek ini bertujuan untuk mengembangkan dan membandingkan beberapa model forecasting guna memprediksi penjualan pada periode mendatang. Dataset yang digunakan berisi data penjualan historis beserta variabel pendukung yang berpotensi memengaruhi penjualan, seperti aktivitas promosi dan faktor eksternal lainnya. Sebelum proses pemodelan, dilakukan Exploratory Data Analysis (EDA) untuk memahami pola data, tren, serta komponen musiman (seasonality) yang terdapat dalam penjualan.

## 🔧 Tahapan Utama

- 📊 EDA (Exploratory Data Analysis) — analisis tren penjualan, seasonality, distribusi data, serta korelasi antar variabel.
- 🛠️ Feature Engineering — pembuatan fitur time series seperti lag features, moving average.
- 📈 Time Series Analysis — uji stasioneritas, dekomposisi tren dan musiman, serta analisis ACF dan PACF.
- 🤖 Modeling — implementasi model ARIMA, SARIMAX, LSTM-Bidirectional, dan LSTM-GRU serta lainnya untuk prediksi penjualan.
- ⚙️ Hyperparameter Tuning — optimasi parameter model statistik dan deep learning untuk meningkatkan akurasi prediksi.
- 📏 Evaluation — evaluasi performa model menggunakan MAPE dan RMSE serta perbandingan hasil forecasting antar model.
- 📉 Forecasting & Visualization — visualisasi hasil prediksi dan perbandingan antara nilai aktual dan hasil forecast.

## 📄 Dataset

- 55572 rows
- 5 columns
- 1 Feature Target Sale Price

## 📊 Model Performance

| No | Model | MAPE (%) ↓ | RMSE ↓ |
|:--:|--------|-----------:|--------:|
| 1 | ARIMA (9,1,5) | 12.438 | 1,892.1781 |
| 2 | SARIMAX (9,1,5)(0,0,1,7) | 11.758 | 1,766.2590 |
| 3 | LSTM-Bidirectional | 11.670 | 1,690.6464 |
| 4 | **🔥 LSTM-GRU** | **10.688** | **1,566.7059** |

### 🏆 Best Model: LSTM-GRU

- ✅ **MAPE terendah:** 10.688%
- ✅ **RMSE terendah:** 1,566.7059
- ✅ Mampu menangkap pola non-linear dan dependensi jangka panjang dengan lebih baik dibanding model lainnya.
- ✅ Direkomendasikan untuk implementasi **Sales Forecasting** pada data penjualan dengan pola tren dan seasonality yang kompleks.

### 📈 Ranking Model

🥇 **LSTM-GRU**  
🥈 **LSTM-Bidirectional**  
🥉 **SARIMAX (9,1,5)(0,0,1,7)**  
🏅 **ARIMA (9,1,5)**

> **Note:** Semakin kecil nilai MAPE dan RMSE, semakin baik performa model dalam melakukan prediksi penjualan.
- 
### 🔍 Insight

- 🚀 LSTM-GRU memberikan performa terbaik dengan nilai MAPE dan RMSE terendah, sehingga menghasilkan prediksi penjualan yang paling akurat.
- 📈 Model deep learning (LSTM-GRU dan LSTM-Bidirectional) mampu menangkap pola non-linear dan dependensi jangka panjang lebih baik dibandingkan model statistik tradisional.
- 🔄 SARIMAX mengungguli ARIMA karena mampu memanfaatkan informasi musiman dan variabel eksternal untuk meningkatkan akurasi prediksi.
- 📊 ARIMA menjadi baseline yang baik, namun memiliki keterbatasan dalam menangkap kompleksitas pola penjualan dibandingkan model yang lebih modern.
- 🎯 Hasil menunjukkan bahwa pendekatan deep learning lebih efektif untuk sales forecasting pada dataset dengan pola tren dan seasonality yang kompleks.

## 🛠 Library yang Digunakan
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Statsmodels, TensorFlow/Keras, ARIMA, SARIMAX, LSTM, dan GRU.

## 🚀 Cara Menjalankan
- Upload dataset ke environment (Google Colab / lokal)
- Pastikan path dataset sesuai:

