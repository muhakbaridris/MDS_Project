# 🧴 MDS: Manajemen Data Statistika - Scraping Penjualan Parfum Tokopedia

## 📌 Deskripsi Proyek

Proyek ini merupakan bagian dari inisiatif *Manajemen Data Statistika* (MDS) yang berfokus pada pengumpulan, penyimpanan, dan analisis data dari platform e-commerce. Pada studi kasus ini, kami melakukan scraping data penjualan **parfum** dari Tokopedia pada **empat toko populer**:

Brand parfum best seller berdasarkan peringkat dari website Markethac
<img width="896" alt="Image" src="https://github.com/user-attachments/assets/1c35c33f-9b79-4ea1-bb02-508b6cdeef3d" />

- HMNS  
- Mykonos  
- Octarine  
- SAFF & Co

Pemilihan kategori *parfum* didasarkan pada tingginya **rating pengguna** dan jumlah **produk terjual** yang menandakan popularitas dan permintaan pasar yang tinggi.

## 🎯 Tujuan

- Mengimplementasikan teknik web scraping secara etis untuk mengumpulkan data dari Tokopedia.
- Mengelola data hasil scraping menggunakan database non-relasional (MongoDB) dan menyimpannya secara cloud melalui MongoDB Atlas.
- Menganalisis produk-produk terlaris dan berperingkat tertinggi di antara 4 toko parfum tersebut.
- Menyusun **Top 5 Produk Terlaris** secara keseluruhan sebagai hasil akhir.

## 🧰 Tools & Teknologi

| Tools             | Keterangan                                                                 |
|-------------------|----------------------------------------------------------------------------|
| **Python**        | Bahasa pemrograman utama untuk scraping dan analisis data.                 |
| **MongoDB**       | Database NoSQL untuk menyimpan data hasil scraping.                        |
| **MongoDB Atlas** | Cloud database service dari MongoDB untuk penyimpanan online.             |
| **BeautifulSoup / Selenium / Requests** | Digunakan untuk mengambil dan memproses data HTML dari Tokopedia. |

## 🗂️ Struktur Proyek

    
    📁 mds-parfum-scraper/
    ├── 📁 data/                 # Dataset mentah & bersih
    ├── 📁 src/                  # Kode scraping & utilitas
    │   ├── scraper.py          # Fungsi scraping per toko
    │   └── database.py         # Koneksi MongoDB Atlas
    ├── 📁 analysis/             # Notebook eksplorasi dan analisis
    │   └── top5_analysis.ipynb # Analisis Top 5 produk terlaris
    ├── requirements.txt        # Daftar pustaka Python
    └── README.md               # Dokumentasi proyek


## 📊 Hasil Utama

- Dataset berisi data produk seperti: nama produk, harga, rating, total terjual, dan tautan produk.
- Penyimpanan data real-time di MongoDB Atlas.
- Visualisasi produk-produk parfum terlaris di antara keempat toko.
- Menyusun **Top 5 Produk Parfum Terlaris** berdasarkan penjualan tertinggi.
  
Top 5 Rekomendasi
  <img width="896" alt="Image" src="https://github.com/user-attachments/assets/9f2fdc87-d3ff-41d6-a23d-abcab1b69489" />
  
Top 5 Budget For 200k
  <img width="889" alt="Image" src="https://github.com/user-attachments/assets/26da5417-06b9-4ba2-bf1e-609a630b89ee" />

Top 5 Budget For 100k
  <img width="896" alt="Image" src="https://github.com/user-attachments/assets/9f2fdc87-d3ff-41d6-a23d-abcab1b69489" />

## 🛡️ Etika Scraping

Kami memastikan scraping dilakukan dengan mempertimbangkan:
- Tidak membanjiri server (dengan delay / sleep).
- Tidak mengakses data di balik autentikasi atau yang dilindungi hak akses.
- Hanya mengambil data publik.

## 🚀 Cara Menjalankan Proyek

1. **Clone repositori ini**
   ```bash
   git clone https://github.com/username/mds-parfum-scraper.git
   cd mds-parfum-scraper

2. **Install dependensi**
   ```bash
   pip install -r requirements.txt

3. **Atur koneksi MongoDB Atlas di file .env**
    ```bash
    MONGO_URI=mongodb+srv://<username>:<password>@<cluster>.mongodb.net

4. **Jalankan scraper**
   ```bash
   python src/scraper.py

5. **Lakukan analisis data**
Buka file Jupyter Notebook di folder analysis/ dan jalankan top5_analysis.ipynb

## 📌 Catatan Tambahan
Jika ingin menambahkan toko atau kategori lain, cukup ubah parameter scraping pada scraper.py.

Proyek ini dapat dikembangkan lebih lanjut untuk visualisasi interaktif menggunakan Streamlit atau Dash.

## 📈 Data Scraping Analysis

Berikut merupakan link RPubs data scraping analysis:  
📎 **[Data Scraping and Visualization](https://colab.research.google.com/drive/1id2nHpYixufnqX_CooeHArZ75Ds1mKdb?usp=sharing))**

---

## 📚 PPT

Berikut adalah link powerpoint berkaitan dengan project yang telah dibuat:  
📎 **[PPT Data Scraping and Visualization](https://github.com/muhakbaridris/MDS_Project/blob/d41d64cf8b61273e09b7d3ae2ee83d2095318b00/Presentation.pdf)**

---

## 🧑‍💻 Kontributor
<img width="764" alt="Image" src="https://github.com/user-attachments/assets/c0100ae7-27af-46f7-8e95-c8b3ed3b446e" />
