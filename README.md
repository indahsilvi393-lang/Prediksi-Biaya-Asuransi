# 🩺 Prediksi Biaya Asuransi Kesehatan

Proyek ini bertujuan untuk **memprediksi biaya klaim asuransi kesehatan** menggunakan beberapa algoritma *Machine Learning* seperti **Linear Regression**, **Ridge Regression**, **Lasso Regression**, dan **XGBoost**.  
Analisis dilakukan untuk memahami pengaruh faktor-faktor seperti **usia, jenis kelamin, kebiasaan merokok, indeks massa tubuh (BMI)**, dan **wilayah tempat tinggal** terhadap biaya klaim.

---

## 🧠 **Tujuan Proyek**
- Memprediksi biaya klaim asuransi dengan akurasi tinggi  
- Mengidentifikasi faktor paling berpengaruh terhadap biaya klaim  
- Membandingkan performa model *Linear*, *Lasso*, *Ridge*, dan *XGBoost Regression*

---

## 🧩 **Dataset**
Dataset yang digunakan berasal dari:
- **Kaggle**: *Medical Cost Personal Dataset*  
- Terdiri dari **1338 baris data** dan **7 fitur utama**, yaitu:
  - Usia (age): Usia penerima manfaat utama.
  - Jenis kelamin (sex) : Jenis kelamin pemegang polis asuransi, bisa perempuan atau laki-laki.
  - BMI (bmi): Indeks massa tubuh, memberikan pemahaman tentang berat badan yang relatif tinggi atau rendah dibandingkan tinggi badan. Ini merupakan indeks obyektif dari berat badan (kg/m²) dengan menggunakan rasio tinggi terhadap berat badan. Idealnya berkisar antara 18,5 hingga 24,9.
  - Jumlah anak (children): Jumlah anak yang ditanggung oleh asuransi kesehatan / jumlah tanggungan.
  - Perokok (smoker): Kebiasaan merokok.
  - Wilayah tempat tinggal (region): Area tempat tinggal penerima manfaat di AS, seperti timur laut (northeast), tenggara (southeast), barat daya (southwest), dan barat laut (northwest).

---

## ⚙️ **Model dan Evaluasi**
Empat model regresi digunakan dalam eksperimen:
- **Linear Regression**
- **Ridge Regression**
- **Lasso Regression**
- **XGBoost Regression**
---

## 🧾 **Overall Results**

| Model              | Train MAE | Test MAE | Train MSE | Test MSE | Train RMSE | Test RMSE | Train R² | Test R² | Training Time (s) |
|--------------------|-----------|----------|------------|-----------|-------------|------------|-----------|----------|-------------------|
| Linear Regression  | 0.787188  | 0.839831 | 0.977548   | 1.052403  | 0.988710    | 1.025867   | 0.913443  | 0.894387 | 0.015742          |
| Ridge Regression   | 0.787840  | 0.836646 | 0.979962   | 1.049878  | 0.989930    | 1.024636   | 0.913229  | 0.894641 | 0.007496          |
| Lasso Regression   | 0.892664  | 0.881224 | 1.225243   | 1.230933  | 1.106907    | 1.109474   | 0.891511  | 0.876471 | 0.002201          |
| XGBoost Regression | 0.039163  | 0.986092 | 0.003113   | 1.529381  | 0.055790    | 1.236681   | 0.999724  | 0.846521 | 0.194125          |

📈 **Kesimpulan:**  
- Model **XGBoost** menunjukkan nilai *Train R²* yang sangat tinggi (0.9997) menandakan overfitting,  
  sementara **Ridge Regression** memiliki performa paling seimbang antara data train dan test.  
- Secara keseluruhan, **Ridge Regression** menjadi model terbaik untuk prediksi biaya asuransi dengan generalisasi yang baik.

---

## 🚀 **Cara Menjalankan**
1. Clone repository:
   ```bash
   git clone https://github.com/indahsilvi393-lang/Prediksi-Biaya-Asuransi.git
