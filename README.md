# 💻 Warung Seblak Jaya - Point of Sale System

Aplikasi berbasis Python yang digunakan untuk mencatat transaksi penjualan makanan seperti Mie Jebew dan Seblak di Warung Seblak Jaya - SMKN 1 Probolinggo. Sistem ini mendukung multi pembeli, pencetakan struk, serta penyimpanan data transaksi ke dalam format JSON.

---

## 📌 Fitur

- ✅ Input transaksi hingga 5 pembeli sekaligus
- ✅ Pilihan menu Mie Jebew dan Seblak dengan level pedas, rasa, dan jenis kuah
- ✅ Cetak struk transaksi dengan format rapi
- ✅ Simulasi pembayaran dengan metode Cash atau QRIS
- ✅ Simpan transaksi ke file `transaksi.json`
- ✅ Validasi input jumlah dan nominal pembayaran
- ✅ Tampilkan isi file JSON setelah transaksi

---

## 🧰 Teknologi yang Digunakan

- Bahasa Pemrograman: **Python 3**
- Modul Bawaan: `json`
- Tidak menggunakan library eksternal
- Bisa dikompilasi menjadi `.exe` menggunakan `pyinstaller`

---

## 🛠️ Cara Instalasi

### 📦 Dari File .exe

1. Unduh file `UASDPK.exe`
2. Jalankan aplikasi langsung dengan klik ganda (tidak memerlukan Python)

### 🧑‍💻 Dari Kode Sumber

1. Pastikan Python 3 telah terinstal di sistem
2. Clone atau unduh proyek ini
3. Jalankan program menggunakan perintah:

```bash
python UASDPK.py
```

---

## 👨‍🏫 Panduan Pengguna

1. Jalankan program
2. Masukkan nama penjual
3. Masukkan jumlah pembeli (maksimal 5)
4. Untuk setiap pembeli:
   - Masukkan nama pembeli
   - Pilih kategori: `Mie Jebew`, `Seblak`, atau `Selesai`
   - Pilih topping dan jumlah untuk tiap kategori
   - Masukkan level pedas (1-5), jenis kuah (berkuah/nyemek), dan rasa (asin/manis/gurih manis) sesuai pilihan kategori
5. Setelah selesai memilih, pilih metode pembayaran: `Cash` atau `QRIS`
6. Masukkan nominal pembayaran (minimal sama dengan total)
7. Struk akan dicetak ke terminal
8. Transaksi otomatis disimpan ke `transaksi.json`
9. Anda bisa memilih untuk menampilkan isi file JSON setelah transaksi

---

## 📁 Struktur Folder

```plaintext
.
├── UASDPK.py           # File utama Python (kode sumber)
├── UASDPK.exe          # File executable hasil konversi (opsional)
├── UASDPK.spec         # File spesifikasi PyInstaller (jika dikompilasi)
├── transaksi.json      # Output file JSON hasil transaksi
└── README.md           # Dokumentasi aplikasi
```

---

## 📄 Dokumentasi Kode (Ringkasan)

- `Item`, `MieJebew`, `Seblak` → representasi objek makanan
- `ItemDetail` → detail pesanan pembeli
- `Transaksi` → logika utama pencatatan, penghitungan, pencetakan struk, dan penyimpanan
- `main()` → fungsi utama yang menangani alur input dari pengguna

---

## 📝 Lisensi

Proyek ini dibuat untuk keperluan tugas UAS DPK dan bebas digunakan untuk keperluan edukasi.

---

## 🙌 Kontributor

- **Nama:** [Isi Nama Anda]
- **Sekolah:** SMKN 1 Probolinggo
- **Mata Pelajaran:** Dasar Pemrograman Komputer (DPK)
