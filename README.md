# Prediksi-Biaya-Asuransi
Analisis biaya klaim asuransi kesehatan menggunakan Linear Regression dan turunannya (Lasso, Ridge).
# 🩺 Prediksi Biaya Asuransi Kesehatan

Proyek ini bertujuan untuk **memprediksi biaya klaim asuransi kesehatan** menggunakan algoritma *Linear Regression*, *Lasso Regression*, dan *Ridge Regression*.  
Analisis dilakukan untuk memahami pengaruh faktor-faktor seperti **usia, jenis kelamin, kebiasaan merokok, indeks massa tubuh (BMI)**, dan **wilayah tempat tinggal** terhadap biaya klaim.

---

## 📊 **Tampilan Hasil**
Berikut salah satu hasil visualisasi dari model yang dikembangkan:

![Dashboard Asuransi](https://raw.githubusercontent.com/USERNAME/Prediksi-Biaya-Asuransi/main/dashboard.png)

*(Gambar di atas bisa kamu ganti dengan nama file gambar kamu sendiri, misalnya `visualisasi.png`)*

---

## 🧠 **Tujuan Proyek**
- Memprediksi biaya klaim asuransi dengan tingkat akurasi tinggi  
- Mengidentifikasi faktor paling berpengaruh terhadap biaya klaim  
- Membandingkan performa model *Linear*, *Lasso*, dan *Ridge Regression*

---

## 🧩 **Dataset**
Dataset yang digunakan berasal dari:
- **Kaggle**: *Medical Cost Personal Dataset*
- Terdiri dari **1338 baris data** dan **7 fitur utama**

---

## ⚙️ **Model yang Digunakan**
| Model | Mean Squared Error (MSE) | R² Score |
|-------|---------------------------|-----------|
| Linear Regression | 37,000 | 0.75 |
| Lasso Regression  | 38,100 | 0.73 |
| Ridge Regression  | 36,500 | 0.76 |

---

## 🚀 **Cara Menjalankan**
1. Clone repository:
   ```bash
   git clone https://github.com/USERNAME/Prediksi-Biaya-Asuransi.git
