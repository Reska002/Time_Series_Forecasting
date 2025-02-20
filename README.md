# **Prediksi Harga Saham ISAT.JK dengan Time Series Forecasting**

Created by:
- Hafizh
- Dhika
- Iqbal
- Bryan
- Reska

### **Context**

**Indosat Ooredoo Hutchison (ISAT.JK)** adalah salah satu perusahaan telekomunikasi terbesar di Indonesia yang sahamnya diperdagangkan di **Bursa Efek Indonesia (BEI)**. Harga saham **ISAT.JK** dipengaruhi oleh berbagai faktor, seperti **kinerja perusahaan**, **kondisi makroekonomi**, **persaingan industri**, **sentimen pasar**, dan **peristiwa global**. Sebagai instrumen investasi yang volatil, **prediksi pergerakan harga saham ISAT.JK** menjadi krusial bagi investor, analis keuangan, dan pemangku kepentingan untuk mengambil keputusan yang informatif, baik dalam hal pembelian, penjualan, maupun strategi portofolio.

### **Problem Statement**

Meskipun data historis harga saham **ISAT.JK** tersedia, ketidakpastian pergerakan harga akibat dinamika pasar yang kompleks membuat prediksi jangka pendek maupun menengah menjadi sulit. **Tantangan utama** meliputi:  
1. **Volatilitas tinggi**: Fluktuasi harga harian yang dipengaruhi sentimen pasar dan faktor eksternal.  
2. **Ketergantungan pada faktor multidimensi**: Harga saham tidak hanya bergantung pada data historis, tetapi juga indikator ekonomi, kinerja perusahaan, dan berita industri.  
3. **Kebutuhan akan keputusan real-time**: Investor membutuhkan prediksi akurat untuk meminimalkan risiko dan memaksimalkan keuntungan.  

Tanpa model *forecasting* yang andal, keputusan investasi berisiko menjadi **suboptimal** atau bahkan merugikan.  

### **Goals** 

1. **Mengembangkan model time series forecasting** untuk memprediksi harga penutupan (*closing price*) saham **ISAT.JK** dalam jangka waktu tertentu (misalnya, 7-30 hari ke depan).  
2. **Menganalisis pola historis** dan faktor-faktor yang signifikan memengaruhi pergerakan harga saham.  
3. **Mengevaluasi performa model** untuk memastikan akurasi dan keandalan prediksi.  
4. **Memberikan rekomendasi strategis** berdasarkan hasil prediksi kepada investor atau pihak terkait.

### **Analytic Approach**  

1. **Data Collection**: 
   - Mengumpulkan data historis harga saham **ISAT.JK** (*open*, *close*, *high*, *low*, volume perdagangan) dari sumber tepercaya.  

2. **Understanding and Preprocessing**:  
   - Menganalisa tren dari data
   - Pembagian data dengan *time-based splitting*.
3. **Model Development**:  
   - Membandingkan algoritma seperti **ARIMA**, **SARIMA**, atau **Prophet**.  
   - Menguji kombinasi fitur teknis (harga historis).  
5. **Interpretasi Hasil**: 
   - Analisis residual, identifikasi pola error, dan optimasi *hyperparameter*.

### **Metric Evaluation**

**Metrik evaluasi utama**:  
1. **MAE (Mean Absolute Error)**: Mengukur rata-rata kesalahan absolut prediksi.  
2. **RMSE (Root Mean Squared Error)**: Memberikan bobot lebih tinggi pada kesalahan besar.  
3. **MAPE (Mean Absolute Percentage Error)**: Menilai persentase kesalahan relatif terhadap harga aktual.  
4. **R-squared (R²)**: Mengevaluasi seberapa baik variasi data dijelaskan oleh model.  

**Kriteria Sukses**:  
- Model dianggap baik jika **MAPE < 5%** pada data uji.  
- Prediksi harus konsisten mengikuti **tren aktual**, termasuk dalam kondisi pasar volatil.  
- Model harus mengungguli **baseline** (contoh: prediksi naive menggunakan harga hari sebelumnya).

## **Data Understanding**

Permasalahan di atas akan dianalisis menggunakan dataset yang berisi data historis harga saham **ISAT.JK**. Dataset ini diambil dari **Yahoo Finance**, sebuah platform terpercaya yang menyediakan data keuangan dan pasar saham. Dataset ini dapat diakses melalui link berikut: [Download Dataset ISAT.JK](https://finance.yahoo.com/quote/ISAT.JK/history?p=ISAT.JK). 

### **Power Point**

https://www.canva.com/design/DAGeS6yB3Rk/iVCTC0fsTp6zO7clGUUE8Q/edit?utm_content=DAGeS6yB3Rk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
