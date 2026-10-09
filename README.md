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

### 2. Split Excel (Fitur Terbaru 🚀)
- Memisahkan data Excel menjadi beberapa file terpisah berdasarkan nilai kolom acuan.
- Struktur kolom dan tata letak tetap konsisten mengikuti **file pertama**.
- **Fleksibilitas Pemotongan Karakter**:
  - Ambil sejumlah digit/karakter dari kiri (contoh: 4 digit dari kiri kolom A / kode wilayah).
  - Atau gunakan seluruh isi kolom tanpa pemotongan.
- **Nama File Output Kustom**:
  - Format penamaan: `[referensi split]_[inputan user]_[timestamp].xlsx`
  - Contoh: `3201_rekap_kecamatan_20261009_145022.xlsx`
  - Dilengkapi *live preview* nama file secara real-time saat mengetik.
- **Opsi Unduhan Fleksibel**:
  - **Unduh Semua (.ZIP)**: Satu kali klik untuk mengunduh seluruh file hasil split yang dibungkus rapi dalam arsip ZIP.
  - **Unduh Satu per Satu**: Unduh file individual langsung dari tabel hasil.
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