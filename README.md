# 🛍️ Analisis Sentimen Pengguna pada Aplikasi Shopee

Proyek ini bertujuan untuk menganalisis sentimen pengguna dari ulasan yang diberikan pada aplikasi Shopee. Sentimen diklasifikasikan ke dalam tiga kategori utama: **positif**, **negatif**, dan **netral**.

## 📌 Tujuan

Mengekstrak insight dari ulasan pengguna dengan pendekatan analisis sentimen untuk mengetahui bagaimana perasaan pengguna terhadap layanan di aplikasi Shopee.

## 🧰 Metode

- **Metode Pelabelan:** *Inset Lexicon*
- **Model yang Digunakan:**
  - Deep Learning (TF-IDF)
  - Support Vector Machine / SVM (TF-IDF)
  - Decision Tree (CountVectorizer)

## 🧪 Tahapan Proyek

1. **Scraping Data**  
   Mengambil data ulasan pengguna dari sumber online.

2. **Preprocessing**  
   Melakukan pembersihan data teks melalui beberapa tahapan seperti:
   - Cleaning
   - Case Folding
   - Normalisasi
   - Tokenizing
   - Stopword Removal
   - Stemming

3. **Pelabelan Data**  
   Data diberi label menggunakan metode *lexicon-based* dengan referensi dari Inset Lexicon.

4. **Pemodelan**  
   Data dilatih dan diuji menggunakan beberapa algoritma untuk membandingkan performa.

5. **Evaluasi Model**  
   Model dievaluasi menggunakan metrik akurasi, precision, recall, dan f1-score.

6. **Pengujian Data Baru**  
   Model yang telah dibangun digunakan untuk mengklasifikasikan ulasan baru.

## 📈 Hasil Evaluasi

| Model            | Akurasi | Keterangan                                                             |
|------------------|---------|------------------------------------------------------------------------|
| Deep Learning     | 94%     | Sangat baik untuk kelas positif & netral; negatif sedikit lebih rendah |
| SVM               | 92%     | Positif sangat akurat; negatif lebih rendah                            |
| Decision Tree     | 86%     | Negatif kurang baik (recall 59%)                                       |

## 📎 Tools & Library

- Python
- Scikit-learn
- TensorFlow / Keras
- NLTK
- Pandas & NumPy
- Matplotlib / Seaborn
- RapidMiner (untuk visualisasi dan model pembanding)

