# Excel Tools — Penggabung & Pemisah (Split) Excel

Aplikasi web modern berbasis client-side untuk mengolah data file Excel (.xlsx, .xls) dan CSV tanpa perlu server atau upload data ke pihak ketiga (100% aman dan berjalan di browser).

---

## Fitur Utama

### 1. Gabung Excel (Merge)
- Menggabungkan beberapa file Excel / CSV menjadi satu file.
- Struktur kolom otomatis mengikuti urutan dan nama kolom pada **file pertama**.
- Pemetaan kolom otomatis jika urutan kolom pada file berikutnya berbeda.
- Opsi pengurutan data (*sorting*) berdasarkan kolom yang dipilih.
- Pratinjau (*preview*) data hasil gabungan sebelum diunduh.
- Unduh hasil dalam format `.xlsx` atau `.csv`.

### 2. Split Excel (Fitur Canggih & Fleksibel 🚀)
- **Split Multi-Kolom dengan Pengaturan Urutan (Order)**:
  - Dapat memisahkan file berdasarkan **1 atau lebih kolom acuan**.
  - Dilengkapi tombol geser urutan (▲ / ▼) untuk mengatur prioritas pemisahan (*hierarchical grouping*) dan susunan nama file output.
  - Setiap kolom acuan memiliki konfigurasi aturan karakter independen.
- **Tipe Data Output Teks Murni (Anti Notasi E 🛡️)**:
  - Seluruh kolom dan sel pada file output (.xlsx) diatur bertipe **teks murni (`text format` `@`)**.
  - Menjamin angka berdigit panjang (seperti NIK 16 digit, nomor KK, nomor telepon/HP, ID pelanggan, barcode) **tidak berubah menjadi notasi ilmiah `E`** (misal `3.201E+15`) dan angka 0 di depan tetap aman terjaga.
- **Fleksibilitas Pemotongan Karakter**:
  - Ambil sejumlah digit/karakter dari kiri (contoh: 2 digit kode provinsi, 4 digit kode kecamatan).
  - Atau gunakan seluruh isi kolom tanpa pemotongan.
- **Nama File Output Kustom & Berurutan**:
  - Format penamaan mengikuti urutan kolom: `[ref_kolom_1]_[ref_kolom_2]_[inputan user]_[timestamp].xlsx`
  - Contoh: `32_01_rekap_kecamatan_20261010_092500.xlsx`
  - Dilengkapi *live preview* nama file dan pola format secara real-time saat mengetik.
- **Opsi Unduhan Fleksibel**:
  - **Unduh Semua (.ZIP)**: Satu kali klik untuk mengunduh seluruh file hasil split dalam arsip ZIP. Menggunakan pemrosesan *asynchronous chunking* non-blocking sehingga browser tidak akan membeku (*unresponsive*) bahkan saat memproses ratusan file sekaligus.
  - **Unduh Satu per Satu**: Unduh file individual langsung dari tabel hasil (.xlsx atau .csv).
  - **Pratinjau Data**: Lihat data isi baris untuk masing-masing grup split sebelum mengunduh.

### 3. Animasi Indikator Proses (Upload & Unduh ✨)
- **Animasi Saat Upload Berkas**:
  - Modal animasi pemrosesan file yang muncul otomatis saat file diseret atau dipilih.
  - Ikon upload panah melayang dinamis (*upward bouncing icon*) dengan cincin rotasi gradien.
  - Indikator progres membaca file demi file secara *real-time* (misal: *Membaca berkas 2 dari 5: data.xlsx*).
  - Area *Drop Zone* aktif berdenyut dengan indikator pemrosesan.
- **Animasi Saat Unduh Berkas**:
  - Modal animasi berdesain *glassmorphism* modern dengan *backdrop blur*.
  - Ikon unduh interaktif (*bouncing download arrow*, *spinning gradient ring*, & *pulsing glow*).
  - Indikator bar progres visual dengan persentase *real-time* (pada pengompresan ZIP dan unduh berurutan).
  - Memberikan feedback visual yang jelas dan responsif saat browser memproses data besar.

### 4. Tampilan File Terunggah Minimalis & Kompak
- **Tata Letak Grid Responsif**: Menggunakan multi-kolom responsif sehingga tidak memanjang ke bawah ketika mengunggah puluhan hingga ratusan berkas sekaligus.
- **Scrollbar Halus & Ketinggian Terkendali**: Batas ketinggian maksimal (*max-height: 230px*) dengan scrollbar halus terintegrasi menjaga antarmuka tetap rapi dan ringkas.
- **Kartu Berkas Ringkas**: Informasi ukuran file, jumlah baris, dan jumlah kolom tertata rapi dengan pemisah titik minimalis, teks nama file terpotong elegan jika terlalu panjang (*ellipsis*), serta *tooltip* nama lengkap saat kursor diarahkan ke file.

---

## Cara Menjalankan

Cukup buka file `index.html` langsung di browser favorit Anda (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari) tanpa perlu menginstal runtime tambahan.