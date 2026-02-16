# Analisis Sentimen Review Aplikasi Shopee di Google Play Store

Proyek ini menganalisis persepsi pengguna terhadap aplikasi Shopee berdasarkan review di Google Play Store. Notebook Jupyter digunakan untuk membersihkan teks ulasan, menormalkan ragam bahasa informal, dan menyiapkan data untuk tahap klasifikasi sentimen.

![Python](https://img.shields.io/badge/Python-3.12%2B-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Status](https://img.shields.io/badge/Status-In%20Progress-success)

## Ruang Lingkup

- Mengimpor dan menyiapkan review aplikasi Shopee dari Google Play Store ke dalam dataset terstruktur
- Membersihkan teks dari emoji, URL, mention, karakter non alfabet, dan kata gaul
- Menyusun pipeline awal untuk evaluasi sentimen (positif, netral, negatif)
- Menyediakan dasar bagi eksplorasi lebih lanjut seperti fitur TF-IDF dan model klasifikasi

## Teknologi

- Python 3 (virtual environment lokal atau Conda)
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn
- NLTK, Sastrawi, WordCloud

## Struktur Folder

```text
Sentimen Analisis Youtube/
├── projeck/
│   ├── [0] Pra Premprosesan data.ipynb.ipynb
│   ├── [1] Text Cleaning.ipynb
│   ├── [2] Pembuatan Model.ipynb
│   ├── hasil_pelabelan.csv
│   └── shopee_review.csv (dataset arsip)
└── env/
```

## Menjalankan Notebook

1. Clone repositori kemudian masuk ke direktori proyek
2. Aktivasi environment:
   - `source env/Scripts/activate` (Git Bash)
   - `.\env\\Scripts\\Activate.ps1` (PowerShell)
   - `conda activate sentimen-shopee` (jika memakai Conda)
3. Pasang dependensi tambahan bila perlu: `pip install -r requirements.txt` (opsional) atau instal manual (pandas, numpy, matplotlib, seaborn, nltk, wordcloud, sastrawi)
4. Jalankan Jupyter Notebook: `jupyter notebook`
5. Buka notebook sesuai urutan numerik untuk menjaga konsistensi pipeline

## Pipeline Notebook

1. **[0] Pra Premprosesan data.ipynb.ipynb**
   - Memuat review mentah aplikasi Shopee
   - Membersihkan kolom non-informatif dan menangani nilai kosong
2. **[1] Text Cleaning.ipynb**
   - Case folding
   - Penghapusan emoji, tautan, simbol khusus
   - Normalisasi slang dengan kamus kustom dan stopword filtering
   - Tokenisasi serta rekonstruksi kalimat bersih
3. **[2] Pembuatan Model.ipynb**
   - (Work in progress) menyiapkan fitur tekstual dari review dan baseline klasifikasi sentimen

## Rencana Lanjutan

- Menyelesaikan notebook modeling dan menambahkan metrik evaluasi
- Membuat visualisasi distribusi sentimen dan word cloud spesifik polaritas
- Mengemas pipeline ke dalam modul Python untuk eksekusi batch
- Mendesain README tambahan untuk dokumentasi eksperimen dan laporan akhir

## Kontribusi

Kontribusi dipersilakan. Buka issue untuk diskusi atau ajukan pull request dengan penjelasan perubahan.

## Lisensi

Proyek ini menggunakan lisensi **MIT**.

Lihat detail pada file `LICENSE`.

---

Jika proyek ini membantu, silakan bintangi repositori sebagai dukungan.