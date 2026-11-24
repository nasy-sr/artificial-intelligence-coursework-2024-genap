# Artificial Intelligence - Semester 2 (2024/2025 Genap)

Kumpulan tugas praktikum dan implementasi algoritma mata kuliah *Artificial Intelligence* menggunakan Python.

- *Kelas:* 2A
- *Periode Akademik:* 2024/2025 Genap
- *Bahasa / Tools:* Python, Google Colab

## Daftar Tugas & Eksperimen

| No | File | Topik / Algoritma | Ringkasan |
| :--- | :--- | :--- | :--- |
| 01 | `01_bfs_river_crossing_puzzle.ipynb` | Breadth-First Search (BFS) & State-Space Search | Menyelesaikan *river-crossing puzzle* (robot, fox, chicken, grain) untuk menemukan jalur transisi valid terpendek (7 langkah transisi). |
| 02 | `02-sms-spam-classification-naive-bayes.ipynb` | Text Classification & Multinomial Naive Bayes | Klasifikasi pesan SMS *ham* vs *spam* menggunakan *TF-IDF Vectorizer* dan *Multinomial Naive Bayes* (akurasi **96,68%** pada data uji). |
| 03 | `03-multi-class-text-classification-20-newsgroups.ipynb` | Multi-Class Text Classification & Multinomial Naive Bayes | Klasifikasi teks multi-kelas (20 kategori topik *20 Newsgroups*) dengan *CountVectorizer*, *spaCy tokenizer*, dan *Multinomial Naive Bayes* (akurasi **0,59** / F1 *macro* **0,56**). |
| 04 | `04-multi-class-text-classification-spacy-tokenizer.ipynb` | Multi-Class Text Classification, spaCy Tokenizer & Multinomial Naive Bayes | Klasifikasi teks multi-kelas (20 kategori *20 Newsgroups*, 11.096 data) menggunakan *CountVectorizer*, *custom tokenizer* spaCy, dan *Multinomial Naive Bayes* (akurasi **0,60** / F1 *macro* **0,58**), dilengkapi eksperimen *lemmatization* dengan model `en_core_web_lg`. |
| 05 | `05-uts-gender-classification-nb-knn.ipynb` | Gaussian Naive Bayes & K-Nearest Neighbors (KNN) | Eksplorasi data, visualisasi korelasi, dan klasifikasi dataset `gender_classification.csv` menggunakan Naive Bayes dan KNN beserta evaluasi akurasi dan *confusion matrix*. |
| 06 | `06-knn-classification-iris-dataset.ipynb` | K-Nearest Neighbors (KNN) & StandardScaler | Klasifikasi multi-kelas dataset *Iris* (`iris.csv`) dengan *feature scaling* (`StandardScaler`), evaluasi nilai $k$ (`1, 3, 5, 7, 9`) melalui *confusion matrix* dan *classification report* (akurasi **0,97**–**1,00**), serta visualisasi akurasi vs $k$. |
| 07 | `07_uas_heart_disease_classification_nb_knn.ipynb` | Heart Disease Prediction (Naive Bayes vs. KNN) | Klasifikasi biner risiko penyakit jantung pada *dataset* UCI Cleveland menggunakan rasio *split* 60:40, 70:30, dan 80:20; Naive Bayes unggul dengan akurasi tertinggi 0.9167 pada *split* 80:20. |


## Proyek Evaluasi (UTS & UAS)

### 1. Proyek UTS — Gender Classification (Naive Bayes vs. KNN)
* **Notebook:** [`uts_gender_classification_nb_knn.ipynb`](./uts_gender_classification_nb_knn.ipynb)
* **Dataset:** `gender_classification.csv` (analisis statistik deskriptif, eksplorasi fitur, dan pembagian data latih/uji dengan `train_test_split`).
* **Algoritma & Evaluasi:** Mengimplementasikan dan membandingkan model **Gaussian Naive Bayes** (`GaussianNB`) dan **K-Nearest Neighbors** (`KNeighborsClassifier`), dievaluasi menggunakan **Accuracy**, **Classification Report** (Precision, Recall, F1-Score), serta **Confusion Matrix**.

### 2. Proyek UAS — Heart Disease Prediction (Naive Bayes vs. KNN)
* **Notebook:** [`uas_heart_disease_classification_nb_knn.ipynb`](./uas_heart_disease_classification_nb_knn.ipynb)
* **Dataset:** [UCI Machine Learning Repository — Heart Disease Dataset](https://archive.ics.uci.edu/dataset/45/heart+disease) (subset Cleveland Clinic Foundation, 303 sampel awal, 14 fitur; target `num` diubah menjadi biner `0` dan `1`).
* **Pra-pemrosesan:** Menghapus nilai hilang (`?`) dengan `dropna()`, serta menormalisasi fitur dengan `StandardScaler` untuk model KNN.
* **Evaluasi & Hasil:** Membandingkan **Naive Bayes** dan **KNN** pada rasio *split* **60:40**, **70:30**, dan **80:20** memakai metrik **Akurasi**, **Sensitivitas**, **Spesifisitas**, dan **Kappa**. **Naive Bayes** konsisten unggul di seluruh rasio *split*, dengan akurasi terbaik **0.9167** dan spesifisitas **0.9722** pada rasio **80:20** (dibanding KNN **0.8333** pada rasio yang sama).
