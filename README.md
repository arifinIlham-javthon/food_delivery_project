# Food Delivery Data Cleaning & EDA

Projek ini adalah simulasi *pipeline* Data Science untuk membersihkan dan menganalisis dataset operasi aplikasi *Food Delivery* lokal. Dataset sengaja dipilih karena memiliki tingkat *kekotoran* data yang tinggi (missing values, oulier ekstrem, dan format tanggal campur aduk).

## Tujuan Projek
1. Melakukan *Data Cleaning* (Handling Missing Values & Outlier).
2. Melakukan *Feature Engineering* (Ektraksi waktu * kategori).
3. Menarik *insight* bisnis menggunakan agregasi Pandas dan visualisasi data.

## Tech Stack
- **Python** (Pandas, Numpy)
- **Visualisasi** (Matplotlib, Seaborn)
- **Environment** (Jupyter Notebook / VS Code)

## Insight Utama
1. **Waktu Tunggu vs Jarak:** Terdapat korelasi positif kuat (0.75) antara jarak kirim dengan tunggu. Semakin jauh, semakin lama.
2. **Promo tidak selalu memperlambat:** Pesanan dengan promo (`True`) tidak selalu memiliki waktu tunggu yang lebih lama dibanding tanpa promo, menandakan sistem *load balanching* berjalan baik.
3. **Outlier Harga:** Ditemukan harga ekstrem hingga Rp 8 juta yang harus difilter menggunakan metode IQR agar tidak merusak rata-rata.

## Sumber Data
Dataset diperoleh dari [Hugging Face - Zaky/Food-Delivery-Dataset](huggingface.co/datasets/ZakyF/Food-Delivery-Dataset).
*Catatan: File CSV tidak-diapload ke repo ini karena ukurannya. Silahkan unduh dari link di atas dan letakkan di folder `data/`.*

---
*Created by [arifinIlham-javthon]*