# 🏨 Hotel Business Intelligence Dashboard

![Dashboard Preview](screenshots/dashboard_main.png)
*(Pastikan kamu mengupload screenshot dashboard utama ke folder 'screenshots' dan ganti nama filenya di sini)*

## 📌 Gambaran Proyek (Project Overview)
Proyek ini bertujuan untuk menganalisis kinerja operasional dan pendapatan sebuah hotel menggunakan data historis pemesanan (booking). Dashboard ini dibuat menggunakan **Power BI** untuk membantu manajemen hotel dalam memantau tren pendapatan, tingkat pembatalan (cancellation rate), serta efisiensi penggunaan kamar.

Analisis ini menjawab pertanyaan bisnis utama:
1. Segmen pasar mana yang paling menguntungkan namun memiliki risiko pembatalan tertinggi?
2. Bagaimana tren pendapatan (Revenue) dan tarif harian rata-rata (ADR) sepanjang tahun?
3. Seberapa sering terjadi ketidaksesuaian operasional (tamu tidak mendapatkan tipe kamar yang dipesan)?

## 📊 Fitur & Analisis Utama
Dashboard ini terdiri dari beberapa analisis kunci:

### 1. Analisis Pendapatan (Revenue Analysis)
- **Total Revenue & ADR:** Memantau pendapatan total dan harga rata-rata kamar per malam.
- **Seasonal Trend:** Visualisasi tren pendapatan bulanan untuk mengidentifikasi *peak season* (musim ramai) dan *low season*.

### 2. Analisis Pembatalan (Cancellation Analysis)
- **Volume vs Risiko:** Menggunakan *Combo Chart* untuk membandingkan jumlah booking (Volume) dengan persentase pembatalan (Risk) per segmen pasar.
- **Insight:** Menemukan bahwa segmen **Online TA** memiliki volume tertinggi namun juga tingkat pembatalan yang signifikan, sedangkan segmen **Direct** cenderung lebih loyal.

### 3. Efisiensi Operasional (Room Operations)
- **Reserved vs Assigned Room:** Menganalisis ketidaksesuaian antara kamar yang dipesan dengan kamar yang diberikan.
- **Impact Analysis:** Mengidentifikasi apakah perubahan tipe kamar (upgrade/downgrade) mempengaruhi keputusan tamu untuk membatalkan pesanan.

## 🛠️ Tools & Teknologi
- **Microsoft Power BI:** Untuk visualisasi data interaktif dan dashboarding.
- **Power Query:** Untuk pembersihan data (ETL), pembuatan kolom kondisional, dan transformasi data.
- **DAX (Data Analysis Expressions):** Digunakan untuk membuat *Calculated Measures* seperti:
  - `Total Revenue`
  - `Cancellation Rate %`
  - `Room Mismatch Status`
- **Data Modelling:** Menggunakan skema hubungan (Star Schema) antara tabel fakta (*fact_bookings*) dan tabel dimensi (*dim_date*, *dim_room*).

### 🔗 [Klik di sini untuk melihat Dashboard Interaktif](https://app.powerbi.com/view?r=eyJrIjoiM2NiYzJhMTEtNGMyZS00MTdlLTlhNDMtYWRjMzA4ZmVjNGVmIiwidCI6IjM0NjI3ODc0LWVkM2EtNDk3Yy04ZmI5LTE2Y2U3ZTk3NjRmMSIsImMiOjEwfQ%3D%3D)

## 📂 Struktur File
```text
📁 Hotel-BI-Dashboard
│
├── 📄 Hotel_Dashboard_Naufal.pbix  # File project Power BI (Download untuk melihat interaksi)
├── 📄 hotel_bookings.csv           # Dataset mentah (Sumber: Kaggle)
├── 📁 screenshots                  # Kumpulan gambar preview dashboard
│   ├── dashboard_main.png
│   └── analysis_cancel.png
└── 📝 README.md                    # Dokumentasi proyek ini


