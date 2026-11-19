# Text Summarization untuk Tugas Akhir Mata kuliah NLP

Proyek Tugas Akhir mata kuliah Pemrosesan Bahasa Alami (NLP), Kelompok 2A.
Membandingkan pendekatan **extractive** dan **abstractive** untuk meringkas artikel WikiHow berbahasa Indonesia.

## Structure Project

```
text-summarize-nlp/
├── notebooks/   .ipynb per job (Google Colab)
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_extractive.ipynb
│   ├── 03_abstractive.ipynb
│   └── 04_evaluation.ipynb
├── src/         all code
├── results/     hasil prediksi setiap proses
├── report/      draf laporan akhir
├── README.md
└── .gitignore
```

## Pembagian Job

| Peran | Tugas | Anggota | Branch |
|---|---|---|---|
| 1. Data & Preprocessing | EDA, pembersihan, split data | [Andita Tifanny] | `data` |
| 2. Extractive | TF-IDF, TextRank, LSA | [Ali Fikri] | `extractive` |
| 3. Abstractive | LSTM + attention, model pretrained | [Waffiq Muchlishin] | `abstractive` |
| 4. Evaluasi & Laporan | ROUGE, analisis error, laporan | [Taharo Hafwenia] | `evaluation` |

## Deskripsi Dataset

- **Nama:** WikiLingua (`esdurmus/wiki_lingua` di Hugging Face)
- **Config data yang dipakai:** `indonesian` (16.308 artikel dataset)
- **Sumber:** artikel WikiHow
- **Struktur:** setiap artikel terdiri dari beberapa bagian dan tiap bagian memiliki `section_name`, `document` (teks), dan `summary` (ringkasan)
- **Tautan:** https://huggingface.co/datasets/esdurmus/wiki_lingua
- **Lisensi:** kartu dataset mencantumkan CC BY 3.0 sekaligus merujuk CC BY-NC-SA 3.0.

