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
