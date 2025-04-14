# Analisa Sentimen Reviews Aplikasi Tiktok Playstore

## Struktur Folder

```
Analisa-Sentimen-Reviews-TikTok/
├── data/
│   ├── slang.json           # Daftar kata slang yang digunakan dalam analisis sentimen
│   └── tiktok_reviews.csv   # Dataset review TikTok yang diambil dari Playstore
├── model/
│   ├── model_logreg.pkl     # Model Logistic Regression yang telah dilatih
│   ├── model_LSTM.h5        # Model LSTM yang telah dilatih
│   ├── model_SVM.pkl        # Model SVM yang telah dilatih
│   ├── tfidf_vectorizer.pkl # Model TF-IDF untuk ekstraksi fitur
│   └── tokenizer.pkl        # Tokenizer untuk model LSTM
├── inference.ipynb          # Notebook untuk melakukan inferensi pada model
├── requirements.txt         # Daftar dependencies
├── scraping_tiktok.ipynb    # Notebook untuk scraping
└── sentimen_tiktok.ipynb    # Notebook untuk pelatihan, evaluasi, dan eksperimen model
```

## Penilaian


## Penilaian

Untuk proyek ini, berikut adalah kriteria yang harus dipenuhi:

| Kriteria                               | Deskripsi                                                                                                                                                  | Status |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| **Penggunaan Algoritma Deep Learning** | Model yang digunakan harus berbasis **Deep Learning**.                                                                                                     | ✅      |
| **Akurasi Model**                      | **Akurasi** pada **training set** dan **testing set** harus lebih dari **92%**.                                                                            | ✅      |
| **Dataset**                            | Dataset harus memiliki **minimal tiga kelas** untuk sentimen dan **minimal 10.000 sampel data**.                                                           | ✅      |
| **Skema Pelatihan**                    | Melakukan **minimal 3 percobaan skema pelatihan** yang berbeda, dengan variasi algoritma pelatihan, metode ekstraksi fitur, pelabelan, dan pembagian data. | ✅      |
| **Inferensi**                          | Lakukan inferensi atau testing menggunakan file `.ipynb` atau `.py`. Output harus berupa **kelas kategorikal** (contoh: Negatif, Netral, Positif).         | ✅      |
| **Bukti Inferensi**                    | Sertakan bukti inferensi dalam bentuk **screenshot** atau **output** yang terdapat pada notebook yang digunakan untuk inferensi.                           | ✅      |

### Skema Pelatihan

Berikut adalah **3 percobaan skema pelatihan** dengan variasi yang berbeda:

| Percobaan       | Pelatihan            | Ekstraksi Fitur                      | Pembagian Data |
| --------------- | -------------------- | ------------------------------------ | -------------- |
| **Percobaan 1** | LSTM                 | Tokenizer + Padding + Word Embedding | 80/10/10       |
| **Percobaan 2** | LOGISTIC REGRESSION  | TF-IDF                               | 80/20          |
| **Percobaan 3** | SUPER VECTOR MACHINE | TF-IDF                               | 80/20          |

### Catatan:
- Jika **akurasi testing set** tidak lebih dari 92%, pastikan **semua percobaan** memiliki **akurasi minimal 85%** pada testing set.
- Jika Anda mencoba lebih dari tiga skema pelatihan, pastikan **setidaknya satu percobaan** memiliki akurasi **lebih dari 92%** pada **training set** dan **testing set**, dan sisanya memiliki **akurasi di atas 85%**.

<!-- ## Tidak Sesuai Kriteria


Jika submission Anda **tidak memenuhi kriteria** berikut, maka akan **ditolak** oleh reviewer. Pastikan untuk mematuhi semua poin berikut agar submission Anda diterima.

| Kriteria                                                  | Deskripsi                                                                                                                  | Status |
| --------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- | ------ |
| **Tidak Melampirkan Kode dan Proses Data Scraping**       | Pastikan Anda melampirkan kode untuk proses scraping data dari Playstore.                                                  | [ ]    |
| **Akurasi Model di Bawah 85%**                            | Akurasi model Anda harus **lebih dari 85%** pada testing set. Jika di bawah itu, submission akan ditolak.                  | [ ]    |
| **Tidak Melampirkan 4 File Kriteria Utama**               | Pastikan Anda melampirkan keempat file kriteria utama sesuai dengan ketentuan pada tab "Ketentuan Berkas Submission".      | [ ]    |
| **Menggunakan Data yang Sudah Tersedia pada Open Source** | Data yang digunakan dalam proyek Anda harus **dapatkan secara legal dan bukan data yang sudah tersedia pada open source**. | [ ]    |

### Catatan:
- **Kode dan Proses Scraping**: Harus ada skrip untuk scraping data (misalnya, `scraping_tiktok.ipynb`).
- **Akurasi Model**: Jika akurasi model di bawah 85%, submission Anda tidak akan diterima.
- **4 File Kriteria Utama**: Pastikan Anda melampirkan file yang sesuai, seperti model yang dilatih, skrip pelatihan, dan notebook inferensi.
- **Sumber Data**: Gunakan data yang dapat diambil atau dikumpulkan secara sah, bukan yang sudah ada di repository atau sumber terbuka tanpa izin. -->


