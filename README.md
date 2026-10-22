# uts-machine-learning-241011401716

# UTS Machine Learning - Linear Regression & Logistic Regression

Repositori ini berisi penyelesaian Tugas Tengah Semester (UTS) mata kuliah **Machine Learning** yang mengimplementasikan algoritma **Linear Regression** dan **Logistic Regression** secara mandiri (*from scratch*) menggunakan library NumPy, Pandas, dan Matplotlib.

---

## Identitas Mahasiswa

- **Nama**  : [Nama Lengkap Anda]
- **NIM**   : 241011401716
- **Kelas** : Reg B / Reg C *(pilih salah satu)*
- **Random State** : 16 *(diambil dari 2 digit terakhir NIM)*

---

## Ringkasan Hasil Model & Evaluasi

### Bagian A – Linear Regression (Prediksi Penjualan Berdasarkan Biaya Iklan)

- **Dataset**: `Ads_Data.csv` (40 sampel)
- **Pembagian Data**: Train (80% / 32 baris), Test (20% / 8 baris)
- **Persamaan Regresi**: $\hat{y} = 15.3408 + 6.1362 \times X$

| Metrik Evaluasi | Data Training | Data Testing |
|---|---|---|
| **MAE** | 4.6710 | 5.6872 |
| **MSE** | 33.6469 | 46.0270 |
| **RMSE** | 5.8006 | 6.7843 |
| **$R^2$ Score** | **0.9466** | **0.9161** |

> **Kesimpulan**: Model memiliki performa yang sangat baik dengan $R^2$ sebesar **0.9161** pada data testing, yang berarti 91.61% variasi penjualan dapat dijelaskan oleh biaya iklan.

---

### Bagian B – Logistic Regression (Klasifikasi Email Spam)

- **Dataset**: `Email_Data.csv` (60 sampel)
- **Pembagian Data**: Train (75% / 45 baris), Test (25% / 15 baris)
- **Learning Rate**: 0.1 | **Iterasi**: 10,000

| Metrik Evaluasi (Threshold = 0.5) | Nilai |
|---|---|
| **Accuracy** | **86.67%** (0.8667) |
| **Precision** | **88.89%** (0.8889) |
| **Recall** | **88.89%** (0.8889) |
| **F1-Score** | **88.89%** (0.8889) |

---

## Struktur Repositori

```text
uts-machine-learning-241011401716/
├── README.md            # Dokumentasi & ringkasan hasil UTS
├── tugas_UTS.ipynb      # Jupyter Notebook lengkap dengan kode & output
├── Ads_Data.csv         # Dataset biaya iklan & penjualan
└── Email_Data.csv       # Dataset fitur email & label spam
