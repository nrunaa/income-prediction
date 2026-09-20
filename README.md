# Prediksi Kategori Pendapatan Individu 

Repositori ini berisi proyek *Machine Learning* untuk memprediksi kategori pendapatan individu (apakah `<=50K` atau `>50K`) berdasarkan dataset *Census Income* (KDD)[cite: 9]. Proyek ini merupakan bagian dari pengerjaan tugas di *Study Group*: AI Engineering[cite: 8].

## 💡 Deskripsi Proyek
Tujuan utama dari proyek ini adalah membangun model klasifikasi biner yang mampu memprediksi tingkat pendapatan seseorang berdasarkan karakteristik demografis, pendidikan, okupasi/pekerjaan, dan kondisi finansial[cite: 9]. Evaluasi performa model diukur menggunakan metrik utama **F1-Macro**[cite: 9].

## ⚙️ Alur Kerja (*Pipeline*)
Proses pengerjaan proyek ini meliputi[cite: 9]:
1. **Data Cleaning & EDA**: Penanganan *missing values*, identifikasi duplikat, dan analisis pola/distribusi data seperti usia, jam kerja per minggu, serta *capital-gain*[cite: 8, 9].
2. **Preprocessing**: 
   * Numerik: Imputasi *Median* dan di-skala dengan `StandardScaler`[cite: 9, 10].
   * Kategorikal: Imputasi *Most-Frequent* dan di- *encode* dengan `One-Hot Encoding`[cite: 9, 10].
3. **Eksperimen Model**: Membandingkan tiga algoritma yaitu **Logistic Regression**, **Random Forest**, dan **CatBoost**[cite: 9, 10].

## 🏆 Hasil Evaluasi
Berdasarkan hasil eksperimen, algoritma **CatBoost** (menggunakan fitur original tanpa tambahan *feature engineering* logaritmik) terbukti memberikan performa terbaik dengan skor **F1-Macro sebesar 0.8103**[cite: 9]. Model CatBoost ini kemudian ditetapkan sebagai model final untuk mengenerate hasil prediksi pada data *testing*[cite: 9].

## 📂 Struktur & Penjelasan File
* **`AI Engineering_103012530054_Nahdah Runa Musyaffa_Notebook Machine Learning.ipynb`** : *Source code* lengkap (Python) yang memuat proses eksplorasi data (EDA), *preprocessing*, pembangunan model, hingga evaluasi[cite: 10].
* **`AI Engineering_103012530054_Nahdah Runa Musyaffa_Submission.csv`** : Hasil *generate* prediksi final dari model terbaik terhadap data *testing*[cite: 9].
* **`AI Engineering_103012530054_Nahdah Runa Musyaffa_Laporan.pdf`** : *Technical report* lengkap mengenai penjelasan setiap alur eksperimen *Machine Learning* yang dilakukan[cite: 9].
* **`AI Engineering_103012530054_Nahdah Runa Musyaffa_Bonus Laporan.pdf`** : Analisis mendalam terkait distribusi pendapatan berdasarkan pekerjaan (*occupation*) dan tingkat pendidikan (*education*), beserta rekomendasi strategi untuk SDM perusahaan[cite: 8].

## 👤 Author
* **Nahdah Runa Musyaffa** (103012530054)[cite: 8, 9]
* Universitas Telkom[cite: 9]
