# Global-Retail-Performance-Dashboard-2024
Analisis penjualan retail global dengan 1.000 transaksi di 10 negara, dengan menggunakan Excel (VLOOKUP/HLOOKUP/Pivot) untuk analisis, dan dashboard interaktif untuk insight bisnis.

#### Tujuan:
1. Melakukan data enrichment menggunakan VLOOKUP.
2. Menghitung metrik bisnis (Gross Sales, Net Sales, Profit, Margin).
3. Membuat 5 Pivot Table untuk analisis multidimensi.
4. Menyusun dashboard interaktif dengan insight bisnis yang actionable.

#### Sheet dalam File Excel

| Sheet | Isi | 
|---|---|
| RAW_DATA | Data mentah (13 kolom) |
| REF_Country | Master negara (region, kode, tax rate) | 
| REF_Target | Target Q1–Q4 per kategori |
| REF_Cost | Harga modal per kategori | 
| ANALYSIS | Data + 12 kolom hasil rumus |
| Pivot_1 – Pivot_5 | 5 Pivot Table analisis | 
| DASHBOARD | Dashboard visual | 

#### Proses yang Dilakukan
1. Data Enrichment (VLOOKUP) <br> Melengkapi kolom kosong dengan data dari tabel referensi: <br> - Region (dari REF_Country) <br> - Country Code (dari REF_Country) <br> - Tax Rate (dari REF_Country) <br> - Target Q1 (dari REF_Target) <br> - Cost Per Unit (dari REF_Cost)
2. Kalkulasi Metrik Penjualan <br> Menghitung kolom turunan menggunakan rumus aritmatika, seperti: <br> - Gross Sales (Quantity × Unit Price) <br> - Discount Amount (Gross Sales × Discount Rate) <br> - Net Sales (Gross Sales − Discount Amount) <br> - Total Cost (Cost Per Unit × Quantity) <br> - Profit (Net Sales − Total Cost)
3. Ekstraksi Dimensi Waktu <br> Membuat kolom waktu dari Order_Date, seperti: <br> - Month (nama bulan) <br> - Quarter (Q1–Q4) <br> - Year (tahun)
4. Analisis Pivot Table  <br> Membuat Pivot Table untuk analisis, seperti: <br> - Pivot Net Sales per Country <br> - Pivot Trend Penjualan Bulanan <br> - Pivot Category × Channel <br> - Pivot Top 5 Products <br> - Pivot Region Performance 
5. Visualisasi Chart <br> Membuat chart dari Pivot Table, seperti: <br> - Line Chart (trend bulanan) <br> - Horizontal Bar Chart (top countries) <br> - Pie Chart (category × channel) <br> - Pie Chart (top 5 products) <br> - Doughnut Chart (profit by region)
6. Pembuatan Dashboard <br> Menyusun dashboard interaktif yang berisi: <br> - 4 KPI Cards (Total Net Sales, Profit, Quantity, Orders) <br> - 5 Chart dari Pivot Table

#### Dashboad Preview
![Dashboard](Dashboard.png)
![Dashboard](BeforeAfter.png)
![dashboard](Pivot.png)


