# 📊 PCA & MDS Visualization from Scratch on Iris Dataset

## Identitas Mahasiswa  
**Nama:** Thalita Zahra Sutejo  
**NIM:** 18222023  
**Kelas:** 01 - Data Analytics (K01)

## 📌 Deskripsi Singkat  
Tugas ini merupakan implementasi dan analisis dua teknik *dimensionality reduction* — **Principal Component Analysis (PCA)** dan **Multidimensional Scaling (MDS)** — secara manual (*from scratch*) pada dataset klasik **Iris**. Proses dilakukan secara bertahap mulai dari *data cleaning*, *preprocessing*, perhitungan manual PCA dan MDS, hingga visualisasi serta analisis hasil proyeksi dua dimensi dari kedua metode.


## 🧰 Tools dan Bahasa Pemrograman  
- **Python** (Jupyter Notebook)  
- **Library:**  
  - `pandas` untuk manipulasi data  
  - `numpy` untuk perhitungan numerik  
  - `matplotlib` & `seaborn` untuk visualisasi  
  - `scipy.spatial.distance` untuk menghitung matriks jarak pada MDS  
  - `sklearn.preprocessing.StandardScaler` untuk standardisasi fitur  

## 🔎 Tahapan Implementasi

### 1. Data Cleaning & Preprocessing
- Memisahkan fitur numerik dan label kategorikal
- Memeriksa dan menghapus data duplikat (3 baris)
- Validasi tipe data dan label
- Deteksi outlier dengan visualisasi boxplot
- Standardisasi fitur numerik menggunakan *z-score normalization*

### 2. Implementasi PCA (From Scratch)
- Menghitung rata-rata tiap fitur
- Membentuk matriks kovarians
- Dekomposisi eigen untuk mendapatkan *principal components*
- Memilih dua komponen utama untuk proyeksi 2D
- Visualisasi hasil proyeksi PCA

### 3. Implementasi MDS (From Scratch)
- Menghitung jarak Euclidean antar sampel
- Membentuk *distance matrix* dan *Gram matrix* melalui *double centering*
- Dekomposisi eigen terhadap Gram matrix
- Proyeksi ke dalam dua dimensi
- Visualisasi hasil proyeksi MDS

### 4. Analisis Hasil Visualisasi
- Interpretasi hasil proyeksi PCA dan MDS
- Perbandingan keterpisahan kelas, interpretabilitas dimensi, serta kelebihan dan keterbatasan metode
- Refleksi terhadap kesamaan hasil visualisasi kedua metode


## 📈 Hasil Utama
- PCA dan MDS sama-sama berhasil memisahkan kelas **Iris-setosa** secara jelas.
- **Iris-versicolor** dan **Iris-virginica** menunjukkan tumpang tindih pada kedua metode.
- Hasil visualisasi kedua metode tampak sangat mirip, karena data Iris memiliki struktur linier dan variansi yang sejalan dengan jarak antar titik.
- PCA unggul dalam efisiensi dan interpretasi dimensi, sedangkan MDS menonjol dalam pelestarian jarak antar data.


## 🧠 Refleksi  
Melalui implementasi dari nol, diperoleh pemahaman yang lebih dalam tentang cara kerja internal PCA dan MDS. Proyek ini menekankan pentingnya pemilihan teknik reduksi dimensi berdasarkan struktur data dan tujuan eksplorasi. Kombinasi keduanya memberikan sudut pandang yang saling melengkapi dalam memahami data berdimensi tinggi.
