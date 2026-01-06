# 🎓 SPK Alokasi Dana Pendidikan Papua Pegunungan (AHP-TOPSIS)

Sistem Pendukung Keputusan (SPK) untuk menentukan prioritas alokasi dana bantuan infrastruktur pendidikan di Provinsi Papua Pegunungan menggunakan integrasi metode **Analytic Hierarchy Process (AHP)** dan **TOPSIS**.
🔗 **Akses Aplikasi:** [edufund-decision.streamlit.app](https://edufund-decision.streamlit.app/)

## 📌 Latar Belakang
Provinsi Papua Pegunungan menghadapi tantangan disparitas infrastruktur pendidikan yang kompleks karena faktor geografis ekstrem. Dengan keterbatasan anggaran, diperlukan mekanisme pengambilan keputusan yang objektif agar alokasi dana tepat sasaran pada kabupaten yang paling membutuhkan intervensi segera.

## 🛠️ Metodologi
Sistem ini beroperasi dalam dua tahapan utama:
1.  **Analytic Hierarchy Process (AHP):** Digunakan untuk menghitung bobot kepentingan relatif kriteria melalui matriks perbandingan berpasangan (Pairwise Comparison).
2.  **TOPSIS:** Menghasilkan ranking kabupaten berdasarkan jarak terdekat dari solusi ideal positif dan jarak terjauh dari solusi ideal negatif.



## 📊 Kriteria Penilaian
Terdapat 4 kriteria utama yang digunakan (Data TA 2022/2023):
- **C1: Kondisi Ruang Kelas (Cost):** Persentase kerusakan ruang kelas.
- **C2: Jumlah Perpustakaan (Benefit):** Jumlah perpustakaan sekolah kondisi baik.
- **C3: Akses Listrik (Cost):** Persentase sekolah tanpa akses listrik.
- **C4: Akses Komputer (Benefit):** Persentase sekolah dengan fasilitas komputer.

## 🚀 Panduan Jalankan Aplikasi

### 1. Persiapan Lingkungan (Setup)
* **Buat Folder Proyek:** Buat folder baru di komputer Anda, misalnya `spk_papua`.
* **Buka Terminal/CMD:** Masuk ke dalam folder tersebut.
* **Buat Virtual Environment:**
    ```bash
    python -m venv venv
    ```
* **Aktifkan Virtual Environment:**
    * **Windows:** `venv\Scripts\activate`
    * **Mac/Linux:** `source venv/bin/activate`

### 2. Instalasi Library
Jalankan perintah ini untuk menginstal dependensi yang dibutuhkan:
```bash
pip install streamlit pandas numpy
```

### 3. Menjalankan Aplikasi
Simpan kode sumber Anda sebagai app.py di folder tersebut, lalu jalankan:
```bash
streamlit run app.py
```
Aplikasi akan otomatis terbuka di browser Anda pada alamat http://localhost:8501.

## **📝 Fitur Utama**
* **Sidebar Konfigurasi**: Mengatur jumlah kriteria dan alternatif secara dinamis.
* **Pairwise Matrix**: Input nilai perbandingan kriteria AHP secara transparan.
* **Transparansi Kalkulasi**: Menampilkan Matriks Keputusan (X), Matriks Ternormalisasi (R), Matriks Terbobot (V), hingga Solusi Ideal.
* **Visualisasi Ranking**: Kartu hasil ranking berwarna berdasarkan tingkat urgensi.

© 2026 - Sistem Pendukung Keputusan Alokasi Dana Pendidikan Papua Pegunungan.
