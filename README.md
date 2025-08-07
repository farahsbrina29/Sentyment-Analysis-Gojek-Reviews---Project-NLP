#  Analisis Sentimen Review Gojek

Proyek ini merupakan analisis sentimen terhadap ulasan pengguna aplikasi **Gojek**. Tujuan dari proyek ini adalah untuk mengklasifikasikan ulasan menjadi **positif** atau **negatif** menggunakan pendekatan **TF-IDF** dan algoritma klasifikasi sederhana.

---


##  Tools dan Library

- Python
- NLTK
- Sastrawi
- Scikit-learn
- Matplotlib / Seaborn
- Wordcloud

---

##  Alur Proses

### 1. Pelabelan Sentimen

- Ulasan diberi label berdasarkan skor:
  - **Positif (1)** jika skor tinggi
  - **Negatif (0)** jika skor rendah

---

### 2. Preprocessing Teks

Langkah-langkah preprocessing yang dilakukan:

- **Tokenisasi**: menggunakan `RegexpTokenizer` dan `word_tokenize` dari NLTK
- **Stopword Removal**: menghapus kata-kata umum yang tidak penting
- **Stemming**: menggunakan library **Sastrawi** untuk mengubah kata ke bentuk dasar
- **Cleaning**:
  - Menghapus kata-kata dengan lebih dari 4 huruf (jika diperlukan)
  - Menghapus simbol dan karakter tidak relevan

---

### 3. Visualisasi WordCloud

- Word cloud dibuat untuk memvisualisasikan kata-kata yang sering muncul dalam:
  - Ulasan **positif**
  - Ulasan **negatif**

---

### 4. Vektorisasi Teks

- Menggunakan **TF-IDF Vectorizer** dari Scikit-learn untuk mengubah teks ke bentuk numerik.

---

### 5. Split Data

- Data dibagi menjadi **training set** dan **testing set** menggunakan `train_test_split`.

---

### 6. Evaluasi Model

Model dievaluasi menggunakan beberapa metrik:

- ✅ **Confusion Matrix**
- 📈 **ROC Curve**
- 📊 **Recall Curve**
- 🎯 **F1 Score**

---

## 📌 Hasil & Kesimpulan

- Model mampu memprediksi sentimen dengan hasil yang cukup baik berdasarkan metrik evaluasi.
- Analisis ini dapat digunakan untuk memantau kepuasan pengguna terhadap layanan Gojek secara otomatis.
