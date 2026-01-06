Maksud saya, jawaban sebelumnya sudah saya masukkan ke dalam **kotak kode (code block)** agar format Markdown-nya tidak terproses oleh sistem saya, sehingga Anda bisa melihat simbol-simbol aslinya (seperti `###`, `*`, dan backtick ```).

Jika Anda ingin membuat file bernama `PANDUAN.md`, silakan **Copy & Paste** isi di bawah ini:

```markdown
# Panduan Jalankan Aplikasi SPK Papua

### 1. Persiapan Lingkungan (Setup)
* **Buat Folder Proyek:** Buat folder baru bernama `spk_papua`.
* **Buka Terminal/CMD:** Masuk ke folder tersebut.
* **Buat Virtual Environment:**
  ```bash
  python -m venv venv

```

* **Aktifkan Virtual Environment:**
* **Windows:** `venv\Scripts\activate`
* **Mac/Linux:** `source venv/bin/activate`



---

### 2. Instalasi Library

Jalankan perintah ini di terminal:

```bash
pip install streamlit pandas numpy

```

---

### 3. Menyimpan Kode Sumber

1. Salin kode program yang sudah ada.
2. Simpan dengan nama **`app.py`** di dalam folder `spk_papua`.

---

### 4. Menjalankan Aplikasi

Jalankan perintah:

```bash
streamlit run app.py

```

---

> **Tips:** Aplikasi biasanya berjalan di `http://localhost:8501`. Pastikan venv aktif setiap kali ingin menjalankan aplikasi.
