# UTS-Graf-Sains-Data
UTS Graf Sains Data - Analisis Graf dan Sistem Rekomendasi KNN

# UTS Graf Sains Data

## Deskripsi
Repository ini berisi pengerjaan UTS mata kuliah Graf Sains Data, meliputi pemodelan graf interaksi pengguna dan item, pembentukan Vector Space Model (VSM), analisis kemiripan item menggunakan Cosine Similarity, penyimpanan relasi pada Neo4j, serta evaluasi sistem rekomendasi menggunakan K-Nearest Neighbors (KNN).

## Dataset
Dataset yang digunakan adalah data interaksi e-commerce Retailrocket yang dibagi menjadi:
- `retailrocket_train_new.csv`: data training P1.
- `retailrocket_test_new.csv`: data testing P2.

Kolom utama meliputi timestamp, visitorid, event, itemid, dan transactionid.

## Isi Repository
- `UTS_Graf_Sains_Data.ipynb`: kode Python, output, visualisasi, dan penjelasan analisis.
- `retailrocket_train_new.csv`: dataset training.
- `retailrocket_test_new.csv`: dataset testing.

## Metode
1. Membentuk dan menganalisis graf bipartit Visitor–Item.
2. Membandingkan VSM User dan VSM Item.
3. Menghitung Cosine Similarity antaritem.
4. Menyimpan dan memverifikasi relasi SIMILAR_TO di Neo4j.
5. Membuat rekomendasi item menggunakan KNN dengan k = 5.
6. Mengevaluasi rekomendasi menggunakan Hit@5 dan NDCG@5.

## Hasil Evaluasi
Pada eksperimen untuk visitor yang dipilih, nilai Hit@5 dan NDCG@5 adalah 0,0000. Tidak ada item rekomendasi teratas yang cocok dengan item aktual pada periode testing.

## Cara Menjalankan
Buka notebook menggunakan Jupyter Notebook atau JupyterLab. Pastikan dependensi Python sudah terpasang dan sesuaikan lokasi dataset serta konfigurasi koneksi Neo4j sebelum menjalankan sel yang memerlukannya.
