# 🚚 Delivery Time Analysis & Prediction

## 📌 Deskripsi Proyek
Pertumbuhan layanan food delivery meningkatkan ekspektasi pelanggan terhadap kecepatan dan ketepatan pengiriman. Namun, tahap last-mile delivery menjadi bagian paling kompleks dan dapat menyumbang lebih dari 50% biaya logistik.

Keterlambatan pengiriman tidak hanya berdampak pada operasional, tetapi juga secara langsung mempengaruhi kepuasan pelanggan dan performa bisnis.

Proyek ini bertujuan untuk menganalisis faktor-faktor yang memengaruhi delivery time serta membangun model prediksi untuk meningkatkan efisiensi operasional.

---

## 🎯 Tujuan Analisis
- Menganalisis performa delivery saat ini  
- Mengidentifikasi faktor utama yang memengaruhi delivery time  
- Membangun model prediksi waktu pengiriman  
- Memberikan rekomendasi untuk meningkatkan on-time delivery  

---

## 📂 Dataset
- Sumber: Kaggle (Food Delivery Time Prediction Dataset)  
- Jumlah data: 1000 baris, 9 kolom  

**Fitur utama:**
- Distance (km)  
- Delivery Time (target)  
- Traffic Condition  
- Weather  
- Preparation Time  
- Courier Experience  
- Time of Day  
- Vehicle Type  

---

## ⚙️ Proses Analisis

### 1. Data Cleaning
- Menangani 120 missing value:
  - Numerik → median  
  - Kategori → "Unknown"  
- Tidak terdapat data duplikat  

### 2. Handling Outlier
- Outlier hanya pada delivery time (~0.6%)  
- Dipertahankan karena merepresentasikan kondisi nyata  

### 3. Feature Engineering
- Distance Group (Near, Medium, Far)  
- Preparation Time Group (Fast, Normal, Slow)  
- Courier Experience Level (Low, Medium, High)  

### 4. Exploratory Data Analysis (EDA)
- Analisis korelasi antar variabel  
- Identifikasi faktor utama driver delivery time  

### 5. Modeling
- Model terbaik: **Linear Regression**  
- MAE: 6.44  
- RMSE: 10.31  
- MAPE: 10.85%  
- Model cukup akurat dalam memprediksi delivery time  

---

## 📊 Key Insights

### 1. Performa delivery masih belum optimal
- On-time delivery hanya **42%**  
- 58% order mengalami keterlambatan  
- Rata-rata delivery time: **56.73 menit**  

### 2. Jarak adalah faktor paling dominan
- Jarak dekat: ~34 menit  
- Jarak jauh: ~71 menit  
- Delivery time meningkat lebih dari 2x  

### 3. Faktor operasional sangat berpengaruh
- Preparation time: +17 menit  
- Traffic: +12 menit  
- Weather: hingga +14 menit  

### 4. Faktor minor
- Vehicle type & courier experience → pengaruh kecil (2–6 menit)  

---

## 💡 Business Recommendations

### 1. Optimasi proses persiapan pesanan
- Batasi preparation time (≤15 menit)  
- Standarisasi SOP restoran  

### 2. Perbaiki sistem dispatching
- Prioritaskan order jarak jauh  
- Sesuaikan assignment dengan kondisi traffic  

### 3. Implementasi dynamic routing
- Gunakan data real-time traffic & weather  
- Optimalkan rute pengiriman  

### 4. Gunakan model prediksi untuk estimasi delivery
- Estimasi waktu lebih akurat  
- Meningkatkan customer experience  

---

## 🛠 Tools yang Digunakan
- Python (Pandas, Scikit-learn, Matplotlib, Seaborn)  
- Power BI  
- Microsoft Excel  

---

## 📊 Dashboard
Dashboard digunakan untuk:
- Monitoring KPI delivery  
- Analisis faktor keterlambatan  
- Evaluasi performa operasional  
- Visualisasi model prediction  

---

## 📌 Kesimpulan
Analisis menunjukkan bahwa delivery time dipengaruhi secara signifikan oleh jarak, waktu persiapan, dan kondisi lalu lintas. Selain itu, model prediksi yang dibangun mampu memberikan estimasi yang cukup akurat.

Dengan mengoptimalkan faktor operasional utama, perusahaan dapat meningkatkan on-time delivery, mengurangi keterlambatan, dan meningkatkan kepuasan pelanggan.
