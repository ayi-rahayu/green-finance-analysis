# 🌱 Green Finance Integrated Analysis
Analisis gabungan dari dataset keuangan, lingkungan, sosial, ekonomi, dan geospasial proyek hijau di Indonesia.

## 📘 Deskripsi
Repositori ini dibuat sebagai bagian dari tugas *Eco Techno Leader* untuk memahami dan memimpin transformasi berbasis data dalam keuangan berkelanjutan (Green Finance). Dataset ini mencakup informasi finansial, lingkungan, sosial, ekonomi makro, dan geospasial dari proyek-proyek hijau.

## 📂 Struktur Dataset

### 1. Financial Dataset
| Field | Deskripsi |
|-------|-----------|
| `Investment_Amount` | Total dana yang diinvestasikan dalam proyek (Rp). |
| `Loan_Interest_Rate` | Suku bunga pinjaman per tahun (%). |
| `Default_Risk_Score` | Skor risiko gagal bayar (0-100). |
| `Green_Bond_Spread` | Selisih imbal hasil obligasi hijau dan konvensional (bps). |

📌 *Formula:*
```math
GNPV = Σ (CFₜ + Eₜ) / (1 + r)ᵗ - I₀
```

### 2. Environmental Dataset
| Field | Deskripsi |
|-------|-----------|
| `CO2_Emissions_Reduction` | Ton emisi CO2 yang dikurangi per tahun. |
| `Renewable_Energy_Share` | Persentase energi terbarukan (%). |
| `Water_Savings` | Penghematan air (m³/tahun). |
| `Biodiversity_Impact_Score` | Skor dampak keanekaragaman hayati (-100 sampai 100). |

📌 *Formula:*
```math
CROI = Σ (Rₜ + Pc) / I₀
```

### 3. Social Dataset
| Field | Deskripsi |
|-------|-----------|
| `Jobs_Created` | Jumlah lapangan kerja tetap (FTE). |
| `Community_Engagement_Score` | Skor keterlibatan masyarakat (0-100). |
| `Access_to_Clean_Energy_Rate` | Peningkatan akses energi bersih (%). |
| `Gini_Coefficient_Impact` | Perubahan terhadap ketimpangan pendapatan. |

📌 *Formula:*
```math
SROI = Σ (NVsocial) / I₀
```

### 4. Economic Dataset
| Field | Deskripsi |
|-------|-----------|
| `GDP_Growth` | Pertumbuhan PDB (%). |
| `Inflation_Rate` | Inflasi tahunan (%). |
| `FDI_Inflows` | Investasi asing langsung (miliar USD). |
| `Unemployment_Rate` | Tingkat pengangguran (%). |

📌 *Formula:*
```math
ERAF = 1 + w₁·ΔInflasi + w₂·ΔPengangguran − w₃·ΔPDB
```

### 4. Geospatial Dataset
| Field | Deskripsi |
|-------|-----------|
| `Latitude / Longitude` | Koordinat proyek. |
| `Proximity_to_Protected_Area` | Jarak ke area lindung (km). |
| `Land_Use_Change` | Perubahan tutupan lahan. |

📌 *Formula:*
```math
GRI = w₁·S_hazard + w₂·S_proximity + w₃·S_landuse
```

## 📈 Model Prediktif
- **Regresi Linear**: Prediksi pengurangan emisi berdasarkan investasi.
- **Regresi Logistik**: Prediksi keberhasilan proyek (Y = 1 / gagal = 0).
- Gunakan nilai-nilai seperti `CO2_Emissions_Reduction`, `Default_Risk_Score`, dan `Investment_Amount`.

## 📜 Regulasi Pendukung
- **OJK**: POJK No. 60/2017 dan No. 51/2017
- **THI**: Taksonomi Hijau Indonesia
- **Perpres No. 98 Tahun 2021** – Nilai Ekonomi Karbon
- **UU No. 32 Tahun 2009** – Perlindungan dan Pengelolaan Lingkungan Hidup

## 💡 Tips Praktis Pengambilan Keputusan Investasi Hijau

Gunakan metrik berikut sebagai indikator utama dalam evaluasi proyek:

- **GNPV**, **SROI**, dan **CROI** untuk menilai kelayakan finansial, sosial, dan lingkungan proyek.
- **Prioritaskan proyek** dengan karakteristik sebagai berikut:
  - `CO2_Emissions_Reduction > 50 ton`
  - `CROI > 1`
  - `GRI < 0.7`
- Pastikan transparansi data sosial dan tingkat keterlibatan masyarakat yang tinggi dalam perencanaan dan pelaksanaan proyek.

---

## 🧠 Referensi Akademik

- Sachs et al. (2023) – *Handbook of Green Finance*
- Tolliver et al. (2022) – *Journal of Cleaner Production*
- IPCC (2023) – *Climate Change Synthesis Report*

## 📁 Struktur Folder & File GitHub
```
green-finance-analysis/
│
├── README.md                   ← Penjelasan lengkap proyek dan semua indikator
├── requirements.txt            ← Daftar pustaka Python yang dibutuhkan
├── .gitignore                  ← Abaikan file yang tidak perlu (misal: *.ipynb_checkpoints)
│
├── notebooks/
│   └── GreenFinance_Analysis.ipynb  ← Jupyter Notebook utama (analisis semua aspek)
│
├── data/
│   ├── Financial_Dataset.xlsx
│   ├── Environmental_Dataset.xlsx
│   ├── Social_Dataset.xlsx
│   ├── Economic_Dataset.xlsx
│   └── Geospatial_Dataset.xlsx
│
└── visualizations/
    ├── gnpv_bar_chart.png
    ├── croi_bar_chart.png
    ├── sroi_bar_chart.png
    ├── eraf_bar_chart.png
    └── gri_bar_chart.png
```
