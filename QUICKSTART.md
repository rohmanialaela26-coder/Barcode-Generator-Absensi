# ⚡ Quick Start Guide

Panduan cepat untuk mulai menggunakan Barcode Absensi Generator dalam 5 menit!

---

## 🎯 Dalam 5 Menit

### 1️⃣ Download (30 detik)

Pilih salah satu:

**Opsi A: Download File Langsung**
- Download `barcode-absensi-excel.html`
- Download `template-siswa.xlsx`

**Opsi B: Clone dari GitHub**
```bash
git clone https://github.com/username/barcode-absensi-generator.git
cd barcode-absensi-generator
```

### 2️⃣ Buka Aplikasi (10 detik)

1. Cari file `barcode-absensi-excel.html`
2. **Double-click** atau **drag ke browser**
3. Aplikasi terbuka di browser

✅ **Selesai!** Tidak perlu instalasi apapun.

### 3️⃣ Siapkan Data (2 menit)

**Opsi A: Gunakan Template**
1. Buka aplikasi
2. Klik "Download Template Excel"
3. Edit template dengan data siswa Anda
4. Simpan file

**Opsi B: Pakai Excel Sendiri**
1. Buat file Excel dengan 3 kolom:
   - Kolom A: NIS (contoh: 001, 002, 003)
   - Kolom B: NAMA (contoh: Ahmad Rizki)
   - Kolom C: KELAS (contoh: 10-A, 11-B)
2. Tambahkan header di baris pertama
3. Simpan sebagai `.xlsx` atau `.csv`

### 4️⃣ Generate Kartu (1 menit)

1. **Upload file Excel**
   - Drag & drop ke area upload
   - Atau klik tombol upload

2. **Review preview**
   - Lihat 5 baris pertama data Anda
   - Pastikan format benar

3. **Klik "Generate Kartu"**
   - Tunggu sebentar...
   - Barcode otomatis terbuat!

4. **Download atau Cetak**
   - Download ZIP: simpan semua kartu
   - Print: langsung ke printer
   - Export CSV: backup data

---

## 🎫 Format Data Excel yang Benar

### ✅ Template yang Benar

```
| NIS | NAMA | KELAS |
|-----|------|-------|
| 001 | Ahmad Rizki | 10-A |
| 002 | Budi Santoso | 10-A |
| 003 | Citra Dewi | 10-B |
```

### ✅ Apa yang Boleh

```
NIS:
- 001, 002, 003 (angka)
- S001, A02 (dengan huruf)
- Max 5 karakter

NAMA:
- Ahmad Rizki (dengan spasi)
- Budi Santoso (dengan spasi)
- Citra Dewi Putri (nama panjang ok)

KELAS:
- 10-A (format standar)
- 10A (tanpa dash)
- X-A (Roman numeral)
- 1-A (satu digit)
- Semua format support!
```

### ❌ Apa yang TIDAK Boleh

```
❌ NIS: Kosong (wajib ada)
❌ NAMA: Kosong (wajib ada)
❌ Baris pertama bukan header
❌ Format: .doc atau .xls lama
❌ Encoding: Special characters aneh
```

---

## 📥 Langkah Upload File

### Cara Upload (3 cara)

**Cara 1: Drag & Drop** (paling mudah)
1. Buka aplikasi
2. Ambil file Excel dari folder
3. Drag ke area upload (bagian biru)
4. Drop file
5. Done! Preview otomatis muncul

**Cara 2: Klik Upload**
1. Klik tombol upload
2. Browse folder
3. Pilih file Excel
4. Klik Open
5. File terbaca otomatis

**Cara 3: Copy-Paste Path** (advanced)
1. Copy full path file
2. Edit HTML (buka di text editor)
3. Modify script
4. (Tidak recommended untuk pemula)

### Troubleshooting Upload

| Problem | Solusi |
|---------|--------|
| File tidak terbaca | Pastikan format .xlsx atau .csv |
| Preview kosong | Cek header ada di baris 1 |
| Data tidak muncul | NIS atau NAMA mungkin kosong |
| File terlalu besar | Hapus sheet yang tidak perlu dulu |

---

## 🖨️ Cetak Kartu

### Persiapan Sebelum Cetak

**Hardware:**
- ✓ Printer (bisa color atau B&W)
- ✓ Kertas HVS A4 putih

**Software:**
- ✓ Browser sudah siap (Chrome recommended)
- ✓ File HTML sudah generate kartu

### Langkah Cetak

```
1. Klik tombol "Cetak Kartu" di aplikasi
   ATAU Tekan Ctrl+P (Cmd+P di Mac)

2. Dialog print terbuka, setting:
   - Printer: Pilih printer Anda
   - Paper: A4
   - Margins: Normal
   - Orientation: Portrait
   - Scale: 100% (penting!)

3. Klik "Print Preview" untuk check dulu

4. Klik "Print" jika OK
```

### Tips Cetak Berkualitas

✓ **Test print 1-2 halaman dulu** - jangan print semua langsung  
✓ **Biarkan tinta kering 5 menit** - hindari smudge  
✓ **Potong dengan cutter** - hasil lebih rapi  
✓ **Laminating** - buat kartu tahan bertahun-tahun  
✓ **Punch lubang** - buat gantungan jika perlu  

---

## 📦 Download Kartu

### Download Opsi 1: ZIP (Recommended)

**Apa didapat:**
- Semua kartu dalam 1 file
- INDEX.html untuk navigasi
- CSV data backup
- Bisa dibuka offline

**Cara:**
1. Klik "Download ZIP"
2. File otomatis download
3. Extract ZIP ke folder
4. Buka INDEX.html
5. Klik nama siswa untuk lihat kartu

**Keuntungan:**
- ✅ Terdiri dari banyak file
- ✅ Mudah di-share
- ✅ Bisa dibuka offline
- ✅ File terpisah per siswa

### Download Opsi 2: CSV

**Apa didapat:**
- Data siswa + barcode code dalam CSV
- Bisa dibuka di Excel
- Cocok untuk database/automation

**Cara:**
1. Klik "Download CSV"
2. File CSV otomatis download
3. Buka di Excel atau text editor

---

## 🎬 Contoh Workflow Lengkap

### Scenario: Guru membuat kartu untuk 200 siswa

```
📋 Langkah 1: Persiapan (5 menit)
├─ Guru buka Excel yang sudah ada (daftar siswa)
├─ Check format: NIS | NAMA | KELAS
└─ Save file

🎫 Langkah 2: Generate (2 menit)
├─ Buka barcode-absensi-excel.html
├─ Upload file Excel
├─ Klik Generate Kartu
└─ Preview ok ✓

📦 Langkah 3: Download (1 menit)
├─ Klik "Download ZIP"
├─ Extract ZIP
└─ Cek INDEX.html

🖨️ Langkah 4: Cetak (20 menit untuk 200 kartu)
├─ Buka ZIP yang sudah di-extract
├─ Preview beberapa kartu
├─ Buka dengan default print setting
├─ Print (perhatikan margin & scale!)
└─ Biarkan tinta kering

✂️ Langkah 5: Finishing (30 menit)
├─ Potong kartu sesuai garis tepi
├─ Punch lubang (optional)
├─ Laminating (optional tapi recommended)
└─ Kartu ready to use! 🎉

⏱️ Total waktu: ~1 jam untuk 200 siswa
```

---

## 🆘 Help & Troubleshooting

### Common Issues & Solutions

| Issue | Penyebab | Solusi |
|-------|----------|--------|
| Aplikasi tidak mau buka | File HTML rusak | Download ulang |
| Upload failed | Browser cache | Refresh & coba lagi |
| Barcode blur | Printer setting | Check 100% scale |
| ZIP tidak bisa di-extract | File corrupt | Download ulang |
| Data tidak muncul | Format Excel salah | Check header & kolom |

### Bantuan Lebih Lanjut

**Lihat dokumentasi lengkap:**
- 📖 [README.md](README.md) - Dokumentasi lengkap
- 🐛 [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md) - Masalah & solusi
- 💬 [GitHub Issues](https://github.com/username/barcode-absensi-generator/issues) - Q&A komunitas

**Contact Support:**
- 📧 Email: support@example.com
- 💬 Forum: https://github.com/username/barcode-absensi-generator/discussions

---

## 🚀 Tips Sukses

### Untuk Pemula

✓ Jangan takut coba-coba  
✓ Test dengan data kecil dulu (10-20 siswa)  
✓ Jangan langsung print semua sekaligus  
✓ Baca dokumentasi jika ada masalah  

### Untuk Pengguna Reguler

✓ Simpan template Excel (bisa reuse tahun depan)  
✓ Backup data (simpan CSV yang di-export)  
✓ Laminating kartu buat tahan lama  
✓ Organize file dengan folder terpisah per tahun  

### Untuk Admin/IT

✓ Setup di server lokal untuk offline use  
✓ Share link aplikasi ke semua guru  
✓ Maintain backup data CSV  
✓ Monitor performance dengan banyak siswa  

---

## ✨ Fitur Bonus yang Bermanfaat

### Fitur Hidden yang Jarang Tahu

- **Multiple Sheets**: Excel dengan >1 sheet otomatis terdeteksi
- **Keyboard Shortcut**: Ctrl+P untuk cetak
- **Offline Mode**: Download ZIP untuk offline access
- **Format Kelas Fleksibel**: 10-A, 10A, X-A, semua support
- **Large Files**: Support hingga 10,000 siswa sekaligus

---

## 📊 Next Steps

### Setelah Selesai Cetak

1. **Bagikan kepada guru**: Share link aplikasi
2. **Training ringan**: Ajari guru cara pakai
3. **Feedback**: Tanya apakah ada masalah
4. **Iteration**: Update data tahun depan

### Untuk Advanced Users

- Integrate dengan database sekolah
- Automate dengan barcode scanner
- Real-time attendance tracking
- Export ke sistem absensi digital

---

## 🎓 Learning Resources

- [Baca dokumentasi full](README.md)
- [Tonton tutorial video](#) (akan segera tersedia)
- [Join komunitas Discord](#) (akan segera tersedia)
- [Baca blog tips & tricks](#) (akan segera tersedia)

---

**Siap mulai? Download file dan buka di browser! 🚀**

Punya pertanyaan? [Buka issue di GitHub](https://github.com/username/barcode-absensi-generator/issues) atau email support@example.com

---

Last updated: 2026-03-21