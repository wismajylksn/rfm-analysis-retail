# 🛒 Retail Customer Segmentation: RFM Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

**Oleh:** Wisma Jaya Laksana  
**Lihat Postingan LinkedIn:** [Link Postingan LinkedIn Kamu]

## 📌 Project Overview
Project ini bertujuan untuk membantu bisnis retail online memahami perilaku pelanggan mereka secara mendalam. Saya menggunakan metode **RFM (Recency, Frequency, Monetary)** untuk mengelompokkan pelanggan ke dalam berbagai segmen strategis. 

Tujuan utama analisis ini adalah menjawab pertanyaan bisnis kritis: 
> *"Siapa pelanggan paling berharga kita, dan siapa pelanggan yang sudah mulai meninggalkan toko kita?"*

## 🛠️ Tech Stack & Tools
- **Python:** Data Cleaning, Feature Engineering, & RFM Scoring logic (Library: `pandas`, `matplotlib`, `seaborn`, `squarify`).
- **Tableau:** Interactive Dashboard & Data Storytelling (File `.twbx` tersedia di repository ini).

## 🧮 Metodologi (The Flow)
1. **Data Cleaning:** - Menghapus data transaksi tanpa `CustomerID`.
   - Menghapus anomali data (transaksi dengan `Quantity` atau `UnitPrice` bernilai negatif yang mengindikasikan retur barang).
2. **Feature Engineering:** Membuat kolom `TotalPrice` sebagai representasi nilai omzet tiap transaksi.
3. **RFM Calculation:**
   - **Recency (R):** Jarak hari dari transaksi terakhir ke tanggal analisis.
   - **Frequency (F):** Total jumlah transaksi unik per pelanggan.
   - **Monetary (M):** Total uang yang dihabiskan oleh pelanggan.
4. **Scoring & Segmentation:** Menggunakan pendekatan statistik (Kuantil) untuk memberikan skor 1-5 pada setiap metrik, kemudian memetakannya ke dalam 10 segmen pelanggan (misal: *Champions, Loyal Customers, Hibernating, dll*).

## 📊 Key Business Insights
Berdasarkan visualisasi data yang telah dibuat:
1. **Mayoritas Pelanggan Berada di Segmen "Hibernating" (1.049 pelanggan):** Sebagian besar basis pelanggan adalah orang-orang yang dulu pernah berbelanja, namun sudah lama sekali tidak kembali.
2. **Hukum Pareto Berlaku (The Power of Champions):** Meskipun pelanggan berstatus **"Champions"** dan **"Loyal Customers"** secara kuantitas lebih sedikit (~606 & 827 orang), namun **kedua segmen inilah yang menyumbang mayoritas total omzet (Revenue)** bagi perusahaan (Mencapai > 4 Juta).

## 💡 Rekomendasi Actionable
- **Pertahankan yang Setia:** Fokuskan budget *loyalty program*, layanan VIP, atau diskon eksklusif untuk memanjakan segmen *Champions* agar mereka tidak direbut kompetitor.
- **Reaktivasi Pelanggan Tidur:** Kirimkan *email marketing* atau promo *win-back* (diskon besar bersyarat) khusus untuk sebagian pelanggan *Hibernating* yang masih memiliki potensi aktif kembali.

## 📂 Cara Menjalankan Project Ini
1. Clone repository ini: `git clone https://github.com/wismajylksn/rfm-analysis-retail.git`
2. Buka notebook `latihan-rfm-wisma.ipynb` untuk melihat detail tahapan *coding* Python.
3. Download file `ds-rfm.twbx` dan buka menggunakan **Tableau Desktop / Tableau Public** untuk berinteraksi langsung dengan dashboard.

---
*End-to-end Data Analytics Project - 2026*
