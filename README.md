# 🏠 Estimasi Harga Rumah di Yogyakarta menggunakan Machine Learning

Proyek ini merupakan implementasi **Machine Learning Regression** untuk melakukan estimasi harga rumah di wilayah **Daerah Istimewa Yogyakarta (DIY)** berdasarkan data iklan properti daring.  
Model dibangun menggunakan pendekatan **Random Forest Regressor** dengan preprocessing data dan feature engineering yang berfokus pada karakteristik properti dan lokasi.

---

## 📌 Deskripsi Singkat

Dataset diolah dari data mentah berformat **JSON** yang berisi informasi iklan rumah, seperti:
- Luas bangunan
- Luas tanah
- Jumlah kamar tidur
- Jumlah lantai
- Lokasi (kabupaten & kecamatan)
- Judul iklan properti

Proyek ini secara otomatis **membedakan data jual dan sewa** dengan melakukan analisis teks pada judul iklan (misalnya: *jual*, *sewa*, *disewakan*, dan variasinya).  
Hanya data **jual rumah** yang digunakan untuk pelatihan model prediksi harga.

---

## ✨ Fitur Utama

- Parsing dan pembersihan data properti dari format JSON
- Deteksi otomatis transaksi **jual vs sewa** berbasis teks
- Feature engineering lokasi hingga tingkat **kabupaten dan kecamatan**
- Exploratory Data Analysis (EDA)
- Visualisasi distribusi dan korelasi data
- Implementasi **Random Forest Regressor**
- Transformasi log pada harga untuk mengurangi pengaruh outlier
- Evaluasi model menggunakan:
  - R² Score
  - Mean Absolute Error (MAE)
  - Cross Validation
- Seluruh proses disusun dalam **1-cell Jupyter Notebook** untuk kemudahan eksekusi

---

## 🧠 Metode Machine Learning

- **Model**: Random Forest Regressor  
- **Pendekatan**: Supervised Learning (Regression)
- **Target**: Harga rumah
- **Teknik tambahan**:
  - Log transformation pada harga
  - Encoding fitur kategorikal
  - Train-test split & cross validation

---

## 📂 Struktur Proyek

```text
.
├── notebook.ipynb        
├── data/
│   └── raw_data.json     
└── README.md
