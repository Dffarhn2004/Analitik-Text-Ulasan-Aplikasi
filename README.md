# Analitik Teks - Klasifikasi Sentimen Ulasan Aplikasi

Tugas UTS Text Analytics: klasifikasi sentimen (positive/negative) ulasan Google Play untuk Gojek, Shopee, dan Tokopedia (23 Feb - 25 Mar 2026), dengan TF-IDF dan Word2Vec sebagai fitur serta Naive Bayes, Logistic Regression, dan Linear SVM sebagai classifier.

**Penulis:** Muhammad Daffa Raihan (NIM 25917045)

## Isi repositori
| Berkas / folder | Keterangan |
|---|---|
| `Tugas_Klasifikasi_Teks_Ulasan.ipynb` | Notebook utama (Bagian 0-6), sudah dijalankan beserta hasilnya |
| `Laporan_Klasifikasi_Teks_Ulasan.pdf` | Laporan tertulis |
| `data/reviews.csv`, `data/manual_annotation.csv` | Dataset (sumber: Hugging Face `RimuruChan67/indonesian-googleplay-sentiment`) |
| `article/` | Artikel Bagian 0: *Fenomena 'Krisis Ojol' di Bulan Ramadan* (RRI, 14 Maret 2026) |
| `refs/` | Makalah rujukan Bagian 6 |
| `requirements.txt` | Pustaka Python |

## Menjalankan
```bash
pip install -r requirements.txt
jupyter notebook Tugas_Klasifikasi_Teks_Ulasan.ipynb
```
Jalankan dari folder ini (path data relatif). NLTK mengunduh stopwords/punkt otomatis. Stemming Sastrawi membuat eksekusi penuh memakan belasan menit.

## Ringkasan hasil (1.032 data uji, kelas negative)
Accuracy 0,90-0,91 dan F1 0,92-0,93 untuk keempat model; perbedaan antarmodel belum signifikan (uji McNemar, selang kepercayaan bootstrap). Catatan metodologis dan batasan ada di notebook dan laporan.
