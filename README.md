# 🌍 Simulasi Ekonomi Makro Interaktif

Aplikasi web untuk mensimulasikan dampak kebijakan moneter dan fiskal menggunakan kerangka **New Keynesian Open Economy Model**.

![Demo](https://img.shields.io/badge/Demo-Live-brightgreen)
![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-1.32+-red)

## 🚀 Deploy ke Streamlit Cloud

1. **Fork/Clone repository ini** ke akun GitHub Anda
2. Buka [share.streamlit.io](https://share.streamlit.io)
3. Login dengan GitHub → Klik **New App**
4. Pilih repository ini → Branch: `main` → Main file: `app.py`
5. Python version: `3.10` atau `3.11`
6. Klik **Deploy!** 🎉

Aplikasi akan live di: `https://[nama-app].streamlit.app`

## 📦 Fitur Utama

✅ **Model Ekonomi Lengkap**
- Taylor Rule (kebijakan moneter endogen)
- Kurva Phillips (dinamika inflasi)
- Adaptive Expectations (pembelajaran agen)
- UIP & Neraca Perdagangan (sektor eksternal)
- IS Curve (dinamika output gap)

✅ **Simulasi Monte Carlo**
- 50–500 jalur stokastik
- Pita kepercayaan 90% (fan chart)
- Guncangan demand, supply, kebijakan, eksternal

✅ **Interaktif & Edukatif**
- Slider parameter real-time
- Upload dataset CSV kustom
- Download sample data
- Export hasil ke CSV/Excel

✅ **Analisis Otomatis**
- Klasifikasi rezim ekonomi (Stabil/Waspada/Tegangan)
- Penilaian stance kebijakan moneter
- Indikator risiko & rekomendasi kebijakan

## 🎮 Cara Menggunakan

### 1. Jalankan dengan Data Default
- Buka aplikasi → simulasi dummy otomatis berjalan
- Lihat grafik, metrik, dan analisis di dashboard

### 2. Ubah Parameter Kebijakan
- Geser slider di sidebar (θπ, θy, G, dll.)
- Klik **🔄 Jalankan Ulang Simulasi**
- Amati perubahan grafik & analisis

### 3. Upload Dataset Kustom
- Klik **📥 Download Sample Dataset** untuk template
- Siapkan CSV dengan kolom: `periode`, `G`, `r_world`
- Upload via **📤 Upload CSV Anda**
- Klik **🔄 Jalankan Ulang Simulasi**

### 4. Export Hasil
- Buka tab **📥 Data Lengkap**
- Klik **📄 Unduh CSV** atau **📊 Unduh Excel**

## ⚙️ Parameter yang Dapat Diatur

| Parameter | Simbol | Rentang | Default | Arti |
|-----------|--------|---------|---------|------|
| Respons Inflasi | θπ | 0.0 – 3.0 | 1.5 | Koefisien Taylor Rule terhadap inflasi |
| Respons Output | θy | 0.0 – 2.0 | 1.1 | Koefisien Taylor Rule terhadap output gap |
| Adaptive Exp. | λ | 0.0 – 1.0 | 0.65 | Bobot pembelajaran dari inflasi masa lalu |
| Phillips Slope | κ | 0.0 – 0.5 | 0.18 | Sensitivitas inflasi terhadap output |
| Fiscal Multiplier | φ | 0.0 – 1.0 | 0.35 | Efektivitas stimulus fiskal |
| Ketidakpastian | σ | 0.0 – 1.5 | 0.45 | Volatilitas guncangan stokastik |
| Jumlah Simulasi | N_sim | 50 – 500 | 150 | Jalur Monte Carlo |
| Stimulus Fiskal | G | 0.5 – 2.0 | 1.0 | Level baseline pengeluaran pemerintah |
| Target Inflasi | π* | 0.0 – 5.0 | 2.25 | Anchor kebijakan bank sentral |
| Suku Bunga Netral | r* | 0.0 – 6.0 | 3.0 | Tingkat suku bunga riil netral |
| Suku Bunga Dunia | rʷ | 0.0 – 6.0 | 2.0 | Acuan kebijakan moneter global |

## 📚 Referensi Model

1. Taylor, J. B. (1993). *Discretion versus policy rules in practice*. Carnegie-Rochester.
2. Galí, J. (2015). *Monetary Policy, Inflation, and the Business Cycle*. Princeton.
3. Obstfeld, M. & Rogoff, K. (1996). *Foundations of International Macroeconomics*. MIT.
4. Bank Indonesia. (2023). *Laporan Kebijakan Moneter*.

## ⚠️ Disclaimer

Aplikasi ini bersifat **edukatif dan stylized**. Model menggunakan parameter ilustratif dan tidak menggantikan model forecasting resmi bank sentral atau lembaga internasional. Hasil simulasi tidak boleh digunakan sebagai dasar pengambilan kebijakan moneter/fiskal tanpa kalibrasi empiris lanjutan.

## 🤝 Kontribusi

1. Fork repository
2. Buat branch fitur (`git checkout -b fitur/baru`)
3. Commit perubahan (`git commit -am 'Tambah fitur X'`)
4. Push ke branch (`git push origin fitur/baru`)
5. Buka Pull Request

## 📄 Lisensi

Distributed under the MIT License. See `LICENSE` for more information.

---
**Dibuat dengan ❤️ untuk edukasi kebijakan makroekonomi**  
[www.dataaksi.id](https://www.dataaksi.id)